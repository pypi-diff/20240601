# Comparing `tmp/plyball-2.3.3.tar.gz` & `tmp/plyball-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.3.3.tar", max compression
+gzip compressed data, was "plyball-2.3.4.tar", max compression
```

## Comparing `plyball-2.3.3.tar` & `plyball-2.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2024-05-29 12:58:14.215675 plyball-2.3.3/LICENSE.txt
--rw-r--r--   0        0        0      819 2024-05-29 12:58:14.215675 plyball-2.3.3/README.md
--rw-r--r--   0        0        0       22 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/__init__.py
--rw-r--r--   0        0        0       48 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/baseballreference/__init__.py
--rw-r--r--   0        0        0     9626 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/baseballreference/baseballreference.py
--rw-r--r--   0        0        0       33 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/fangraphs/__init__.py
--rw-r--r--   0        0        0    15578 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/fangraphs/fangraphs.py
--rw-r--r--   0        0        0       26 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/lahman/__init__.py
--rw-r--r--   0        0        0    10203 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/lahman/lahman.py
--rw-r--r--   0        0        0     6098 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/mlb/__init__.py
--rw-r--r--   0        0        0       28 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/ottoneu/__init__.py
--rw-r--r--   0        0        0    13950 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/ottoneu/ottoneu.py
--rw-r--r--   0        0        0        0 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/pipeline/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/pipeline/evaluation.py
--rw-r--r--   0        0        0     3517 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/player_id_lookup.py
--rw-r--r--   0        0        0      268 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/player_map.py
--rw-r--r--   0        0        0       35 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/retrosheet/__init__.py
--rw-r--r--   0        0        0     8085 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/retrosheet/retrosheet.py
--rw-r--r--   0        0        0       30 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/statcast/__init__.py
--rw-r--r--   0        0        0    14792 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/statcast/statcast.py
--rw-r--r--   0        0        0     4433 2024-05-29 12:58:14.215675 plyball-2.3.3/plyball/utils.py
--rw-r--r--   0        0        0     3098 2024-05-29 12:58:26.615672 plyball-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 plyball-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-06-01 19:11:35.622928 plyball-2.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      819 2024-06-01 19:11:35.622928 plyball-2.3.4/README.md
+-rw-r--r--   0        0        0       22 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/__init__.py
+-rw-r--r--   0        0        0       48 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/baseballreference/__init__.py
+-rw-r--r--   0        0        0     9626 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/baseballreference/baseballreference.py
+-rw-r--r--   0        0        0       33 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/fangraphs/__init__.py
+-rw-r--r--   0        0        0    15581 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/fangraphs/fangraphs.py
+-rw-r--r--   0        0        0       26 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/lahman/__init__.py
+-rw-r--r--   0        0        0    10203 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/lahman/lahman.py
+-rw-r--r--   0        0        0     6346 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/mlb/__init__.py
+-rw-r--r--   0        0        0       28 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/ottoneu/__init__.py
+-rw-r--r--   0        0        0    13956 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/ottoneu/ottoneu.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/pipeline/__init__.py
+-rw-r--r--   0        0        0     3019 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/pipeline/evaluation.py
+-rw-r--r--   0        0        0     3517 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/player_id_lookup.py
+-rw-r--r--   0        0        0      268 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/player_map.py
+-rw-r--r--   0        0        0       35 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/retrosheet/__init__.py
+-rw-r--r--   0        0        0     8085 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/retrosheet/retrosheet.py
+-rw-r--r--   0        0        0       30 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/statcast/__init__.py
+-rw-r--r--   0        0        0    14792 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/statcast/statcast.py
+-rw-r--r--   0        0        0     4433 2024-06-01 19:11:35.622928 plyball-2.3.4/plyball/utils.py
+-rw-r--r--   0        0        0     3098 2024-06-01 19:11:46.283033 plyball-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 plyball-2.3.4/PKG-INFO
```

### Comparing `plyball-2.3.3/LICENSE.txt` & `plyball-2.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/README.md` & `plyball-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/baseballreference/baseballreference.py` & `plyball-2.3.4/plyball/baseballreference/baseballreference.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/fangraphs/fangraphs.py` & `plyball-2.3.4/plyball/fangraphs/fangraphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             'players': kwargs.get('players', '0'),
             'page': '1_999999999',
             'pageitems': '2000000000'
         }
 
         s = requests.get(
             self._urls['leaders'].format('&'.join(['{}={}'.format(k, v) for k, v in parameters.items()]))).json()
-        self.logger.info(self._urls['leaders'].format('&'.join(['{}={}'.format(k, v) for k, v in parameters.items()])))
+        self.logger.debug(self._urls['leaders'].format('&'.join(['{}={}'.format(k, v) for k, v in parameters.items()])))
         return s
 
     def __get_leader_table(self,
                            player_type: Literal['pit', 'bat'],
                            start_season: int,
                            **kwargs) -> pd.DataFrame:
 
