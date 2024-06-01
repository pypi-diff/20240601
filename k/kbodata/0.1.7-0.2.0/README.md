# Comparing `tmp/kbodata-0.1.7.tar.gz` & `tmp/kbodata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbodata-0.1.7.tar", max compression
+gzip compressed data, was "kbodata-0.2.0.tar", max compression
```

## Comparing `kbodata-0.1.7.tar` & `kbodata-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1061 2022-01-24 07:41:16.234182 kbodata-0.1.7/LICENSE
--rw-r--r--   0        0        0     4840 2022-02-13 10:53:11.572029 kbodata-0.1.7/README.md
--rw-r--r--   0        0        0      403 2022-07-25 14:16:51.321405 kbodata-0.1.7/kbodata/__init__.py
--rw-r--r--   0        0        0        0 2022-01-24 07:41:16.234832 kbodata-0.1.7/kbodata/get/__init__.py
--rw-r--r--   0        0        0     1485 2022-02-11 00:32:12.000000 kbodata-0.1.7/kbodata/get/game.py
--rw-r--r--   0        0        0     3643 2022-04-12 04:26:52.926890 kbodata-0.1.7/kbodata/get/schedule.py
--rw-r--r--   0        0        0        0 2022-01-24 07:41:16.236405 kbodata-0.1.7/kbodata/load/__init__.py
--rw-r--r--   0        0        0      471 2022-01-30 15:36:57.951507 kbodata-0.1.7/kbodata/load/batter.py
--rw-r--r--   0        0        0      477 2022-01-30 15:36:57.953361 kbodata-0.1.7/kbodata/load/pitcher.py
--rw-r--r--   0        0        0      468 2022-01-30 15:36:57.953417 kbodata-0.1.7/kbodata/load/scoreboard.py
--rw-r--r--   0        0        0        0 2022-01-24 07:41:16.236622 kbodata-0.1.7/kbodata/parser/__init__.py
--rw-r--r--   0        0        0     5140 2022-02-20 12:49:54.569207 kbodata-0.1.7/kbodata/parser/batter.py
--rw-r--r--   0        0        0     3297 2022-02-20 12:43:10.797810 kbodata-0.1.7/kbodata/parser/config.ini
--rw-r--r--   0        0        0     3943 2022-02-19 09:10:02.666405 kbodata-0.1.7/kbodata/parser/html.py
--rw-r--r--   0        0        0     4474 2022-01-29 18:06:53.136100 kbodata-0.1.7/kbodata/parser/page.py
--rw-r--r--   0        0        0     3202 2022-02-11 02:33:06.000000 kbodata-0.1.7/kbodata/parser/pitcher.py
--rw-r--r--   0        0        0     6792 2022-07-25 14:16:39.648269 kbodata-0.1.7/kbodata/parser/schedule.py
--rw-r--r--   0        0        0     3099 2022-04-12 04:54:47.983046 kbodata-0.1.7/kbodata/parser/scoreboard.py
--rw-r--r--   0        0        0     3955 2022-01-29 18:24:04.802402 kbodata-0.1.7/kbodata/parser/util.py
--rw-r--r--   0        0        0      633 2022-07-25 14:02:23.961845 kbodata-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5818 2022-07-25 14:18:11.761284 kbodata-0.1.7/setup.py
--rw-r--r--   0        0        0     5770 2022-07-25 14:18:11.761743 kbodata-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-18 07:58:30.374186 kbodata-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4840 2024-05-18 07:58:30.374579 kbodata-0.2.0/README.md
+-rw-r--r--   0        0        0      403 2024-06-01 15:52:10.063406 kbodata-0.2.0/kbodata/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 07:58:30.378080 kbodata-0.2.0/kbodata/get/__init__.py
+-rw-r--r--   0        0        0     2439 2024-06-01 14:19:05.099611 kbodata-0.2.0/kbodata/get/game.py
+-rw-r--r--   0        0        0     3397 2024-06-01 07:45:00.507019 kbodata-0.2.0/kbodata/get/schedule.py
+-rw-r--r--   0        0        0        0 2024-05-18 07:58:30.378845 kbodata-0.2.0/kbodata/load/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-18 07:58:30.379079 kbodata-0.2.0/kbodata/load/batter.py
+-rw-r--r--   0        0        0      477 2024-05-18 07:58:30.379292 kbodata-0.2.0/kbodata/load/pitcher.py
+-rw-r--r--   0        0        0      468 2024-05-18 07:58:30.379565 kbodata-0.2.0/kbodata/load/scoreboard.py
+-rw-r--r--   0        0        0        0 2024-05-18 07:58:30.380014 kbodata-0.2.0/kbodata/parser/__init__.py
+-rw-r--r--   0        0        0     5135 2024-06-01 15:36:40.116201 kbodata-0.2.0/kbodata/parser/batter.py
+-rw-r--r--   0        0        0     3340 2024-06-01 15:35:05.166075 kbodata-0.2.0/kbodata/parser/config.ini
+-rw-r--r--   0        0        0     4007 2024-06-01 14:00:26.864625 kbodata-0.2.0/kbodata/parser/html.py
+-rw-r--r--   0        0        0     5122 2024-06-01 14:07:23.408481 kbodata-0.2.0/kbodata/parser/page.py
+-rw-r--r--   0        0        0     3195 2024-06-01 14:54:54.595870 kbodata-0.2.0/kbodata/parser/pitcher.py
+-rw-r--r--   0        0        0     7894 2024-06-01 07:36:01.877313 kbodata-0.2.0/kbodata/parser/schedule.py
+-rw-r--r--   0        0        0     3099 2024-05-18 07:58:30.382451 kbodata-0.2.0/kbodata/parser/scoreboard.py
+-rw-r--r--   0        0        0     3955 2024-05-18 07:58:30.382819 kbodata-0.2.0/kbodata/parser/util.py
+-rw-r--r--   0        0        0      632 2024-06-01 15:55:58.555919 kbodata-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5821 1970-01-01 00:00:00.000000 kbodata-0.2.0/PKG-INFO
```

### Comparing `kbodata-0.1.7/LICENSE` & `kbodata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kbodata-0.1.7/README.md` & `kbodata-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kbodata-0.1.7/kbodata/get/game.py` & `kbodata-0.2.0/kbodata/get/game.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 """KBO 정규 시즌 게임 자료를 가져와서 사용할 수 있도록 가공하기 쉽게 수정해주는 모듈 
 """
