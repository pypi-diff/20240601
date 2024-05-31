# Comparing `tmp/pkrcomponents-2.0.0.tar.gz` & `tmp/pkrcomponents-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-2.0.0.tar", last modified: Fri May 31 18:46:10 2024, max compression
+gzip compressed data, was "pkrcomponents-2.0.1.tar", last modified: Fri May 31 21:36:25 2024, max compression
```

## Comparing `pkrcomponents-2.0.0.tar` & `pkrcomponents-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:09.745436 pkrcomponents-2.0.0/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-2.0.0/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-2.0.0/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-2.0.0/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-2.0.0/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-31 18:42:51.000000 pkrcomponents-2.0.0/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.023970 pkrcomponents-2.0.0/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4097 2024-05-31 18:42:39.000000 pkrcomponents-2.0.0/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-2.0.0/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4030 2024-05-29 18:47:23.000000 pkrcomponents-2.0.0/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-2.0.0/pkrcomponents/buy_in.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-2.0.0/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-2.0.0/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1401 2024-05-29 11:06:38.000000 pkrcomponents-2.0.0/pkrcomponents/deck.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-2.0.0/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-2.0.0/pkrcomponents/level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-2.0.0/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/lookup_table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-2.0.0/pkrcomponents/payout.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5171 2024-05-29 13:53:41.000000 pkrcomponents-2.0.0/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-2.0.0/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    18160 2024-05-31 17:25:18.000000 pkrcomponents-2.0.0/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13465 2024-05-31 18:42:39.000000 pkrcomponents-2.0.0/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3422 2024-05-31 18:42:39.000000 pkrcomponents-2.0.0/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.087520 pkrcomponents-2.0.0/pkrcomponents/utils/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-2.0.0/pkrcomponents/utils/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      185 2024-05-31 18:09:47.000000 pkrcomponents-2.0.0/pkrcomponents/utils/converters.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-2.0.0/pkrcomponents/utils/validators.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      693 2024-05-31 18:46:08.000000 pkrcomponents-2.0.0/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-2.0.0/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 21:36:25.679315 pkrcomponents-2.0.1/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 21:36:25.161927 pkrcomponents-2.0.1/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-2.0.1/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-2.0.1/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-2.0.1/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-31 21:36:25.669501 pkrcomponents-2.0.1/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-2.0.1/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-31 21:34:14.000000 pkrcomponents-2.0.1/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 21:36:25.559239 pkrcomponents-2.0.1/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-2.0.1/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-2.0.1/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4097 2024-05-31 18:42:39.000000 pkrcomponents-2.0.1/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-2.0.1/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4030 2024-05-29 18:47:23.000000 pkrcomponents-2.0.1/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-2.0.1/pkrcomponents/buy_in.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-2.0.1/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-2.0.1/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1416 2024-05-31 20:38:00.000000 pkrcomponents-2.0.1/pkrcomponents/deck.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-2.0.1/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-2.0.1/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-2.0.1/pkrcomponents/level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-2.0.1/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-2.0.1/pkrcomponents/lookup_table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-2.0.1/pkrcomponents/payout.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5171 2024-05-29 13:53:41.000000 pkrcomponents-2.0.1/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-2.0.1/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    18239 2024-05-31 20:49:49.000000 pkrcomponents-2.0.1/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13465 2024-05-31 18:42:39.000000 pkrcomponents-2.0.1/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3422 2024-05-31 18:42:39.000000 pkrcomponents-2.0.1/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 21:36:25.619491 pkrcomponents-2.0.1/pkrcomponents/utils/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-2.0.1/pkrcomponents/utils/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      314 2024-05-31 19:39:16.000000 pkrcomponents-2.0.1/pkrcomponents/utils/converters.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-2.0.1/pkrcomponents/utils/validators.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 21:36:25.659039 pkrcomponents-2.0.1/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      715 2024-05-31 21:36:24.000000 pkrcomponents-2.0.1/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-2.0.1/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-31 21:36:25.679315 pkrcomponents-2.0.1/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-2.0.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 21:36:25.651532 pkrcomponents-2.0.1/site/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       51 2024-05-31 21:34:27.000000 pkrcomponents-2.0.1/site/requirements.txt
```

### Comparing `pkrcomponents-2.0.0/LICENSE.txt` & `pkrcomponents-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/MANIFEST.in` & `pkrcomponents-2.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/PKG-INFO` & `pkrcomponents-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-2.0.0/coverage.txt` & `pkrcomponents-2.0.1/coverage.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 pkrcomponents/hand.py                 228      0   100%
 pkrcomponents/level.py                 17      0   100%
 pkrcomponents/listings.py              16      0   100%
 pkrcomponents/lookup_table.py         112      0   100%
 pkrcomponents/payout.py                37      0   100%
 pkrcomponents/players.py              109      0   100%
 pkrcomponents/pot.py                   13      0   100%