@@ -314,15 +314,15 @@
 
         # ?pos = all & level = 0 & lg = all & stats = pit & qual = 0 & type = 0 & team = & season = 2023 & seasonEnd = 2023 & org = & ind = 0 & splitTeam = false & players = & sort = 25, 1
 
         json = requests.get(
             url=self._urls['milb_stats'].format(
                 '&'.join(['{}={}'.format(k, v) for k, v in parameters.items()]))).json()
 
-        self.logger.info("JSON", json=json)
+        self.logger.debug("JSON", json=json)
         df = pd.DataFrame(json)
         # df['Name'] = df.Name.apply(lambda x: BeautifulSoup(x, 'lxml').a.contents[0])
 
         return df
 
     def get_zip_bat_projections(self) -> pd.DataFrame:
         parameters = {
@@ -379,14 +379,14 @@
             'start': start_date,
             'end': end_date
         }
 
         url = 'https://www.fangraphs.com/api/players/game-log?{}'.format(
             '&'.join(['{}={}'.format(k, v) for k, v in parameters.items() if v != '' and v is not None]))
 
-        logging.info(url)
+        logging.debug(url)
 
         json = requests.get(url).json()
 
         df = pd.DataFrame(json['mlb'])
 
         return df
```

### Comparing `plyball-2.3.3/plyball/lahman/lahman.py` & `plyball-2.3.4/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/mlb/__init__.py` & `plyball-2.3.4/plyball/mlb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import datetime as dt
 import logging
 from typing import List, Dict
 
 import pandas as pd
-
 import requests
 
 base_url = 'https://statsapi.mlb.com/api/v1/'
 
 urls = {
     'schedule_by_day': base_url + "schedule/games/?sportId=1&date={run_date}",
     'line_ups': base_url + 'schedule?gamePk={game_pk}&language=en&hydrate=lineups,probablePitcher(note)',
     'game': base_url + "game/{game_pk}/boxscore?timecode={run_date}",
     'schedule': base_url + "schedule/?eventTypes=primary,secondary&sportId=1&startDate={start_date}&endDate={end_date}"
 }
 
+# TIMECODE_FORMAT = YYYYMMDD_HHMMSS
+TIMECODE_FORMAT = "%Y%m%d_%H%M%S"
+
 headers = {
         "Content-Type": "application/json"
 }
 
 logger = logging.getLogger(__name__)
 
 
@@ -54,15 +56,14 @@
                 game = data["dates"][0]["games"][0]
 
                 # Get the projected lineups
                 for team in ['home', 'away']:
                     try:
                         lineup = game["lineups"][f"{team}Players"]
                     except KeyError:
-                        print(game)
                         logger.info(f"No projected lineup for {team} team")
                         logger.info(game)
                         continue
                     for i, player_info in enumerate(lineup):
                         player = {
                                 "date":          game["gameDate"],
                                 "player_id":     player_info["id"],
@@ -112,25 +113,31 @@
             data = response.json()
 
             # Check if the game data is available
             for date in data["dates"]:
                 for game in date["games"]:
                     return self.get_game_lineups(game["gamePk"])
 
-    def get_game_boxscore(self, game_pk) -> pd.DataFrame:
+    def get_game_boxscore(self, game_pk: str, run_date: dt.datetime) -> pd.DataFrame:
         """
         Get Game Logs
 
         :param game_pk:
         :return:
         """
-        self.logger.info('Getting Game Logs|{}'.format(urls['game'].format(run_date=game_pk)))
+        self.logger.info(
+            'Getting Game Logs|{}'.format(
+                urls['game'].format(game_pk=game_pk,
+                                    run_date=run_date.strftime("%Y-%m-%d"))))
 
         # Send a GET request to the API endpoint
-        response = requests.get(urls['game'].format(run_date=game_pk), headers=headers)
+        response = requests.get(urls['game'].format(
+            game_pk=game_pk,
+            run_date=run_date.strftime(TIMECODE_FORMAT)),
+            headers=headers)
 
         # Check if the request was successful
         if response.status_code == 200:
             # Get the JSON response
             data = response.json()
 
             # Check if the game data is available
```

### Comparing `plyball-2.3.3/plyball/ottoneu/ottoneu.py` & `plyball-2.3.4/plyball/ottoneu/ottoneu.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 class Ottoneu(object):
     """
     A class for scrapping data from an Ottoneu pipeline league.
 
     """
     logger = structlog.get_logger("Ottoneu")
 
+
+
+
     def __init__(self, league_id: int):
         """
         Initialize Ottoneu with the ID of the League you are a part of.
 
         :param league_id:
         :type league_id: int
         """
@@ -97,15 +100,15 @@
                         data = data + '{}%5B{}%5D%5B%5D={}'.format(wrapper, param, selection)
                         data = data + '&'
                 else:
                     data = data + '{}%5B{}%5D={}'.format(wrapper, param, value)
                 data = data + '&'
 
         self.logger.info("{}/ajax/search".format(self.ottoneu_base_url))
-        self.logger.info(data[:-1])
+        self.logger.debug(data[:-1])
 
         a = requests.post("{}/ajax/search".format(self.ottoneu_base_url),
                           data=data,
                           headers=headers)
 
         _json = a.json()
         self.logger.info(f'JSON: {_json}')
@@ -215,22 +218,22 @@
                         data = data + '{}%5B{}%5D%5B%5D={}'.format(wrapper, param, selection)
                         data = data + '&'
                 else:
                     data = data + '{}%5B{}%5D={}'.format(wrapper, param, value)
                 data = data + '&'
 
         self.logger.info("{}/ajax/search".format(self.ottoneu_base_url))
-        self.logger.info(data[:-1])
+        self.logger.debug(data[:-1])
 
         a = requests.post("{}/ajax/search".format(self.ottoneu_base_url),
                           data=data,
                           headers=headers)
 
         _json = a.json()
-        self.logger.info(f'JSON: {_json}')
+        self.logger.debug(f'JSON: {_json}')
         batter_info = []
         batter_stats = []
         for batter in _json['batterResults']:
             batter_info.append({k: v for k, v in batter.items() if k != 'Stats'})
             try:
                 __stat_dict = {k: v for k, v in batter['Stats']['batting'].items()}
             except KeyError as e:
```

### Comparing `plyball-2.3.3/plyball/pipeline/evaluation.py` & `plyball-2.3.4/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/player_id_lookup.py` & `plyball-2.3.4/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/retrosheet/retrosheet.py` & `plyball-2.3.4/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/statcast/statcast.py` & `plyball-2.3.4/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/plyball/utils.py` & `plyball-2.3.4/plyball/utils.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.3/pyproject.toml` & `plyball-2.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plyball"
-version = "2.3.3"
+version = "2.3.4"
 description = ""
 authors = ["W. Aaron Morris <waaronmorris@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 alabaster = "0.7.13"
@@ -29,21 +29,14 @@
 python-dateutil = "2.8.2"
 readme-renderer = "37.3"
 requests = "2.31.0"
 requests-toolbelt = "0.10.1"
 six = "1.16.0"
 snowballstemmer = "2.2.0"
 soupsieve = "2.4.1"
-sphinx = ">=6.1.3"
-sphinxcontrib-applehelp = ">=1.0.4"
-sphinxcontrib-devhelp = ">=1.0.2"
-sphinxcontrib-htmlhelp = ">=2.0.1"
-sphinxcontrib-jsmath = ">=1.0.1"
-sphinxcontrib-qthelp = ">=1.0.2"
-sphinxcontrib-serializinghtml = ">=1.1.3"
 structlog = "^24.1.0"
 tqdm = "4.42.1"
 urllib3 = "1.26.5"
 webencodings = "0.5.1"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^9.7.3"
@@ -52,14 +45,21 @@
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.6.1"
 pytest-xdist = "^3.4.0"
 flake8 = "^7.0.0"
 black = "^22.1.0"
 isort = "^5.10.1"
 twine = "3.1.1"
+sphinx = ">=6.1.3"
+sphinxcontrib-applehelp = ">=1.0.4"
+sphinxcontrib-devhelp = ">=1.0.2"
+sphinxcontrib-htmlhelp = ">=2.0.1"
+sphinxcontrib-jsmath = ">=1.0.1"
+sphinxcontrib-qthelp = ">=1.0.2"
+sphinxcontrib-serializinghtml = ">=1.1.3"
 
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.26.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `plyball-2.3.3/PKG-INFO` & `plyball-2.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.3.3
+Version: 2.3.4
 Summary: 
 Author: W. Aaron Morris
 Author-email: waaronmorris@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -30,21 +30,14 @@
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: readme-renderer (==37.3)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: requests-toolbelt (==0.10.1)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: snowballstemmer (==2.2.0)
 Requires-Dist: soupsieve (==2.4.1)
-Requires-Dist: sphinx (>=6.1.3)
-Requires-Dist: sphinxcontrib-applehelp (>=1.0.4)
-Requires-Dist: sphinxcontrib-devhelp (>=1.0.2)
-Requires-Dist: sphinxcontrib-htmlhelp (>=2.0.1)
-Requires-Dist: sphinxcontrib-jsmath (>=1.0.1)
-Requires-Dist: sphinxcontrib-qthelp (>=1.0.2)
-Requires-Dist: sphinxcontrib-serializinghtml (>=1.1.3)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tqdm (==4.42.1)
 Requires-Dist: urllib3 (==1.26.5)
 Requires-Dist: webencodings (==0.5.1)
 Description-Content-Type: text/markdown
 
 # Overview
```