+from datetime import date
 from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
 from kbodata.parser.batter import batter_modify
 from tqdm import tqdm
-from kbodata.parser.page import parsing_single_game
+from kbodata.parser.page import parsing_single_game, is_game_finished
 from kbodata.parser.scoreboard import scoreboard_modify
 from kbodata.parser.batter import batter_modify
 from kbodata.parser.pitcher import pitcher_modify
+ 
+def get_single_game_data(date, gameId, driver):
+    """단일 경기 데이터를 크롤링하고 사용할 데이터로 전처리 해주는 함수
+    """
+    raw_data = parsing_single_game(date, gameId, driver)
+    scoreboard_modify(raw_data)
+    batter_modify(raw_data)
+    pitcher_modify(raw_data)
+    return raw_data
 
 def get_game_data(schedule, Driver_path):
     """스케쥴에 해당하는 데이터를 가져오는 함수
     데이터들을 스크래핑하여 list로 반환한다.
     """
     data = []
     options = webdriver.ChromeOptions()
     options.add_argument("headless")
     options.add_argument("window-size=1920x1080")
     options.add_argument("disable-gpu")
     options.add_argument("--log-level=2")
-    # 혹은 options.add_argument("--disable-gpu")
-    driver = webdriver.Chrome(Driver_path, options=options)
+    driver = webdriver.Chrome(service=Service(executable_path=Driver_path) , options=options)
     driver.implicitly_wait(100)
 
+    today = date.today().strftime("%Y%m%d")
+    today_result = is_game_finished(today, driver)
+
     with tqdm(desc="in progress",total=len(schedule)) as pbar:
         for idx, row in schedule.iterrows():
-            if row["status"] == 'canceled':
+            # 취소된 경기나 미래 날짜의 경기는 제외
+            if (row["status"] == 'canceled') or (row["status"]== 'scheduled'):
                 pbar.update(1)
+            # 오늘자 경기의 경우 종료되었는지 확인하고 크롤링
+            elif row["status"] == 'ongoing':
+                if today_result[row["gameid"]] == 1:
+                    result = get_single_game_data(row["date"],row["gameid"],driver)
+                    data.append(result)
+                    pbar.update(1)
+                else:
+                    pbar.update(1)
+                    continue
+            # 끝난 경기라면 바로 크롤링
             else:
-                raw_data = parsing_single_game(row["date"],row["gameid"],driver)
-                scoreboard_modify(raw_data)
-                batter_modify(raw_data)
-                pitcher_modify(raw_data)
-                data.append(raw_data)
+                result = get_single_game_data(row["date"],row["gameid"],driver)
+                data.append(result)
                 pbar.update(1)
     driver.quit()
     return data