-pkrcomponents/table.py                345      2    99%
+pkrcomponents/table.py                270      1    99%
 pkrcomponents/table_player.py         157      1    99%
 pkrcomponents/tournament.py            46      0   100%
 pkrcomponents/utils/__init__.py         0      0   100%
-pkrcomponents/utils/converters.py       3      0   100%
+pkrcomponents/utils/converters.py       5      0   100%
 pkrcomponents/utils/validators.py       7      0   100%
 -------------------------------------------------------
-TOTAL                                1571      4    99%
+TOTAL                                1498      3    99%
```

### Comparing `pkrcomponents-2.0.0/pkrcomponents/_common.py` & `pkrcomponents-2.0.1/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/action.py` & `pkrcomponents-2.0.1/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/bitcard.py` & `pkrcomponents-2.0.1/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/board.py` & `pkrcomponents-2.0.1/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/buy_in.py` & `pkrcomponents-2.0.1/pkrcomponents/buy_in.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/card.py` & `pkrcomponents-2.0.1/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/constants.py` & `pkrcomponents-2.0.1/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/deck.py` & `pkrcomponents-2.0.1/pkrcomponents/deck.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         random.shuffle(self.cards)
 
     def reset(self):
         """Re-initializes the deck and shuffles it"""
         self.cards = list(Card)
         self.shuffle()
 
-    def draw(self, card=None):
+    def draw(self, card: (str, Card) = None):
         """
         Returns a card from the deck
         If the parameter card is given, it returns the card at stake and pops it from the deck
         """
         if not card:
             return self.cards.pop()
         else:
```

### Comparing `pkrcomponents-2.0.0/pkrcomponents/evaluator.py` & `pkrcomponents-2.0.1/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/hand.py` & `pkrcomponents-2.0.1/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/level.py` & `pkrcomponents-2.0.1/pkrcomponents/level.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/listings.py` & `pkrcomponents-2.0.1/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/lookup_table.py` & `pkrcomponents-2.0.1/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/payout.py` & `pkrcomponents-2.0.1/pkrcomponents/payout.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/players.py` & `pkrcomponents-2.0.1/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/pot.py` & `pkrcomponents-2.0.1/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/table.py` & `pkrcomponents-2.0.1/pkrcomponents/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,98 @@
+from attrs import define, field, Factory
+from attrs.validators import instance_of, optional, ge, gt, le
+
 from pkrcomponents.board import Board
+from pkrcomponents.card import Card
 from pkrcomponents.deck import Deck
 from pkrcomponents.constants import Street
 from pkrcomponents.players import Players
 from pkrcomponents.pot import Pot
 from pkrcomponents.tournament import Level, Tournament
 from pkrcomponents.evaluator import Evaluator
+from pkrcomponents.utils.converters import convert_to_street
 
 
+@define
 class Table:
