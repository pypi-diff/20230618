# Comparing `tmp/texasholdem-0.8a0.tar.gz` & `tmp/texasholdem-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texasholdem-0.8a0.tar", max compression
+gzip compressed data, was "texasholdem-0.9.0.tar", max compression
```

## Comparing `texasholdem-0.8a0.tar` & `texasholdem-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1089 2022-11-03 05:47:50.122739 texasholdem-0.8a0/LICENSE
--rw-r--r--   0        0        0     7338 2022-11-03 05:47:50.122739 texasholdem-0.8a0/README.md
--rw-r--r--   0        0        0     1142 2022-11-03 05:47:50.130739 texasholdem-0.8a0/pyproject.toml
--rw-r--r--   0        0        0      106 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/__init__.py
--rw-r--r--   0        0        0      165 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/agents/__init__.py
--rw-r--r--   0        0        0     2385 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/agents/basic.py
--rw-r--r--   0        0        0      146 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/card/__init__.py
--rw-r--r--   0        0        0     8998 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/card/card.py
--rw-r--r--   0        0        0     1791 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/card/deck.py
--rw-r--r--   0        0        0      174 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/evaluator/__init__.py
--rw-r--r--   0        0        0     3173 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/evaluator/evaluator.py
--rw-r--r--   0        0        0     9846 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/evaluator/lookup_table.py
--rw-r--r--   0        0        0      441 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/game/__init__.py
--rw-r--r--   0        0        0      462 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/game/action_type.py
--rw-r--r--   0        0        0    44637 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/game/game.py
--rw-r--r--   0        0        0     2000 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/game/hand_phase.py
--rw-r--r--   0        0        0    21950 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/game/history.py
--rw-r--r--   0        0        0      918 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/game/player_state.py
--rw-r--r--   0        0        0      134 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/gui/__init__.py
--rw-r--r--   0        0        0     7480 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/gui/abstract_gui.py
--rw-r--r--   0        0        0    33206 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/gui/text_gui.py
--rw-r--r--   0        0        0        0 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/util/__init__.py
--rw-r--r--   0        0        0       61 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/util/errors.py
--rw-r--r--   0        0        0     2733 2022-11-03 05:47:50.134739 texasholdem-0.8a0/texasholdem/util/functions.py
--rw-r--r--   0        0        0     8265 1970-01-01 00:00:00.000000 texasholdem-0.8a0/setup.py
--rw-r--r--   0        0        0     8173 1970-01-01 00:00:00.000000 texasholdem-0.8a0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-03-13 21:04:22.933574 texasholdem-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7073 2023-03-13 21:04:22.933574 texasholdem-0.9.0/README.md
+-rw-r--r--   0        0        0     1151 2023-03-13 21:04:22.941574 texasholdem-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/__init__.py
+-rw-r--r--   0        0        0      165 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/agents/__init__.py
+-rw-r--r--   0        0        0     1545 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/agents/basic.py
+-rw-r--r--   0        0        0      146 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/card/__init__.py
+-rw-r--r--   0        0        0     8998 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/card/card.py
+-rw-r--r--   0        0        0     1791 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/card/deck.py
+-rw-r--r--   0        0        0      174 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/evaluator/__init__.py
+-rw-r--r--   0        0        0     3173 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/evaluator/evaluator.py
+-rw-r--r--   0        0        0     9836 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/evaluator/lookup_table.py
+-rw-r--r--   0        0        0      489 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/game/__init__.py
+-rw-r--r--   0        0        0      462 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/game/action_type.py
+-rw-r--r--   0        0        0    46154 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/game/game.py
+-rw-r--r--   0        0        0     2000 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/game/hand_phase.py
+-rw-r--r--   0        0        0    21950 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/game/history.py
+-rw-r--r--   0        0        0     4221 2023-03-13 21:04:22.941574 texasholdem-0.9.0/texasholdem/game/move.py
+-rw-r--r--   0        0        0      918 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/game/player_state.py
+-rw-r--r--   0        0        0      134 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/gui/__init__.py
+-rw-r--r--   0        0        0     7480 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/gui/abstract_gui.py
+-rw-r--r--   0        0        0    33206 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/gui/text_gui.py
+-rw-r--r--   0        0        0        0 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/util/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/util/errors.py
+-rw-r--r--   0        0        0     2733 2023-03-13 21:04:22.945574 texasholdem-0.9.0/texasholdem/util/functions.py
+-rw-r--r--   0        0        0     7919 1970-01-01 00:00:00.000000 texasholdem-0.9.0/PKG-INFO
```

### Comparing `texasholdem-0.8a0/LICENSE` & `texasholdem-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/README.md` & `texasholdem-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,49 +2,37 @@
 ![Pytest Status](https://github.com/SirRender00/texasholdem/actions/workflows/pytest.yml/badge.svg)
 [![codecov](https://codecov.io/github/SirRender00/texasholdem/branch/main/graph/badge.svg?token=1PH1NHTGXP)](https://codecov.io/github/SirRender00/texasholdem)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://raw.githubusercontent.com/SirRender00/texasholdem/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/texasholdem/badge/?version=stable)](https://texasholdem.readthedocs.io/en/stable/?badge=stable)
 ![Pylint Status](https://github.com/SirRender00/texasholdem/actions/workflows/pylint.yml/badge.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-A python package for Texas Hold 'Em Poker providing
+A python package for Texas Hold 'Em Poker providing:
 - Fast evaluation of hand strengths 
 - Export & import human-readable game history
 - GUIs to view games and game history
 - Simple & complex agents 
 - Compliance with World Series of Poker Official Rules
 - And more
 
 | Version Name | Latest Tag | Release Notes | Patch Notes | Documentation | Release Date | End Support Date |
 | ------------ | ---------- | ------------- | ----------- | ------------- | ------------ | ---------------- |
-| 0.8          | v0.8-alpha.0     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8-alpha.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8-alpha.0) | [Documentation](https://texasholdem.readthedocs.io/en/0.8/) | 2 November 2022 | |
-| 0.7          | v0.7.2           | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.2) | [Documentation](https://texasholdem.readthedocs.io/en/0.7/) | 16 April 2022 | |
-| 0.6          | v0.6.5           | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.6.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.6.5) | [Documentation](https://texasholdem.readthedocs.io/en/0.6/) | 24 March 2022 | |
-| 0.5          | v0.5.3           | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.5.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.5.3) | [Documentation](https://texasholdem.readthedocs.io/en/0.5/) | 21 March 2022 | |
+| 0.9          | v0.9.0     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.9.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.9.0) | [Documentation](https://texasholdem.readthedocs.io/en/0.9/) | 14 March 2023 | |
+| 0.8          | v0.8.1     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8.1) | [Documentation](https://texasholdem.readthedocs.io/en/0.8/) | 6 November 2022 | 30 June 2023 |
+| 0.7          | v0.7.3     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.3) | [Documentation](https://texasholdem.readthedocs.io/en/0.7/) | 16 April 2022 | 30 June 2023 |
 
 Current Roadmap \
 [v1.0.0](https://github.com/SirRender00/texasholdem/wiki/Version-1.0.0-Roadmap)
 
-## Changelog v0.7
-This release features an overhaul to the GUI system and specifically the `TextGUI`
-had a massive overhaul.
+## Changelog v0.9
 
 ### Features
 
-- Added an `AbstractGUI` class for common functionality for all GUIs.
-- The new `TextGUI`
-    - A new history panel
-    - Support any number of players 2 thru 9
-    - Chip animations
-    - Improved UX
-
-### Other Changes
-
-- Simplification of a few steps in a betting round
-- Uncaps the python dependency
+- New class `texasholdem.game.move.MoveIterator` which is a special collection of moves which includes attributes such as `action_types` and `raise_range`. Also supports iteration and checking for membership with the `in` operator. Use the `sample()` method to sample from the collection.
+- New method `texasholdem.game.game.TexasHoldEm.get_available_moves()` which returns a `MoveIterator` of the available moves for the current player.
 
 ## Contributing
 Want a new feature, found a bug, or have questions? Feel free to add to our issue board on Github!
 [Open Issues](https://github.com/SirRender00/texasholdem/issues>).
 
 We welcome any developer who enjoys the package enough to contribute! Please message me at evyn.machi@gmail.com
 if you want to be added as a contributor and check out the
```

### Comparing `texasholdem-0.8a0/pyproject.toml` & `texasholdem-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "texasholdem"
-version = "0.8-alpha.0"
+version = "0.9.0"
 description = "A texasholdem python package"
 authors = ["Evyn Machi <evyn.machi@gmail.com>"]
 keywords = ['texasholdem', 'holdem', 'poker']
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/SirRender00/texasholdem"
 repository = "https://github.com/SirRender00/texasholdem"
@@ -18,24 +18,25 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/SirRender00/texasholdem/issues"
 "Wiki" = "https://github.com/SirRender00/texasholdem/wiki"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Deprecated = "^1.2.13"
-windows-curses = { version = "^2.3.1a2", markers = "sys_platform == 'win32'" }
+windows-curses = { version = "^2.3.1", markers = "sys_platform == 'win32'" }
 
 [tool.poetry.dev-dependencies]
 py = "^1.11.0"
 pytest = "^7.2.0"
 pytest-parallel = "^0.1.1"
-pylint = "^2.15.5"
-sphinx-rtd-theme = "^1.0.0"
-black = "^22.10.0"
-coverage = "^6.5.0"
+pylint = "^2.17.0"
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+black = "^23.1.0"
+coverage = "^7.1.0"
 
 [tool.pylint.master]
 disable = ["import-error", "missing-module-docstring", "unknown-option-value"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `texasholdem-0.8a0/texasholdem/agents/basic.py` & `texasholdem-0.9.0/texasholdem/agents/basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,14 @@
     - :func:`call_agent`
     - :func:`random_agent`
 
 """
 
 from typing import Tuple
 
-import random
-
 from texasholdem.game.game import TexasHoldEm
 from texasholdem.game.action_type import ActionType
 from texasholdem.game.player_state import PlayerState
 
 
 def call_agent(game: TexasHoldEm) -> Tuple[ActionType, None]:
     """
@@ -42,34 +40,12 @@
         game (TexasHoldEm): The TexasHoldEm game
         no_fold (bool): Removes the possibility of folding if no one raised, default False.
     Returns:
         Tuple[ActionType, int]: Returns a uniformly random action from the
             available moves.
 
     """
-    bet_amount = game.player_bet_amount(game.current_player)
-    chips = game.players[game.current_player].chips
-    min_raise = game.value_to_total(game.min_raise(), game.current_player)
-    max_raise = bet_amount + chips
-
-    possible = list(ActionType)
-    possible.remove(ActionType.ALL_IN)
-
-    # A player did not raise
-    if game.players[game.current_player].state == PlayerState.IN:
-        possible.remove(ActionType.CALL)
-        if no_fold:
-            possible.remove(ActionType.FOLD)
-
-    # A player raised
-    if game.players[game.current_player].state == PlayerState.TO_CALL:
-        possible.remove(ActionType.CHECK)
-
-    # not enough chips to raise
-    if max_raise < min_raise:
-        possible.remove(ActionType.RAISE)
-
-    action_type, total = random.choice(possible), None
-    if action_type == ActionType.RAISE:
-        total = random.randint(min_raise, max_raise)
+    moves = game.get_available_moves()
+    if no_fold:
+        del moves[ActionType.FOLD]
 
-    return action_type, total
+    return moves.sample()
```

### Comparing `texasholdem-0.8a0/texasholdem/card/card.py` & `texasholdem-0.9.0/texasholdem/card/card.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/card/deck.py` & `texasholdem-0.9.0/texasholdem/card/deck.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/evaluator/evaluator.py` & `texasholdem-0.9.0/texasholdem/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/evaluator/lookup_table.py` & `texasholdem-0.9.0/texasholdem/evaluator/lookup_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,43 +186,40 @@
         backwards_ranks = range(len(Card.INT_RANKS) - 1, -1, -1)
 
         # 1) Four of a Kind
         rank = LookupTable.MAX_STRAIGHT_FLUSH + 1
 
         # for each choice of a set of four rank
         for i in backwards_ranks:
-
             # and for each possible kicker rank
             kickers = list(backwards_ranks[:])
             kickers.remove(i)
             for k in kickers:
                 product = Card.PRIMES[i] ** 4 * Card.PRIMES[k]
                 self.unsuited_lookup[product] = rank
                 rank += 1
 
         # 2) Full House
         rank = LookupTable.MAX_FOUR_OF_A_KIND + 1
 
         # for each three of a kind
         for i in backwards_ranks:
-
             # and for each choice of pair rank
             pair_ranks = list(backwards_ranks[:])
             pair_ranks.remove(i)
             for pair_rank in pair_ranks:
                 product = Card.PRIMES[i] ** 3 * Card.PRIMES[pair_rank] ** 2
                 self.unsuited_lookup[product] = rank
                 rank += 1
 
         # 3) Three of a Kind
         rank = LookupTable.MAX_STRAIGHT + 1
 
         # pick three of one rank
         for b_rank in backwards_ranks:
-
             kickers = list(backwards_ranks[:])
             kickers.remove(b_rank)
 
             for kickers in itertools.combinations(kickers, 2):
                 card1, card2 = kickers
                 product = (
                     Card.PRIMES[b_rank] ** 3 * Card.PRIMES[card1] * Card.PRIMES[card2]
@@ -230,15 +227,14 @@
                 self.unsuited_lookup[product] = rank
                 rank += 1
 
         # 4) Two Pair
         rank = LookupTable.MAX_THREE_OF_A_KIND + 1
 
         for two_pair in itertools.combinations(backwards_ranks, 2):
-
             pair1, pair2 = two_pair
             kickers = list(backwards_ranks[:])
             kickers.remove(pair1)
             kickers.remove(pair2)
             for kicker in kickers:
                 product = (
                     Card.PRIMES[pair1] ** 2
@@ -249,15 +245,14 @@
                 rank += 1
 
         # 5) Pair
         rank = LookupTable.MAX_TWO_PAIR + 1
 
         # choose a pair
         for pairrank in backwards_ranks:
-
             kickers = list(backwards_ranks[:])
             kickers.remove(pairrank)
 
             for kickers in itertools.combinations(kickers, 3):
                 kicker1, kicker2, kicker3 = kickers
                 product = (
                     Card.PRIMES[pairrank] ** 2
```

### Comparing `texasholdem-0.8a0/texasholdem/game/game.py` & `texasholdem-0.9.0/texasholdem/game/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     PlayerAction,
     HistoryImportError,
     SettleHistory,
 )
 from texasholdem.game.action_type import ActionType
 from texasholdem.game.hand_phase import HandPhase
 from texasholdem.game.player_state import PlayerState
+from texasholdem.game.move import MoveIterator
 from texasholdem.evaluator import evaluator
 from texasholdem.util.functions import check_raise
 
 
 class Player:
     # pylint: disable=too-few-public-methods
     """
@@ -689,15 +690,15 @@
             return None
         return value + self.chips_to_call(player_id) + self.player_bet_amount(player_id)
 
     @versionadded(version="0.6.0")
     def min_raise(self):
         """
         Returns:
-            The minimum amount a player can raise by.
+            int: The minimum amount a player can raise by.
         """
         return max(self.big_blind, self.last_raise)
 
     @check_raise(ValueError)
     @versionchanged(
         reason="The :code:`value` has been renamed to :code:`total` and will "
         "be redefined in 1.0.0. Currently, :code:`value` and :code:`total` "
@@ -819,14 +820,49 @@
                 return (
                     False,
                     f"Expected raise value {new_total} to be more "
                     f"than the chips to call {chips_to_call}",
                 )
         return True, ""
 
+    @versionadded(version="0.9.0")
+    def get_available_moves(self):
+        """
+        Returns:
+            MoveIterator: A special iterator over the possible moves for the current player,
+                includes attributes such as :attr:`~texasholdem.game.move.action_types` and
+                :attr:`~texasholdem.game.move.raise_range`.
+        """
+        bet_amount = self.player_bet_amount(self.current_player)
+        chips = self.players[self.current_player].chips
+        min_raise = self.value_to_total(self.min_raise(), self.current_player)
+        max_raise = bet_amount + chips
+
+        possible = {action: None for action in ActionType}
+        possible[ActionType.RAISE] = range(min_raise, max_raise + 1)
+        del possible[ActionType.ALL_IN]
+
+        # A player did not raise
+        if self.players[self.current_player].state == PlayerState.IN:
+            del possible[ActionType.CALL]
+
+        # A player raised
+        if self.players[self.current_player].state == PlayerState.TO_CALL:
+            del possible[ActionType.CHECK]
+
+        # not enough chips to raise
+        if not self.raise_option:
+            del possible[ActionType.RAISE]
+        elif max_raise < min_raise:
+            del possible[ActionType.RAISE]
+            if chips > self.chips_to_call(self.current_player):
+                possible[ActionType.RAISE] = range(max_raise, max_raise + 1)
+
+        return MoveIterator(possible)
+
     def _take_action(self, action: ActionType, total: Optional[int] = None):
         """
         Execute the action for the current player. Assumes the move is valid.
 
         Arguments:
             action (ActionType): The ActionType to take
             total (int, optional): In the case of raise, how much to raise *to*
```

### Comparing `texasholdem-0.8a0/texasholdem/game/hand_phase.py` & `texasholdem-0.9.0/texasholdem/game/hand_phase.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/game/history.py` & `texasholdem-0.9.0/texasholdem/game/history.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/game/player_state.py` & `texasholdem-0.9.0/texasholdem/game/player_state.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/gui/abstract_gui.py` & `texasholdem-0.9.0/texasholdem/gui/abstract_gui.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/gui/text_gui.py` & `texasholdem-0.9.0/texasholdem/gui/text_gui.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/texasholdem/util/functions.py` & `texasholdem-0.9.0/texasholdem/util/functions.py`

 * *Files identical despite different names*

### Comparing `texasholdem-0.8a0/setup.py` & `texasholdem-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,201 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: texasholdem
+Version: 0.9.0
+Summary: A texasholdem python package
+Home-page: https://github.com/SirRender00/texasholdem
+License: MIT
+Keywords: texasholdem,holdem,poker
+Author: Evyn Machi
+Author-email: evyn.machi@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
+Requires-Dist: windows-curses (>=2.3.1,<3.0.0) ; sys_platform == "win32"
+Project-URL: Bug Tracker, https://github.com/SirRender00/texasholdem/issues
+Project-URL: Documentation, https://texasholdem.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/SirRender00/texasholdem
+Project-URL: Wiki, https://github.com/SirRender00/texasholdem/wiki
+Description-Content-Type: text/markdown
+
+# texasholdem
+![Pytest Status](https://github.com/SirRender00/texasholdem/actions/workflows/pytest.yml/badge.svg)
+[![codecov](https://codecov.io/github/SirRender00/texasholdem/branch/main/graph/badge.svg?token=1PH1NHTGXP)](https://codecov.io/github/SirRender00/texasholdem)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://raw.githubusercontent.com/SirRender00/texasholdem/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/texasholdem/badge/?version=stable)](https://texasholdem.readthedocs.io/en/stable/?badge=stable)
+![Pylint Status](https://github.com/SirRender00/texasholdem/actions/workflows/pylint.yml/badge.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A python package for Texas Hold 'Em Poker providing:
+- Fast evaluation of hand strengths 
+- Export & import human-readable game history
+- GUIs to view games and game history
+- Simple & complex agents 
+- Compliance with World Series of Poker Official Rules
+- And more
+
+| Version Name | Latest Tag | Release Notes | Patch Notes | Documentation | Release Date | End Support Date |
+| ------------ | ---------- | ------------- | ----------- | ------------- | ------------ | ---------------- |
+| 0.9          | v0.9.0     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.9.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.9.0) | [Documentation](https://texasholdem.readthedocs.io/en/0.9/) | 14 March 2023 | |
+| 0.8          | v0.8.1     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8.1) | [Documentation](https://texasholdem.readthedocs.io/en/0.8/) | 6 November 2022 | 30 June 2023 |
+| 0.7          | v0.7.3     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.3) | [Documentation](https://texasholdem.readthedocs.io/en/0.7/) | 16 April 2022 | 30 June 2023 |
+
+Current Roadmap \
+[v1.0.0](https://github.com/SirRender00/texasholdem/wiki/Version-1.0.0-Roadmap)
+
+## Changelog v0.9
+
+### Features
+
+- New class `texasholdem.game.move.MoveIterator` which is a special collection of moves which includes attributes such as `action_types` and `raise_range`. Also supports iteration and checking for membership with the `in` operator. Use the `sample()` method to sample from the collection.
+- New method `texasholdem.game.game.TexasHoldEm.get_available_moves()` which returns a `MoveIterator` of the available moves for the current player.
+
+## Contributing
+Want a new feature, found a bug, or have questions? Feel free to add to our issue board on Github!
+[Open Issues](https://github.com/SirRender00/texasholdem/issues>).
+
+We welcome any developer who enjoys the package enough to contribute! Please message me at evyn.machi@gmail.com
+if you want to be added as a contributor and check out the 
+[Developer's Guide](https://github.com/SirRender00/texasholdem/wiki/Developer's-Guide).
+
+## Install
+The package is available on pypi and can be installed with
+
+```bash
+pip install texasholdem
+```
+
+For the latest experimental version
+```bash
+pip install texasholdem --pre
+```
+
+## Quickstart
+Play a game from the command line and take turns for every player out of the box.
+
+```python
+from texasholdem.game.game import TexasHoldEm
+from texasholdem.gui.text_gui import TextGUI
+
+game = TexasHoldEm(buyin=500, big_blind=5, small_blind=2, max_players=6)
+gui = TextGUI(game=game)
+
+while game.is_game_running():
+    game.start_hand()
+
+    while game.is_hand_running():
+        gui.run_step()
+
+    path = game.export_history('./pgns')     # save history
+    gui.replay_history(path)                 # replay history
+```
+
+## Overview
+The following is a quick summary of what's in the package. Please see the 
+[docs](https://texasholdem.readthedocs.io/en/stable/) for all the details.
+
+### Game Information
+
+Get game information and take actions through intuitive attributes.
+
+```python
+from texasholdem import TexasHoldEm, HandPhase, ActionType
+
+game = TexasHoldEm(buyin=500,
+                   big_blind=5,
+                   small_blind=2,
+                   max_players=9)
+game.start_hand()
+
+assert game.hand_phase == HandPhase.PREFLOP
+assert HandPhase.PREFLOP.next_phase() == HandPhase.FLOP
+assert game.chips_to_call(game.current_player) == game.big_blind
+assert len(game.get_hand(game.current_player)) == 2
+
+game.take_action(ActionType.CALL)
+
+player_id = game.current_player
+game.take_action(ActionType.RAISE, total=10)
+assert game.player_bet_amount(player_id) == 10
+assert game.chips_at_stake(player_id) == 20     # total amount in all pots the player is in
+
+assert game.chips_to_call(game.current_player) == 10 - game.big_blind
+```
+
+### Cards
+The card module represents cards as 32-bit integers for simple and fast hand
+evaluations.
+
+```python
+from texasholdem import Card
+
+card = Card("Kd")                       # King of Diamonds
+assert isinstance(card, int)            # True
+assert card.rank == 11                  # 2nd highest rank (0-12)
+assert card.pretty_string == "[ K ♦ ]"
+```
+
+### Agents
+The package also comes with basic agents including `call_agent` and `random_agent`
+
+```python
+from texasholdem import TexasHoldEm
+from texasholdem.agents import random_agent, call_agent
+
+game = TexasHoldEm(buyin=500, big_blind=5, small_blind=2)
+game.start_hand()
+
+while game.is_hand_running():
+    if game.current_player % 2 == 0:
+        game.take_action(*random_agent(game))
+    else:
+        game.take_action(*call_agent(game))
+```
+
+### Game History
+Export and import the history of hands to files.
+
+```python
+from texasholdem import TexasHoldEm
+from texasholdem.gui import TextGUI
+
+game = TexasHoldEm(buyin=500, big_blind=5, small_blind=2)
+game.start_hand()
+
+while game.is_hand_running():
+    game.take_action(*some_strategy(game))
+
+# export to file
+game.export_history("./pgns/my_game.pgn")
+
+# import and replay
+gui = TextGUI()
+gui.replay_history("./pgns/my_game.pgn")
+```
+PGN files also support single line and end of line comments starting with "#".
+
+### Poker Evaluator
+The evaluator module returns the rank of the best 5-card hand from a list of 5 to 7 cards.
+The rank is a number from 1 (strongest) to 7462 (weakest).
+
+```python
+from texasholdem import Card
+from texasholdem.evaluator import  evaluate, rank_to_string
+
+assert evaluate(cards=[Card("Kd"), Card("5d")],
+                board=[Card("Qd"),
+                       Card("6d"),
+                       Card("5s"),
+                       Card("2d"),
+                       Card("5h")]) == 927
+assert rank_to_string(927) == "Flush, King High"
+```
+
+### GUIs
+The GUI package currently comes with a text-based GUI to play games from the command line. Coming later
+will be web-app based GUIs.
 
-packages = \
-['texasholdem',
- 'texasholdem.agents',
- 'texasholdem.card',
- 'texasholdem.evaluator',
- 'texasholdem.game',
- 'texasholdem.gui',
- 'texasholdem.util']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Deprecated>=1.2.13,<2.0.0']
-
-extras_require = \
-{':sys_platform == "win32"': ['windows-curses>=2.3.1a2,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'texasholdem',
-    'version': '0.8a0',
-    'description': 'A texasholdem python package',
-    'long_description': '# texasholdem\n![Pytest Status](https://github.com/SirRender00/texasholdem/actions/workflows/pytest.yml/badge.svg)\n[![codecov](https://codecov.io/github/SirRender00/texasholdem/branch/main/graph/badge.svg?token=1PH1NHTGXP)](https://codecov.io/github/SirRender00/texasholdem)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://raw.githubusercontent.com/SirRender00/texasholdem/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/texasholdem/badge/?version=stable)](https://texasholdem.readthedocs.io/en/stable/?badge=stable)\n![Pylint Status](https://github.com/SirRender00/texasholdem/actions/workflows/pylint.yml/badge.svg)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nA python package for Texas Hold \'Em Poker providing\n- Fast evaluation of hand strengths \n- Export & import human-readable game history\n- GUIs to view games and game history\n- Simple & complex agents \n- Compliance with World Series of Poker Official Rules\n- And more\n\n| Version Name | Latest Tag | Release Notes | Patch Notes | Documentation | Release Date | End Support Date |\n| ------------ | ---------- | ------------- | ----------- | ------------- | ------------ | ---------------- |\n| 0.8          | v0.8-alpha.0     | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8-alpha.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.8-alpha.0) | [Documentation](https://texasholdem.readthedocs.io/en/0.8/) | 2 November 2022 | |\n| 0.7          | v0.7.2           | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.7.2) | [Documentation](https://texasholdem.readthedocs.io/en/0.7/) | 16 April 2022 | |\n| 0.6          | v0.6.5           | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.6.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.6.5) | [Documentation](https://texasholdem.readthedocs.io/en/0.6/) | 24 March 2022 | |\n| 0.5          | v0.5.3           | [Release Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.5.0) | [Patch Notes](https://github.com/SirRender00/texasholdem/releases/tag/v0.5.3) | [Documentation](https://texasholdem.readthedocs.io/en/0.5/) | 21 March 2022 | |\n\nCurrent Roadmap \\\n[v1.0.0](https://github.com/SirRender00/texasholdem/wiki/Version-1.0.0-Roadmap)\n\n## Changelog v0.7\nThis release features an overhaul to the GUI system and specifically the `TextGUI`\nhad a massive overhaul.\n\n### Features\n\n- Added an `AbstractGUI` class for common functionality for all GUIs.\n- The new `TextGUI`\n    - A new history panel\n    - Support any number of players 2 thru 9\n    - Chip animations\n    - Improved UX\n\n### Other Changes\n\n- Simplification of a few steps in a betting round\n- Uncaps the python dependency\n\n## Contributing\nWant a new feature, found a bug, or have questions? Feel free to add to our issue board on Github!\n[Open Issues](https://github.com/SirRender00/texasholdem/issues>).\n\nWe welcome any developer who enjoys the package enough to contribute! Please message me at evyn.machi@gmail.com\nif you want to be added as a contributor and check out the \n[Developer\'s Guide](https://github.com/SirRender00/texasholdem/wiki/Developer\'s-Guide).\n\n## Install\nThe package is available on pypi and can be installed with\n\n```bash\npip install texasholdem\n```\n\nFor the latest experimental version\n```bash\npip install texasholdem --pre\n```\n\n## Quickstart\nPlay a game from the command line and take turns for every player out of the box.\n\n```python\nfrom texasholdem.game.game import TexasHoldEm\nfrom texasholdem.gui.text_gui import TextGUI\n\ngame = TexasHoldEm(buyin=500, big_blind=5, small_blind=2, max_players=6)\ngui = TextGUI(game=game)\n\nwhile game.is_game_running():\n    game.start_hand()\n\n    while game.is_hand_running():\n        gui.run_step()\n\n    path = game.export_history(\'./pgns\')     # save history\n    gui.replay_history(path)                 # replay history\n```\n\n## Overview\nThe following is a quick summary of what\'s in the package. Please see the \n[docs](https://texasholdem.readthedocs.io/en/stable/) for all the details.\n\n### Game Information\n\nGet game information and take actions through intuitive attributes.\n\n```python\nfrom texasholdem import TexasHoldEm, HandPhase, ActionType\n\ngame = TexasHoldEm(buyin=500,\n                   big_blind=5,\n                   small_blind=2,\n                   max_players=9)\ngame.start_hand()\n\nassert game.hand_phase == HandPhase.PREFLOP\nassert HandPhase.PREFLOP.next_phase() == HandPhase.FLOP\nassert game.chips_to_call(game.current_player) == game.big_blind\nassert len(game.get_hand(game.current_player)) == 2\n\ngame.take_action(ActionType.CALL)\n\nplayer_id = game.current_player\ngame.take_action(ActionType.RAISE, total=10)\nassert game.player_bet_amount(player_id) == 10\nassert game.chips_at_stake(player_id) == 20     # total amount in all pots the player is in\n\nassert game.chips_to_call(game.current_player) == 10 - game.big_blind\n```\n\n### Cards\nThe card module represents cards as 32-bit integers for simple and fast hand\nevaluations.\n\n```python\nfrom texasholdem import Card\n\ncard = Card("Kd")                       # King of Diamonds\nassert isinstance(card, int)            # True\nassert card.rank == 11                  # 2nd highest rank (0-12)\nassert card.pretty_string == "[ K ♦ ]"\n```\n\n### Agents\nThe package also comes with basic agents including `call_agent` and `random_agent`\n\n```python\nfrom texasholdem import TexasHoldEm\nfrom texasholdem.agents import random_agent, call_agent\n\ngame = TexasHoldEm(buyin=500, big_blind=5, small_blind=2)\ngame.start_hand()\n\nwhile game.is_hand_running():\n    if game.current_player % 2 == 0:\n        game.take_action(*random_agent(game))\n    else:\n        game.take_action(*call_agent(game))\n```\n\n### Game History\nExport and import the history of hands to files.\n\n```python\nfrom texasholdem import TexasHoldEm\nfrom texasholdem.gui import TextGUI\n\ngame = TexasHoldEm(buyin=500, big_blind=5, small_blind=2)\ngame.start_hand()\n\nwhile game.is_hand_running():\n    game.take_action(*some_strategy(game))\n\n# export to file\ngame.export_history("./pgns/my_game.pgn")\n\n# import and replay\ngui = TextGUI()\ngui.replay_history("./pgns/my_game.pgn")\n```\nPGN files also support single line and end of line comments starting with "#".\n\n### Poker Evaluator\nThe evaluator module returns the rank of the best 5-card hand from a list of 5 to 7 cards.\nThe rank is a number from 1 (strongest) to 7462 (weakest).\n\n```python\nfrom texasholdem import Card\nfrom texasholdem.evaluator import  evaluate, rank_to_string\n\nassert evaluate(cards=[Card("Kd"), Card("5d")],\n                board=[Card("Qd"),\n                       Card("6d"),\n                       Card("5s"),\n                       Card("2d"),\n                       Card("5h")]) == 927\nassert rank_to_string(927) == "Flush, King High"\n```\n\n### GUIs\nThe GUI package currently comes with a text-based GUI to play games from the command line. Coming later\nwill be web-app based GUIs.\n',
-    'author': 'Evyn Machi',
-    'author_email': 'evyn.machi@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/SirRender00/texasholdem',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