+
```

### Comparing `kbodata-0.1.7/kbodata/get/schedule.py` & `kbodata-0.2.0/kbodata/get/schedule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from datetime import date
 from tqdm import tqdm
 from dateutil.relativedelta import relativedelta
 from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
 import pandas as pd
 from kbodata.parser.schedule import parsing_daily_schedule, parsing_monthly_schedule
 
 def get_daily_schedule(year,month,day,Driver_path):
     """유저 함수: 2008년 이후 데이터 중에 요청된 날짜의 경기 스케쥴을 가져온다.
 
-    ex) get_daily_schedule("20210420","chromedriver")
+    ex) get_daily_schedule(2021,04,20,"chromedriver")
 
         status      date home away  dbheader gameid
     0	finished	20210420	HT	LG	0	HTLG0
     1	finished	20210420	KT	NC	0	KTNC0
     2	finished	20210420	OB	LT	0	OBLT0
     3	finished	20210420	SK	SS	0	SKSS0
     4	finished	20210420	WO	HH	0	WOHH0
@@ -23,40 +24,37 @@
 
     sd_date = date(year, month, day)
     options = webdriver.ChromeOptions()
     options.add_argument("headless")
     options.add_argument("window-size=1920x1080")
     options.add_argument("disable-gpu")
     options.add_argument("--log-level=2")
-    driver = webdriver.Chrome(Driver_path, options=options)
+    driver = webdriver.Chrome(service=Service(executable_path=Driver_path) , options=options)
     driver.implicitly_wait(100)
 
     if sd_date.year < 2008: return print("ERROR: This library only provides data since 2008.")
-    if sd_date > date.today(): return print("ERROR: The end date is later than now.")
-    if sd_date == date.today(): return print("ERROR: Today's game info is not updated yet.")
     
     data = parsing_daily_schedule(year,month,day,driver)
     driver.quit()
     return data
 
 def get_monthly_schedule(year, month, Driver_path):
     """유저 함수: 2008년부터 달 단위로 요청된 경기 스케쥴을 가져온다.
     """
     if (str(year)+str(month)).isdigit() == False:
         return print("ERROR: INVALID PARAMETER. please check year or month")
     st_date = date(year,month,1)
     
     if st_date.year < 2008: return print("ERROR: This library only provides data since 2008.")
-    if st_date > date.today(): return print("ERROR: The date is later than now.")
 
     options = webdriver.ChromeOptions()
     options.add_argument("headless")
     options.add_argument("window-size=1920x1080")
     options.add_argument("disable-gpu")
-    driver = webdriver.Chrome(Driver_path, options=options)
+    driver = webdriver.Chrome(service=Service(executable_path=Driver_path) , options=options)
     driver.implicitly_wait(100)
 
     data = parsing_monthly_schedule(st_date.year,st_date.month,driver)
     driver.quit()
 
     return data
 
@@ -66,22 +64,20 @@
     if len(str(year)) != 4 or (str(year)).isdigit() == False:
         return print("ERROR: INVALID PARAMETER. please check year")
     schedule = pd.DataFrame()
     st_date = date(year,1,1)
     ed_date = date(year,12,30)
     
     if st_date.year < 2008: return print("ERROR: This library only provides data since 2008.")
-    if ed_date.year > date.today().year : return print("ERROR: The end date is later than now.")
     
-    delta = relativedelta(ed_date, st_date)
     options = webdriver.ChromeOptions()
     options.add_argument("headless")
     options.add_argument("window-size=1920x1080")
     options.add_argument("disable-gpu")
-    driver = webdriver.Chrome(Driver_path, options=options)
+    driver = webdriver.Chrome(service=Service(executable_path=Driver_path) , options=options)
     driver.implicitly_wait(100)
 
     with tqdm(desc="in progress",total=12) as pbar:
         while st_date < ed_date:
             data = parsing_monthly_schedule(st_date.year,st_date.month,driver)
             schedule = pd.concat([schedule,data],axis=0,ignore_index=True)
             st_date += relativedelta(months=1)
```

### Comparing `kbodata-0.1.7/kbodata/parser/batter.py` & `kbodata-0.2.0/kbodata/parser/batter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ast
+import json
 import os
 import re
 import configparser
 import pandas as pd
 from kbodata.parser.util import make_primary_key, get_game_info
 
 # 설정파일을 읽어오기 위해 configparser를 사용
@@ -50,15 +50,15 @@
             new_info["hit"] = batter["안타"]
             new_info["bat_num"] = batter["타수"]
             new_info["hit_get"] = batter["타점"]
             new_info["own_get"] = batter["득점"]
             fin_batters.append(new_info)
 
         fin_batters = pd.DataFrame(fin_batters)
-        data["contents"][home_or_away] = ast.literal_eval(
+        data["contents"][home_or_away] = json.loads(
             fin_batters.to_json(orient="records")
         )
     i = i + 1
 
     return data
```

### Comparing `kbodata-0.1.7/kbodata/parser/config.ini` & `kbodata-0.2.0/kbodata/parser/config.ini`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 12안: 1000
 1안: 1001
 1우안: 1002
 1중안: 1003
 2안: 1004
 2우안: 1005
 2유안: 1006
+유2안: 1006
 2좌안: 1007
 2중안: 1008
 3안: 1009
 3유안: 1010
 유3안: 1010
 3좌안: 1011
 3중안: 1012
@@ -113,14 +114,15 @@
 삼진: 2000
 스낫: 2100
 1번: 4000
 1희번: 4100
 2번: 4001
 2희번: 4101
 3번: 4002
+삼번: 4002
 3희번: 4102
 유번: 4003
 유희번: 4103
 투번: 4004
 투희번: 4104
 포번: 4005
 포희번: 4105
@@ -143,14 +145,15 @@
 좌희실: 6104
 중실: 6006
 중희실: 6105
 투실: 6007
 투희실: 6106
 포실: 6008
 포희실: 6107
+유희실: 6108
 1희선: 6200
 3희선: 6201
 투희선: 6202
 포희선: 6203
 삼선: 6204
 타방: 6400
 1비: 7000
```

### Comparing `kbodata-0.1.7/kbodata/parser/html.py` & `kbodata-0.2.0/kbodata/parser/html.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-
+from io import StringIO
 
 def looking_for_team_names(temp_teams):
     """ 모은 HTML soup에서 시합한 두 팀명을 뽑는 함수
     다음과 같은 HTML soup에서 "한화"만 뽑아서 팀명을 찾는다.
     실제로는 아래와 같은 것이 두 팀에서 각 각 타자, 투수 총 네 번 나온다.
     거기서 두 팀만 뽑으면 된다. 또한 아래처럼 "한화 이글스 타자 기록"에서 첫 번째 단어만 뽑으면 된다.
     <h6 class="tit-team" id="lblAwayHitter">
@@ -29,25 +29,31 @@
         else:
             team_name = temp_team[0]
         if team_name not in temp_team_list:
             temp_team_list.append(team_name)
 
     return (temp_team_list[0], temp_team_list[1])
 
+def _read_html(table):
+    html_data = StringIO(table)
+    return pd.read_html(html_data)[0]
+
+
 def scoreboard(tables, teams):
-    temp_df_0 = pd.read_html(str(tables[0]))[0]
+    temp_df_0 = _read_html(str(tables[0]))
     temp_df_0 = temp_df_0.rename(columns={"Unnamed: 0": "승패"})
-    temp_df_1 = pd.read_html(str(tables[1]))[0]
-    temp_df_2 = pd.read_html(str(tables[2]))[0]
+    temp_df_1 = _read_html(str(tables[1]))
+    temp_df_2 = _read_html(str(tables[2]))
     temp_teams_df = pd.DataFrame({"팀": teams})
     temp_total = pd.concat(
         [temp_teams_df, temp_df_0["승패"], temp_df_1, temp_df_2], axis=1
     )
     return temp_total
 