-    """Class representing a poker table"""
-    _board: Board
-    _deck: Deck
-    _players: Players
-    _pots: [Pot]
-    _max_players: int
-    _is_mtt: bool
-    _tournament: Tournament
-    _level: Level
-    _street: Street
-    _seat_playing: int
-    _min_bet: float
-    _cnt_bets: int
-    _evaluator: Evaluator
-    _preflop_bet_factors = [1, 1.1, 1.25, 1.5, 2, 3.5, 5]
-    _postflop_bet_factors = [
+    """
+    This class represents a poker table
+
+    Attributes:
+        board(Board): The board of the table
+        cnt_bets(int): The number of bets made on the table
+        deck(Deck): The deck of the table
+        evaluator(Evaluator): The evaluator of the table
+        hand_has_started(bool): Whether the hand has started
+        is_mtt(bool): Whether the table is a tournament
+        level(Level): The level of the table
+        max_players(int): The maximum number of players on the table
+        min_bet(float): The minimum bet on the table
+        players(Players): The players on the table
+        pot(Pot): The pot of the table
+        seat_playing(int): The seat of the player currently playing
+        street(Street): The current street of the table
+        tournament(Tournament): The tournament associated with the table
+
+    Methods:
+
+
+    """
+    preflop_bet_factors = [1, 1.1, 1.25, 1.5, 2, 3.5, 5]
+    postflop_bet_factors = [
         {"text": "1/4 Pot", "value": 1 / 4},
         {"text": "1/3 Pot", "value": 1 / 3},
         {"text": "1/2 Pot", "value": 1 / 2},
         {"text": "2/3 Pot", "value": 2 / 3},
         {"text": "3/4 Pot", "value": 3 / 4},
         {"text": "Pot", "value": 1}
     ]
+    board = field(default=Factory(Board), validator=instance_of(Board))
+    cnt_bets = field(default=0, validator=[instance_of(int), ge(0)])
+    deck = field(default=Factory(Deck), validator=instance_of(Deck))
+    evaluator = field(default=Factory(Evaluator), validator=instance_of(Evaluator))
+    hand_has_started = field(default=False, validator=instance_of(bool))
+    is_mtt = field(default=False, validator=instance_of(bool))
+    level = field(default=Factory(Level), validator=instance_of(Level))
+    max_players = field(default=6, validator=[instance_of(int), gt(2), le(10)])
+    min_bet = field(default=0, validator=[instance_of(float), ge(0)], converter=float)
+    players = field(default=Factory(Players), validator=instance_of(Players))
+    pot = field(default=Factory(Pot), validator=instance_of(Pot))
+    seat_playing = field(default=0, validator=[instance_of(int), ge(0)])
+    street = field(default=None, validator=optional(instance_of(Street)), converter=convert_to_street)
+    tournament = field(default=None, validator=optional(instance_of(Tournament)))
 
-    def __init__(self, max_players=6):
-        self._board = Board()
-        self._deck = Deck()
-        self._deck.shuffle()
-        self._players = Players()
-        self._pot = Pot()
-        self._evaluator = Evaluator()
-        self._is_mtt = False
-        self._street = Street.PREFLOP
-        self.max_players = max_players
-        self._hand_has_started = False
-        self._cnt_bets = 0
-
-    @property
-    def board(self) -> Board:
-        """Returns the associated board """
-        return self._board
-
-    @property
-    def deck(self) -> Deck:
-        """Returns the associated deck """
-        return self._deck
-
-    @property
-    def players(self) -> Players:
-        """Returns the associated players """
-        return self._players
-
-    @property
-    def max_players(self) -> int:
-        """Returns the maximum players that can be added on this table"""
-        return self._max_players
-
-    @max_players.setter
-    def max_players(self, max_value):
-        """Setter for max players property"""
-        if max_value not in range(1, 11):
-            raise ValueError("Number of players should be between 1 and 10")
-        else:
-            self._max_players = max_value
+    def __attrs_post_init__(self):
+        self.deck.shuffle()
 
     @property
     def is_full(self) -> bool:
         """Returns True if the table is full"""
         return self.players.len == self.max_players
 
     @property
     def is_empty(self) -> bool:
         """Returns True if the table is empty"""
         return self.players.len == 0
 
     @property
-    def pot(self) -> Pot:
-        """Returns the associated pot """
-        return self._pot
-
-    @property
-    def tournament(self) -> Tournament or None:
-        """Returns the associated tournament """
-        return self._tournament
-
-    @property
-    def evaluator(self) -> Evaluator:
-        """Returns the associated evaluator"""
-        return self._evaluator
-
-    @tournament.setter
-    def tournament(self, tournament: Tournament):
-        """Setter for tournament property"""
-        self._tournament = tournament
-
-    @property
-    def street(self) -> Street:
-        """Returns table's current street"""
-        return self._street
-
-    @street.setter
-    def street(self, street: (str, Street)):
-        """Setter for street property"""
-        self._street = Street(street)
-
-    @property
-    def level(self) -> Level:
-        """Returns current level"""
-        if self._is_mtt:
-            return self._tournament.level
-        else:
-            return self._level
-
-    @level.setter
-    def level(self, level: Level):
-        """Setter for level property"""
-        self._level = level
-
-    @property
     def playing_order(self) -> list[int]:
         """Returns the list of the indexes of players on the table, with order depending on current street"""
-        if self._street == Street.PREFLOP:
+        if self.street == Street.PREFLOP:
             return self.players.preflop_ordered_seats
         else:
             return self.players.postflop_ordered_seats
 
     @property
-    def players_order(self):
+    def players_order(self) -> list:
         """Returns the players in playing order"""
         return [self.players[i] for i in self.playing_order]
 
     @property
-    def players_waiting(self):
+    def players_waiting(self) -> list:
         """Returns the list of players on the table that are waiting to play"""
         return [player for player in self.players_order if player.can_play]
 
     @property
     def street_ended(self) -> bool:
         """Returns True if the street has ended"""
         return len(self.players_waiting) == 0 or (
@@ -197,140 +145,195 @@
 
     @property
     def nb_involved(self) -> int:
         """Returns the number of players who didn't fold yet"""
         return len(self.players_involved)
 
     @property
-    def hand_has_started(self) -> bool:
-        """Returns True if the hand has started"""
-        return self._hand_has_started
-
-    @property
     def hand_can_start(self) -> bool:
         """Returns True if the hand can start"""
         return self.players.len >= 2 and not self.hand_has_started
 
     def start_hand(self):
         """Starts a new hand"""
-        self._hand_has_started = True
+        self.hand_has_started = True
         self.street = Street.PREFLOP
         self.street_reset()
         self.post_pregame()
 
-    def draw_flop(self, c1=None, c2=None, c3=None):
-        """For the flop, draws 3 cards in the deck and adds them on the board as flop cards"""
-        if len(self._board) > 0:
-            raise ValueError("Board must be empty before we can draw a flop")
-        c1 = self._deck.draw(c1)
-        c2 = self._deck.draw(c2)
-        c3 = self._deck.draw(c3)
-        self._board.add(c1)
-        self._board.add(c2)
-        self._board.add(c3)
+    def draw_flop(self, card1: (str, Card) = None, card2: (str, Card) = None, card3: (str, Card) = None):
+        """
+        For the flop, draws 3 cards in the deck and adds them on the board as flop cards
 
-    def flop(self, c1=None, c2=None, c3=None):
-        """Draw a flop and steps to this new street"""
+        Args:
+            card1 (str, Card): The first card to draw
+            card2 (str, Card): The second card to draw
+            card3 (str, Card): The third card to draw
+        """
+        if len(self.board) > 0:
+            raise ValueError("Board must be empty before we can draw a flop")
+        card1 = self.deck.draw(card1)
+        card2 = self.deck.draw(card2)
+        card3 = self.deck.draw(card3)
+        self.board.add(card1)
+        self.board.add(card2)
+        self.board.add(card3)
+
+    def flop(self, card1: (str, Card) = None, card2: (str, Card) = None, card3: (str, Card) = None):
+        """
+        Draw a flop and steps to this new street
+
+        Args:
+            card1 (str, Card): The first card to draw
+            card2 (str, Card): The second card to draw
+            card3 (str, Card): The third card to draw
+        """
         if not (self.next_street_ready and self.street == Street.PREFLOP):
             raise ValueError("The PREFLOP must be ended before we can draw a flop")
-        self.draw_flop(c1=c1, c2=c2, c3=c3)
+        self.draw_flop(card1=card1, card2=card2, card3=card3)
         self.street = "flop"
         self.street_reset()
 
-    def draw_turn(self, card=None):
-        """For the turn, draws a card in the deck and adds it on the board as turn card"""
-        if len(self._board) != 3:
+    def draw_turn(self, card: (str, Card) = None):
+        """
+        For the turn, draws a card in the deck and adds it on the board as turn card
+
+        Args:
+            card (str, Card): The card to draw
+        """
+        if len(self.board) != 3:
             raise ValueError("Board size must be 3 before we can draw a turn")
-        card = self._deck.draw(card)
-        self._board.add(card)
+        card = self.deck.draw(card)
+        self.board.add(card)
+
+    def turn(self, card: (str, Card) = None):
+        """
+        Draw a turn and steps to this new street
 
-    def turn(self, card=None):
-        """Draw a turn and steps to this new street"""
+        Args:
+            card (str, Card): The card to draw
+        """
         if not (self.next_street_ready and self.street == Street.FLOP):
             raise ValueError("The FLOP must be ended before we can draw a turn")
         self.draw_turn(card)
         self.street = "turn"
         self.street_reset()
 
-    def draw_river(self, card=None):
-        """For the river, draws a card in the deck and adds it on the board as river card"""
-        if len(self._board) != 4:
+    def draw_river(self, card: (str, Card) = None):
+        """
+        For the river, draws a card in the deck and adds it on the board as river card
+
+        Args:
+            card (str, Card): The card to draw
+        """
+        if len(self.board) != 4:
             raise ValueError("Board size must be 4 before we can draw a turn")
-        card = self._deck.draw(card)
-        self._board.add(card)
+        card = self.deck.draw(card)
+        self.board.add(card)
+
+    def river(self, card: (str, Card) = None):
+        """
+        Draw a river and steps to this new street
 
-    def river(self, card=None):
-        """Draw a river and steps to this new street"""
+        Args:
+            card (str, Card): The card to draw
+        """
         if not (self.next_street_ready and self.street == Street.TURN):
             raise ValueError("The TURN must be ended before we can draw a river")
         self.draw_river(card)
         self.street = "river"
         self.street_reset()
 
     def advance_to_showdown(self):
         """Advance to showdown"""
         if not (self.next_street_ready and self.street == Street.RIVER):
             raise ValueError("The RIVER must be ended before we can advance to showdown")
         self.street = Street.SHOWDOWN
         self.street_reset()
 
-    def add_tournament(self, tournament):
-        """Associates table with a tournament"""
+    def add_tournament(self, tournament: Tournament):
+        """
+        Associates table with a tournament
+
+        Args:
+            tournament (Tournament): The tournament to associate with the table
+        """
         self.tournament = tournament
-        self._is_mtt = True
+        self.level = tournament.level
+        self.is_mtt = True
 
     def add_player(self, player):
         """
         Add a player to the table
+
+        Args:
+            player (TablePlayer): The player to add
         """
         player.sit(self)
         if self.players.len > 1:
             self.players.distribute_positions()
         else:
             self.players.bb = player.seat
 
     def remove_player(self, player):
         """
         Remove a player from the table
+
+        Args:
+            player (TablePlayer): The player to remove
         """
         player.sit_out()
         if self.players.len > 1:
             self.players.distribute_positions()
 
     def set_hero(self, player):
         """
         Set a player as the hero
+
+        Args:
+            player (TablePlayer): The player to set as the hero
         """
         for p in self.players:
             p.is_hero = False
         player.is_hero = True
 
-    def distribute_hero_cards(self, player_name, c1, c2):
+    def distribute_hero_cards(self, player_name: str, card1: (str, Card), card2: (str, Card)):
         """
         Distribute hero cards
+
+        Args:
+            player_name (str): The name of the player
+            card1 (str, Card): The first card
+            card2 (str, Card): The second card
         """
         player = self.players[player_name]
         self.set_hero(player)
-        player.distribute(f"{c1}{c2}")
+        player.distribute(f"{card1}{card2}")
 
     def set_bb_seat(self, player_seat: int):
         """
         Set the seat of the big blind player and redistribute positions
+
+        Args:
+            player_seat (int): The seat of the big blind player
         """
         self.players.bb = player_seat
         if self.players.len > 1:
             self.players.distribute_positions()
 
     def advance_bb_seat(self):
         """Advances the Big Blind seat"""
         self.players.advance_bb_seat()
 
     def set_max_players(self, max_players: int):
         """
         Set the maximum number of players on the table
+
+        Args:
+            max_players (int): The maximum number of players on the table
         """
         self.max_players = max_players
         if self.players.len > 1:
             self.players.distribute_positions()
 
     def post_antes(self):
         """Preflop Ante posting for players on the table"""
@@ -358,92 +361,72 @@
     def post_pregame(self):
         """Preflop posting antes and blinds"""
         self.post_antes()
         self.post_sb()
         self.post_bb()
 
     @property
-    def seat_playing(self):
-        """Returns the seat of the player currently playing"""
-        if not hasattr(self, "_seat_playing"):
-            self._seat_playing = self.playing_order[0]
-        return self._seat_playing
-
-    @property
-    def cost_per_round(self):
+    def cost_per_round(self) -> float:
         """Returns the cost of a round for a player"""
         return self.level.bb * 1.5 + self.level.ante * self.players.len
 
     @property
-    def min_bet(self):
-        """Returns table current minimum bet a player can make"""
-        if not hasattr(self, "_min_bet"):
-            self._min_bet = self.level.bb*2
-        return self._min_bet
-
-    @min_bet.setter
-    def min_bet(self, value: float):
-        """Setter for min bet property"""
-        if value > self.min_bet:
-            self._min_bet = value
-
-    @property
-    def min_bet_bb(self):
+    def min_bet_bb(self) -> float:
         """Returns the minimum bet in big blinds"""
         return self.min_bet/self.level.bb
 
     @property
-    def pot_value(self):
+    def pot_value(self) -> float:
         """Returns the pot's value"""
         return self.pot.value
 
     @property
-    def pot_value_bb(self):
+    def pot_value_bb(self) -> float:
         """Returns the pot's value in big blinds"""
         return round(self.pot_value/self.level.bb, 2)
 
     @property
-    def average_stack(self):
+    def average_stack(self) -> float:
         """Returns the average stack of players on the table"""
         return sum(pl.init_stack for pl in self.players) / self.players.len
 
     @property
-    def average_stack_bb(self):
+    def average_stack_bb(self) -> float:
         """Returns the average stack in big blinds"""
         return round(self.average_stack/self.level.bb, 2)
 
     @property
-    def estimated_players_remaining(self):
+    def estimated_players_remaining(self) -> int:
         """Returns the estimated number of players remaining in the tournament"""
         return self.tournament.estimated_players_remaining(average_stack=self.average_stack)
 
     def advance_seat_playing(self):
         """Advances seat playing to next available player"""
-        self._seat_playing = self.next_seat
+        self.seat_playing = self.next_seat
         if not self.current_player.can_play and self.nb_waiting > 0:
             self.advance_seat_playing()
 
     @property
     def next_player(self):
         """ Returns the next player after the current player"""
         current_player_index = self.players_order.index(self.current_player)
         next_index = current_player_index + 1 if current_player_index < len(self.players_order) - 1 else 0
         return self.players_order[next_index]
 
     @property
-    def next_seat(self):
+    def next_seat(self) -> int:
         """ Returns the next seat to play after the current player"""
         return self.next_player.seat
 
     def street_reset(self):
         """Reset status of players in game and betting status for a new street"""
         self.pot.highest_bet = 0
         self.cnt_bets = 0
-        self._min_bet = self.level.bb
-        self._seat_playing = self.players_in_game[0].seat
+        self.min_bet = self.level.bb
+        self.seat_playing = self.players_in_game[0].seat
         for player in self.players_in_game:
             player.reset_street_status()
 
     @property
     def current_player(self):
         """Returns the player currently playing"""
         return self.players[self.seat_playing]
@@ -475,16 +458,21 @@
             pl_score = player.hand_score
             if not winners.get(pl_score):
                 winners[pl_score] = [player]
             else:
                 winners[pl_score].append(player)
         return winners
 
-    def split_pot(self, players):
-        """Split pot between players"""
+    def split_pot(self, players: list):
+        """
+        Split pot between players
+
+        Args:
+            players (list): The list of players to split the pot between
+        """
         while len(players) > 0 and self.pot.value > 0:
             min_reward = min([pl.max_reward for pl in players])
             reward = min(min_reward, self.pot.value/len(players))
             for player in players:
                 player.reward += reward
                 if player.reward >= player.max_reward:
                     players.remove(player)
@@ -494,42 +482,20 @@
         """Distribute rewards between players"""
         scores = [score for score in self.winners.keys()]
         scores.sort()
         for score in scores:
             players = self.winners[score]
             self.split_pot(players)
 
-    @property
-    def cnt_bets(self) -> int:
-        """Returns the number of bets made on the table"""
-        return self._cnt_bets
-
-    @cnt_bets.setter
-    def cnt_bets(self, value):
-        """Setter for cnt bets property"""
-        self._cnt_bets = value
-
-    @property
-    def preflop_bet_factors(self) -> list:
-        """Returns the preflop bet factors"""
-        return self._preflop_bet_factors
-
-    @property
-    def postflop_bet_factors(self) -> list:
-        """Returns the postflop bet factors"""
-        return self._postflop_bet_factors
-
     def hand_reset(self):
-        """
-        Reset the hand
-        """
+        """Reset the table for a new hand"""
         self.street = Street.PREFLOP
         self.pot.reset()
         self.deck.reset()
         self.board.reset()
         self.players.hand_reset()
-        self._hand_has_started = False
+        self.hand_has_started = False
 
     def advance_to_next_hand(self):
         """Advance to the next hand"""
         self.hand_reset()
         self.players.advance_bb_seat()
```

### Comparing `pkrcomponents-2.0.0/pkrcomponents/table_player.py` & `pkrcomponents-2.0.1/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents/tournament.py` & `pkrcomponents-2.0.1/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-2.0.0/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-2.0.1/pkrcomponents.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 pkrcomponents/players.py
 pkrcomponents/pot.py
 pkrcomponents/table.py
 pkrcomponents/table_player.py
 pkrcomponents/tournament.py
 pkrcomponents/utils/__init__.py
 pkrcomponents/utils/converters.py
-pkrcomponents/utils/validators.py
+pkrcomponents/utils/validators.py
+site/requirements.txt
```

### Comparing `pkrcomponents-2.0.0/setup.py` & `pkrcomponents-2.0.1/setup.py`

 * *Files identical despite different names*