+
 def etc_info(tables, record_etc):
     record = {}
     header_list = tables[3].find_all("th")
     if len(header_list) != 0:
         header = [h.get_text(strip=True) for h in header_list]
         data = tables[3].find_all("td")
         etc_data = [d.get_text(strip=True) for d in data]
@@ -72,42 +78,42 @@
     }
     # etc={i.split(" : ")[0]:i.split(" : ")[1] for i in record_etc[0].get_text().split("\n") if len(i)!=0 }
     record.update(etc)
     return record
 
 
 def away_batter(tables, team):
-    temp1 = pd.read_html(str(tables[4]))[0].dropna()
+    temp1 = _read_html(str(tables[4])).dropna()
     temp1 = temp1.rename(columns={"Unnamed: 1": "포지션"})
     del temp1["Unnamed: 0"]
-    temp2 = pd.read_html(str(tables[5]))[0][:-1]
-    temp3 = pd.read_html(str(tables[6]))[0][:-1]
+    temp2 = _read_html(str(tables[5]))[:-1]
+    temp3 = _read_html(str(tables[6]))[:-1]
     away = pd.concat([temp1, temp2, temp3], axis=1)
     away["팀"] = team[0]
     away = away.fillna(0)
     return away
 
 
 def home_batter(tables, team):
-    temp1 = pd.read_html(str(tables[7]))[0].dropna()
+    temp1 = _read_html(str(tables[7])).dropna()
     temp1 = temp1.rename(columns={"Unnamed: 1": "포지션"})
     del temp1["Unnamed: 0"]
-    temp2 = pd.read_html(str(tables[8]))[0][:-1]
-    temp3 = pd.read_html(str(tables[9]))[0][:-1]
+    temp2 = _read_html(str(tables[8]))[:-1]
+    temp3 = _read_html(str(tables[9]))[:-1]
     home = pd.concat([temp1, temp2, temp3], axis=1)
     home["팀"] = team[1]
     home = home.fillna(0)
     return home
 
 
 def away_pitcher(tables, team):
-    away = pd.read_html(str(tables[10]))[0][:-1]
+    away = _read_html(str(tables[10]))[:-1]
     away["팀"] = team[0]
     away = away.fillna(0)
     return away
 
 
 def home_pitcher(tables, team):
-    home = pd.read_html(str(tables[11]))[0][:-1]
+    home = _read_html(str(tables[11]))[:-1]
     home["팀"] = team[1]
     home = home.fillna(0)
     return home
```

### Comparing `kbodata-0.1.7/kbodata/parser/page.py` & `kbodata-0.2.0/kbodata/parser/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,39 @@
-import ast
+import json
 import os
 import configparser
 from bs4 import BeautifulSoup
+import pandas as pd
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
 from kbodata.parser.html import scoreboard, etc_info, looking_for_team_names
 from kbodata.parser.html import away_batter, home_batter, away_pitcher, home_pitcher
 
 # 설정파일을 읽어오기 위해 configparser를 사용
 config = configparser.ConfigParser()
 # 필요한 변수 가져오기
 config.read(os.path.join(os.path.dirname(__file__),"config.ini"), encoding="utf-8")
 url = config["DEFAULT"]["KBO_URL"]
 
+def is_game_finished(gameDate, driver):
+    """오늘 경기가 완료되었는지 확인하는 함수
+    """
+    temp_url = url + gameDate
+    result = {}
+    driver.get(temp_url)
+    game_elements = WebDriverWait(driver, 100).until(EC.presence_of_all_elements_located((By.CLASS_NAME, "game-cont")))
+    for element in game_elements:
+        data = BeautifulSoup(element.get_attribute('outerHTML'), "lxml").find('li', class_='game-cont')
+        game_id = data.get('g_id')[8:]
+        status = data.get('result_ck')
+        result[game_id] = status
+    return result
+
 
 def parsing_page(gameDate, gameId, driver):
     temp_url = url + gameDate + "&amp;gameId=" + gameDate + gameId + "&amp;section=REVIEW"
     driver.get(temp_url)
     data = WebDriverWait(driver, 100).until(EC.visibility_of_element_located((By.ID,"gameCenterContents")))
     soup = BeautifulSoup(data.get_attribute('innerHTML'), "lxml")
     tables = soup.find_all("table")
@@ -53,15 +68,15 @@
     ----------
     :param1: str
         date: "20181010" 와 같이 경기 날짜로 만들어진 문자열
     :param1: str
         gameld: 경기를 하는 팀명과 더블해더 유무를 이용해 만든 문자열
         "WOOB0"과 같이 만드는데, WO, OB는 각각 팀명을 의미하고
         0은 더블헤더 경기가 아닌 것을 알려준다.
-        만약 더불헤더 경기면 1차전은 "KTLT1"처럼 1로 표시하고
+        만약 더블헤더 경기면 1차전은 "KTLT1"처럼 1로 표시하고
         2차전이면 "KTLT2"으로 표시한다.
 
     Returns
     -------
         json
         게임 자료가 들어 있다. "id" 키에는 '20181010_KTLT1' 과 같은
         정규 시즌 단일 게임 아이디가 들어 있다. Parameters를 이용해서 만든다.
@@ -71,54 +86,56 @@
         - 'ETC_info'
         - 'away_batter'
         - 'home_batter'
         - 'away_pitcher'
         - 'home_pitcher'
     """
 
+    pd.set_option('future.no_silent_downcasting', True)
+    
     temp_page = parsing_page(date, gameId, driver)
 
     temp_scoreboard = scoreboard(temp_page["tables"], temp_page["teams"])
 
     temp_all = {
-        "scoreboard": ast.literal_eval(temp_scoreboard.to_json(orient="records"))
+        "scoreboard": json.loads((temp_scoreboard.to_json(orient="records")))
     }
     temp_all.update(
-        {"ETC_info": etc_info(temp_page["tables"], temp_page["record_etc"])}
+        {"ETC_info": json.loads(json.dumps(etc_info(temp_page["tables"], temp_page["record_etc"])))}
     )
     temp_all.update(
         {
-            "away_batter": ast.literal_eval(
+            "away_batter": json.loads(
                 away_batter(temp_page["tables"], temp_page["teams"]).to_json(
                     orient="records"
                 )
             )
         }
     )
     temp_all.update(
         {
-            "home_batter": ast.literal_eval(
+            "home_batter": json.loads(
                 home_batter(temp_page["tables"], temp_page["teams"]).to_json(
                     orient="records"
                 )
             )
         }
     )
     temp_all.update(
         {
-            "away_pitcher": ast.literal_eval(
+            "away_pitcher": json.loads(
                 away_pitcher(temp_page["tables"], temp_page["teams"]).to_json(
                     orient="records"
                 )
             )
         }
     )
     temp_all.update(
         {
-            "home_pitcher": ast.literal_eval(
+            "home_pitcher": json.loads(
                 home_pitcher(temp_page["tables"], temp_page["teams"]).to_json(
                     orient="records"
                 )
             )
         }
     )
```

### Comparing `kbodata-0.1.7/kbodata/parser/pitcher.py` & `kbodata-0.2.0/kbodata/parser/pitcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ast
+import json
 import pandas as pd
 from kbodata.parser.util import make_primary_key, get_game_info
 
 
 def pitcher_modify(data):
     """수집한 여러 개의 경기가 들어 있는 자료에서 투수 자료만 정리하는 함수
 
@@ -40,33 +40,33 @@
             new_info['hitted'] = pitcher['피안타']
             new_info['homerun'] = pitcher['홈런']
             new_info['battednum'] = pitcher['타수']
             new_info['batternum'] = pitcher['타자']
             fin_pitchers.append(new_info)
 
         fin_pitchers= pd.DataFrame(fin_pitchers)
-        data["contents"][home_or_away] = ast.literal_eval(fin_pitchers.to_json(orient="records"))
+        data["contents"][home_or_away] = json.loads(fin_pitchers.to_json(orient="records"))
     i = i + 1
 
     return data
 
 
 def change_inning(data):
     """이닝수와 나머지를 정리해주는 코드. 이닝수와 나머지 값을 순차적으로 나열한다. 이닝수의 경우 0-18까지 가능하며, 나머지의 경우 0-2까지만 가능하다.
 
     ### Examples:
         - '5' -> 50
-        - '2\\/3' -> 02
-    - '1 2\\/3' -> 12
+        - '2/3' -> 02
+        - '1 2/3' -> 12
     """
     temp = str(data).split()
     
-    if len(temp) == 1 and "\\" not in temp[0]:
+    if len(temp) == 1 and "/" not in temp[0]:
         return temp[0]+"0"
-    elif len(temp) == 1 and "\\" in temp[0]:
+    elif len(temp) == 1 and "/" in temp[0]:
         return "0"+temp[-1][0]
     else:
         return temp[0] + temp[-1][0]
 
 def change_result(result):
 
     if result == '세이브':
```

### Comparing `kbodata-0.1.7/kbodata/parser/schedule.py` & `kbodata-0.2.0/kbodata/parser/schedule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import configparser
 import pandas as pd
 from datetime import date
 from bs4 import BeautifulSoup
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
@@ -14,87 +15,107 @@
 config.read(os.path.join(os.path.dirname(__file__),"config.ini"), encoding="utf-8")
 info_url = config["DEFAULT"]["Game_info_URL"]
 
 
 def parsing_monthly_schedule(year, month, driver):
 
     driver.get(info_url)
-    driver.find_element_by_id("ddlYear").send_keys(str(year))
-    driver.find_element_by_id("ddlMonth").send_keys(str(month).zfill(2))
+    driver.find_element("id", "ddlYear").send_keys(str(year))
+    driver.find_element("id", "ddlMonth").send_keys(str(month).zfill(2))
     data = WebDriverWait(driver, 100).until(EC.visibility_of_element_located((By.ID,"tblSchedule")))
     # 스크래핑 된 데이터 정리
     table = BeautifulSoup(data.get_attribute('innerHTML'), "lxml")
     result = []
     not_listed = ["EAST", "WEST", "드림", "나눔"]
     for td in table.find_all("td"):
         # 경기 없는 날 확인
         if len(td) == 1:
             continue
         for li in td.find_all("li"):
-            info = (li.text).split()
+            text = re.sub(r'\[.*?\]', '', li.text)
+            info = (text).split()
             # 경기날짜 확인
             if li.get('class') == ['dayNum']:
-                day = str(year)+str(month).zfill(2) + info[0].zfill(2)
-                # 미래 경기정보는 제외
-                if date(year,month,int(info[0])) >= date.today():
-                    break
+                day = int(info[0].zfill(2))
+                dt = str(year)+str(month).zfill(2) + info[0].zfill(2)
             # 나눔 경기는 제외
             elif info[0] in not_listed:
                 continue
             # 경기 취소 확인
             elif (li.get('class') == ['rainCancel']) or (day == "20111025"):
                 status = "canceled"
                 home = change_name_to_id(info[2],year)
                 away = change_name_to_id(info[0],year)
-                result.append([status,day,home,away])
+                result.append([status,dt,home,away])
+            elif (len(info) < 5) & (date(year,month,day) == date.today()):
+                status = "ongoing"
+                home = change_name_to_id(info[-1],year)
+                away = change_name_to_id(info[0],year)
+                result.append([status,dt,home,away])
+            elif (len(info) < 5) & (date(year,month,day) > date.today()):
+                status = "scheduled"
+                home = change_name_to_id(info[-1],year)
+                away = change_name_to_id(info[0],year)
+                result.append([status,dt,home,away])
             else:
                 status = "finished"
                 home = change_name_to_id(info[-1],year)
                 away = change_name_to_id(info[0],year)
-                result.append([status,day,home,away])
+                result.append([status,dt,home,away])
     result = pd.DataFrame(result, columns=["status","date","home","away"])
     result = add_gameid(result)
     result = delete_non_provided_data(result)
     
     return result
 
 
 def parsing_daily_schedule(year,month,day,driver):
 
     # 스케쥴 데이터 스크래핑
     driver.get(info_url)
-    driver.find_element_by_id("ddlYear").send_keys(str(year))
-    driver.find_element_by_id("ddlMonth").send_keys(str(month).zfill(2))
+    driver.find_element("id", "ddlYear").send_keys(str(year))
+    driver.find_element("id", "ddlMonth").send_keys(str(month).zfill(2))
     data = WebDriverWait(driver, 100).until(EC.visibility_of_element_located((By.ID,"tblSchedule")))
     # 스크래핑 된 데이터 정리
     table= BeautifulSoup(data.get_attribute('innerHTML'), "lxml")
     result = []
     not_listed = ["EAST", "WEST", "드림", "나눔"]
     for td in table.find_all("td"):
         if td.find("li",{"class":"dayNum"}).text != str(day):
             continue
         for li in td.find_all("li"):
-            info = (li.text).split()
+            text = re.sub(r'\[.*?\]', '', li.text)
+            info = (text).split()
             # 경기날짜 확인
             if li.get('class') == ['dayNum']:
-                day = str(year)+str(month).zfill(2) + info[0].zfill(2)
+                dt = str(year)+str(month).zfill(2) + info[0].zfill(2)
             # 나눔 경기는 제외
             elif info[0] in not_listed:
                 continue
             # 경기 취소 확인
             elif li.get('class') == ['rainCancel']:
                 status = "canceled"
                 home = change_name_to_id(info[2],year)
                 away = change_name_to_id(info[0],year)
-                result.append([status,day,home,away])
+                result.append([status,dt,home,away])
+            elif (len(info) < 5) & (date(year,month,day) == date.today()):
+                status = "ongoing"
+                home = change_name_to_id(info[-1],year)
+                away = change_name_to_id(info[0],year)
+                result.append([status,dt,home,away])
+            elif (len(info) < 5) & (date(year,month,day) > date.today()):
+                status = "scheduled"
+                home = change_name_to_id(info[-1],year)
+                away = change_name_to_id(info[0],year)
+                result.append([status,dt,home,away])
             else:
                 status = "finished"
                 home = change_name_to_id(info[-1],year)
                 away = change_name_to_id(info[0],year)
-                result.append([status,day,home,away])
+                result.append([status,dt,home,away])
     result = pd.DataFrame(result, columns=["status","date","home","away"])
     result = add_gameid(result)
     result = delete_non_provided_data(result)
 
     return result
```

### Comparing `kbodata-0.1.7/kbodata/parser/scoreboard.py` & `kbodata-0.2.0/kbodata/parser/scoreboard.py`

 * *Files identical despite different names*

### Comparing `kbodata-0.1.7/kbodata/parser/util.py` & `kbodata-0.2.0/kbodata/parser/util.py`

 * *Files identical despite different names*

### Comparing `kbodata-0.1.7/setup.py` & `kbodata-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,164 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kbodata
+Version: 0.2.0
+Summary: Scraping Korea Baseball Game information
+Home-page: https://github.com/Hyeonji-Ryu/kbo-data
+License: MIT
+Author: Hyeonji-Ryu
+Author-email: dev.bearabbit@gmail.com
+Requires-Python: >=3.9.0,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bs4 (>=0.0.2,<0.0.3)
+Requires-Dist: lxml (>=5.2.2,<6.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: selenium (>=4.21.0,<5.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
+Project-URL: Documentation, https://github.com/Hyeonji-Ryu/kbo-data/tree/main/docs
+Project-URL: Repository, https://github.com/Hyeonji-Ryu/kbo-data
+Description-Content-Type: text/markdown
+
+# What is kbo-data
+
+kbo-data는 한국프로야구 경기정보를 스크래핑하는 파이썬 패키지입니다.  
+kbo-data is a Python package that provides Korean professional baseball game information by scraping.
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kbodata)
+[![PyPI](https://img.shields.io/pypi/v/kbodata)](https://pypi.org/project/kbodata/)
+[![GitHub license](https://img.shields.io/github/license/Hyeonji-Ryu/kbo-data)](https://github.com/Hyeonji-Ryu/kbo-data/blob/main/LICENSE)
+
+## Required
+
+이 패키지를 사용하기 위해서는 chrome driver가 필요합니다. chrome driver는 [해당 페이지](https://chromedriver.chromium.org/downloads)에서 다운로드할 수 있습니다.  
+This package is required chrome driver. You can download it from [this page](https://chromedriver.chromium.org/downloads)
+
+## How to Use
+
+### 패키지 설치하기
+
+먼저 패키지를 설치합니다.  
+you have to install kbodata package first.
+
+```bash
+pip install kbodata
+```
+
+### 데이터 가져오기 (kbodata.get module)
+
+원하는 날짜의 경기 스케쥴을 다운로드 받습니다.  
+you can download KBO match schedule that you want to get.
+
+```python
+    import kbodata
+
+    # 2021년 4월 20일의 KBO 경기 스케쥴을 가져옵니다.
+    # Get the KBO match schedule for April 20, 2021.
+    >>> day = kbodata.get_daily_schedule(2021,4,20,'chromedriver_path')
+
+    # 2021년 4월 KBO 경기 스케쥴을 가져옵니다.
+    # Get the KBO match schedule for April 2021.
+    >>> month = kbodata.get_monthly_schedule(2021,4,'chromedriver_path')
+
+    # 2021년 KBO 경기 스케쥴을 가져옵니다. 
+    # Get the KBO match schedule for 2021.
+    >>> year = kbodata.get_yearly_schedule(2021,'chromedriver_path')
+```
+
+해당 스케쥴을 바탕으로 경기 정보를 JSON 형식으로 가져옵니다.  
+It will be broght match information in JSON format based on the schedule.  
+
+```python
+    # 2021년 4월 20일의 KBO 경기 정보를 가져옵니다.
+    # Get the KBO match information for April 20, 2021.
+    >>> day_data = kbodata.get_game_data(day,'chromedriver_path')
+
+    # 2021년 4월 KBO 경기 정보를 가져옵니다.
+    # Get the KBO match information for April 2021.
+    >>> month_data = kbodata.get_game_data(month,'chromedriver_path')
+
+    # 2021년 KBO 경기 정보를 가져옵니다. 
+    # Get the KBO match information for 2021.
+    >>> year_data = kbodata.get_game_data(year,'chromedriver_path')
+```
+
+JSON 형식은 아래와 같습니다.  
+The JSON format is as below.
+
+```ini
+    { id: date_gameid,
+    contents: {
+      'scoreboard': []
+      'ETC_info': {}
+      'away_batter': []
+      'home_batter': []
+      'away_pitcher': []
+      'home_pitcher': []
+        }
+    }
+```
+
+## 데이터 변형하기 (kbodata.load module)
+
+가져온 데이터들을 특정 파일 타입으로 변환합니다. 지원하는 파일 타입은 아래와 같습니다.  
+This module converts data into specific file types. The supported file types are as follows.
+
+- DataFrame(pandas)
+- Dict
+
+```python
+    # 팀 경기 정보만을 정리하여 DataFrame으로 변환합니다.
+    scoreboard = kbodata.scoreboard_to_DataFrame(day_data)
+    # 타자 정보만을 정리하여 DataFrame으로 변환합니다.
+    batter = kbodata.batter_to_DataFrame(day_data)
+    # 투수 정보만을 정리하여 DataFrame으로 변환합니다.
+    pitcher = kbodata.pitcher_to_DataFrame(day_data)
+
+    # 팀 경기 정보만을 정리하여 Dict으로 변환합니다.
+    scoreboard = kbodata.scoreboard_to_Dict(day_data)
+    # 타자 정보만을 정리하여 Dict으로 변환합니다.
+    batter = kbodata.batter_to_Dict(day_data)
+    # 투수 정보만을 정리하여 Dict으로 변환합니다.
+    pitcher = kbodata.pitcher_to_Dict(day_data)
+```
+
+변환된 데이터에 대한 정보는 아래의 링크에서 확인할 수 있습니다.  
+You can find information about the converted data at the link below.
+
+- Scoreboard: https://github.com/Hyeonji-Ryu/kbo-data/blob/main/docs/scoreboard.md
+- Batter: https://github.com/Hyeonji-Ryu/kbo-data/blob/main/docs/batter.md
+- Pitcher: https://github.com/Hyeonji-Ryu/kbo-data/blob/main/docs/pitcher.md
+
+## Issues
+
+KBO 공식 홈페이지에 없는 데이터는 제공되지 않습니다. 데이터가 제공되지 않는 경기 정보는 아래와 같습니다.  
+Data that is not on the KBO official website is not provided. Match information for which data is not provided are listed below.  
+
+### 경기 기준 (from game)
+
+- 2008-03-30 LTHH0
+- 2009-04-04 WOLT0
+- 2010-03-20 OBLT0
+- 2010-03-20 WOSS0
+- 2015-07-08 HTWO0
+- 2018-08-01 WOSK0
+
+### 날짜 기준 (from date)
+
+- 2013-03-09
+- 2013-03-10
+- 2013-03-11
+- 2013-03-12
+- 2013-03-13
+- 2013-03-14
+- 2013-03-15
+- 2013-03-16
+- 2013-03-17
+- 2013-03-18
+- 2013-03-19
+- 2013-03-20
 
-packages = \
-['kbodata', 'kbodata.get', 'kbodata.load', 'kbodata.parser']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bs4>=0.0.1,<0.0.2',
- 'lxml>=4.6.2,<5.0.0',
- 'pandas>=1.2.2,<2.0.0',
- 'requests>=2.25.1,<3.0.0',
- 'selenium>=3.141.0,<4.0.0',
- 'tqdm>=4.61.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'kbodata',
-    'version': '0.1.7',
-    'description': 'Scraping Korea Baseball Game information',
-    'long_description': "# What is kbo-data\n\nkbo-data는 한국프로야구 경기정보를 스크래핑하는 파이썬 패키지입니다.  \nkbo-data is a Python package that provides Korean professional baseball game information by scraping.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kbodata)\n[![PyPI](https://img.shields.io/pypi/v/kbodata)](https://pypi.org/project/kbodata/)\n[![GitHub license](https://img.shields.io/github/license/Hyeonji-Ryu/kbo-data)](https://github.com/Hyeonji-Ryu/kbo-data/blob/main/LICENSE)\n\n## Required\n\n이 패키지를 사용하기 위해서는 chrome driver가 필요합니다. chrome driver는 [해당 페이지](https://chromedriver.chromium.org/downloads)에서 다운로드할 수 있습니다.  \nThis package is required chrome driver. You can download it from [this page](https://chromedriver.chromium.org/downloads)\n\n## How to Use\n\n### 패키지 설치하기\n\n먼저 패키지를 설치합니다.  \nyou have to install kbodata package first.\n\n```bash\npip install kbodata\n```\n\n### 데이터 가져오기 (kbodata.get module)\n\n원하는 날짜의 경기 스케쥴을 다운로드 받습니다.  \nyou can download KBO match schedule that you want to get.\n\n```python\n    import kbodata\n\n    # 2021년 4월 20일의 KBO 경기 스케쥴을 가져옵니다.\n    # Get the KBO match schedule for April 20, 2021.\n    >>> day = kbodata.get_daily_schedule(2021,4,20,'chromedriver_path')\n\n    # 2021년 4월 KBO 경기 스케쥴을 가져옵니다.\n    # Get the KBO match schedule for April 2021.\n    >>> month = kbodata.get_monthly_schedule(2021,4,'chromedriver_path')\n\n    # 2021년 KBO 경기 스케쥴을 가져옵니다. \n    # Get the KBO match schedule for 2021.\n    >>> year = kbodata.get_yearly_schedule(2021,'chromedriver_path')\n```\n\n해당 스케쥴을 바탕으로 경기 정보를 JSON 형식으로 가져옵니다.  \nIt will be broght match information in JSON format based on the schedule.  \n\n```python\n    # 2021년 4월 20일의 KBO 경기 정보를 가져옵니다.\n    # Get the KBO match information for April 20, 2021.\n    >>> day_data = kbodata.get_game_data(day,'chromedriver_path')\n\n    # 2021년 4월 KBO 경기 정보를 가져옵니다.\n    # Get the KBO match information for April 2021.\n    >>> month_data = kbodata.get_game_data(month,'chromedriver_path')\n\n    # 2021년 KBO 경기 정보를 가져옵니다. \n    # Get the KBO match information for 2021.\n    >>> year_data = kbodata.get_game_data(year,'chromedriver_path')\n```\n\nJSON 형식은 아래와 같습니다.  \nThe JSON format is as below.\n\n```ini\n    { id: date_gameid,\n    contents: {\n      'scoreboard': []\n      'ETC_info': {}\n      'away_batter': []\n      'home_batter': []\n      'away_pitcher': []\n      'home_pitcher': []\n        }\n    }\n```\n\n## 데이터 변형하기 (kbodata.load module)\n\n가져온 데이터들을 특정 파일 타입으로 변환합니다. 지원하는 파일 타입은 아래와 같습니다.  \nThis module converts data into specific file types. The supported file types are as follows.\n\n- DataFrame(pandas)\n- Dict\n\n```python\n    # 팀 경기 정보만을 정리하여 DataFrame으로 변환합니다.\n    scoreboard = kbodata.scoreboard_to_DataFrame(day_data)\n    # 타자 정보만을 정리하여 DataFrame으로 변환합니다.\n    batter = kbodata.batter_to_DataFrame(day_data)\n    # 투수 정보만을 정리하여 DataFrame으로 변환합니다.\n    pitcher = kbodata.pitcher_to_DataFrame(day_data)\n\n    # 팀 경기 정보만을 정리하여 Dict으로 변환합니다.\n    scoreboard = kbodata.scoreboard_to_Dict(day_data)\n    # 타자 정보만을 정리하여 Dict으로 변환합니다.\n    batter = kbodata.batter_to_Dict(day_data)\n    # 투수 정보만을 정리하여 Dict으로 변환합니다.\n    pitcher = kbodata.pitcher_to_Dict(day_data)\n```\n\n변환된 데이터에 대한 정보는 아래의 링크에서 확인할 수 있습니다.  \nYou can find information about the converted data at the link below.\n\n- Scoreboard: https://github.com/Hyeonji-Ryu/kbo-data/blob/main/docs/scoreboard.md\n- Batter: https://github.com/Hyeonji-Ryu/kbo-data/blob/main/docs/batter.md\n- Pitcher: https://github.com/Hyeonji-Ryu/kbo-data/blob/main/docs/pitcher.md\n\n## Issues\n\nKBO 공식 홈페이지에 없는 데이터는 제공되지 않습니다. 데이터가 제공되지 않는 경기 정보는 아래와 같습니다.  \nData that is not on the KBO official website is not provided. Match information for which data is not provided are listed below.  \n\n### 경기 기준 (from game)\n\n- 2008-03-30 LTHH0\n- 2009-04-04 WOLT0\n- 2010-03-20 OBLT0\n- 2010-03-20 WOSS0\n- 2015-07-08 HTWO0\n- 2018-08-01 WOSK0\n\n### 날짜 기준 (from date)\n\n- 2013-03-09\n- 2013-03-10\n- 2013-03-11\n- 2013-03-12\n- 2013-03-13\n- 2013-03-14\n- 2013-03-15\n- 2013-03-16\n- 2013-03-17\n- 2013-03-18\n- 2013-03-19\n- 2013-03-20\n",
-    'author': 'Hyeonji-Ryu',
-    'author_email': 'dev.bearabbit@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Hyeonji-Ryu/kbo-data',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

