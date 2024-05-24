# Comparing `tmp/infinitode.py-1.0.5.tar.gz` & `tmp/infinitode.py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitode.py-1.0.5.tar", last modified: Sat Jul 15 21:03:48 2023, max compression
+gzip compressed data, was "infinitode.py-1.1.0.tar", last modified: Fri May 24 20:19:28 2024, max compression
```

## Comparing `infinitode.py-1.0.5.tar` & `infinitode.py-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 21:03:48.572318 infinitode.py-1.0.5/
--rw-rw-rw-   0        0        0     1100 2022-04-19 17:21:19.000000 infinitode.py-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     6254 2023-07-15 21:03:48.571057 infinitode.py-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5968 2023-07-15 20:58:30.000000 infinitode.py-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 21:03:48.543198 infinitode.py-1.0.5/infinitode/
--rw-rw-rw-   0        0        0     1469 2023-07-15 20:54:51.000000 infinitode.py-1.0.5/infinitode/__init__.py
--rw-rw-rw-   0        0        0      858 2023-07-15 20:55:02.000000 infinitode.py-1.0.5/infinitode/badge.py
--rw-rw-rw-   0        0        0    18199 2023-07-15 21:00:13.000000 infinitode.py-1.0.5/infinitode/core.py
--rw-rw-rw-   0        0        0      432 2023-07-15 20:55:16.000000 infinitode.py-1.0.5/infinitode/errors.py
--rw-rw-rw-   0        0        0     6821 2023-07-15 20:57:10.000000 infinitode.py-1.0.5/infinitode/leaderboard.py
--rw-rw-rw-   0        0        0     7530 2023-07-15 20:49:19.000000 infinitode.py-1.0.5/infinitode/player.py
--rw-rw-rw-   0        0        0        0 2022-04-25 15:30:52.000000 infinitode.py-1.0.5/infinitode/py.typed
--rw-rw-rw-   0        0        0     6571 2023-07-15 21:00:39.000000 infinitode.py-1.0.5/infinitode/score.py
--rw-rw-rw-   0        0        0      669 2023-07-15 20:57:01.000000 infinitode.py-1.0.5/infinitode/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 21:03:48.568915 infinitode.py-1.0.5/infinitode.py.egg-info/
--rw-rw-rw-   0        0        0     6254 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 21:03:48.572318 infinitode.py-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      758 2022-04-28 14:05:57.000000 infinitode.py-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:19:28.586048 infinitode.py-1.1.0/
+-rw-rw-rw-   0        0        0     1100 2022-04-19 17:21:19.000000 infinitode.py-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6254 2024-05-24 20:19:28.584780 infinitode.py-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5968 2023-07-15 20:58:30.000000 infinitode.py-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:19:28.562075 infinitode.py-1.1.0/infinitode/
+-rw-rw-rw-   0        0        0     1469 2024-05-24 20:15:46.000000 infinitode.py-1.1.0/infinitode/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 20:55:02.000000 infinitode.py-1.1.0/infinitode/badge.py
+-rw-rw-rw-   0        0        0    17232 2024-05-24 19:45:00.000000 infinitode.py-1.1.0/infinitode/core.py
+-rw-rw-rw-   0        0        0      432 2023-07-15 20:55:16.000000 infinitode.py-1.1.0/infinitode/errors.py
+-rw-rw-rw-   0        0        0     6837 2024-05-24 18:07:28.000000 infinitode.py-1.1.0/infinitode/leaderboard.py
+-rw-rw-rw-   0        0        0     7731 2024-05-24 19:06:44.000000 infinitode.py-1.1.0/infinitode/player.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 15:30:52.000000 infinitode.py-1.1.0/infinitode/py.typed
+-rw-rw-rw-   0        0        0     6581 2024-05-24 18:05:48.000000 infinitode.py-1.1.0/infinitode/score.py
+-rw-rw-rw-   0        0        0     1756 2024-05-24 19:53:30.000000 infinitode.py-1.1.0/infinitode/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:19:28.582773 infinitode.py-1.1.0/infinitode.py.egg-info/
+-rw-rw-rw-   0        0        0     6254 2024-05-24 20:19:28.000000 infinitode.py-1.1.0/infinitode.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-05-24 20:19:28.000000 infinitode.py-1.1.0/infinitode.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:19:28.000000 infinitode.py-1.1.0/infinitode.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-24 20:19:28.000000 infinitode.py-1.1.0/infinitode.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 20:19:28.000000 infinitode.py-1.1.0/infinitode.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:19:28.586048 infinitode.py-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      758 2022-04-28 14:05:57.000000 infinitode.py-1.1.0/setup.py
```

### Comparing `infinitode.py-1.0.5/LICENSE` & `infinitode.py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infinitode.py-1.0.5/PKG-INFO` & `infinitode.py-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitode.py
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python wrapper for the Infinitode 2 API.
 Home-page: https://github.com/Sprylos/infinitode.py
 Author: Sprylos
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `infinitode.py-1.0.5/README.md` & `infinitode.py-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `infinitode.py-1.0.5/infinitode/__init__.py` & `infinitode.py-1.1.0/infinitode/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 ~~~~~~~~~~~~~~~~~~~
 
 An asynchronous wrapper for the Infinitode API.
 """
 
 __author__ = "Sprylos"
 __title__ = "infinitode.py"
-__version__ = "1.0.5"
+__version__ = "1.1.0"
 __license__ = """MIT License
 
-Copyright (c) 2023 Sprylos
+Copyright (c) 2024 Sprylos
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `infinitode.py-1.0.5/infinitode/badge.py` & `infinitode.py-1.1.0/infinitode/badge.py`

 * *Files identical despite different names*

### Comparing `infinitode.py-1.0.5/infinitode/core.py` & `infinitode.py-1.1.0/infinitode/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 # std
 import re
-import time
 import asyncio
 import logging
 import datetime
 from typing import (
     Any,
     Dict,
     Optional,
@@ -17,16 +16,16 @@
 import aiohttp
 import bs4
 
 # local
 from .errors import APIError, BadArgument
 from .leaderboard import Leaderboard
 from .player import Player
-from .utils import try_int
 from .score import Score
+from .utils import async_expiring_cache, try_int
 
 
 __all__ = ("Session",)
 
 _log = logging.getLogger(__name__)
 
 ID_REGEX = re.compile(r"U-([A-Z0-9]{4}-){2}[A-Z0-9]{6}")
@@ -34,37 +33,29 @@
 # fmt: off
 LEVELS = (
     '1.1', '1.2', '1.3', '1.4', '1.5', '1.6', '1.7', '1.8', '1.b1',
     '2.1', '2.2', '2.3', '2.4', '2.5', '2.6', '2.7', '2.8', '2.b1',
     '3.1', '3.2', '3.3', '3.4', '3.5', '3.6', '3.7', '3.8', '3.b1',
     '4.1', '4.2', '4.3', '4.4', '4.5', '4.6', '4.7', '4.8', '4.b1',
     '5.1', '5.2', '5.3', '5.4', '5.5', '5.6', '5.7', '5.8', '5.b1', '5.b2',
-    '6.1', '6.2', '6.3', '6.4', '6.5', 'rumble', 'dev', 'zecred',
+    '6.1', '6.2', '6.3', '6.4', '6.5', '6.6', 'rumble', 'dev', 'zecred',
     'DQ1', 'DQ3', 'DQ4', 'DQ5', 'DQ7', 'DQ8', 'DQ9', 'DQ10', 'DQ11', 'DQ12',
 )
+MODES = ('score', 'waves')
+DIFFICULTIES = ('EASY', 'NORMAL', 'ENDLESS_I')
 # fmt: on
 
 
+def _base_url(beta: bool = False) -> str:
+    return f"https://{'beta.' if beta else ''}infinitode.prineside.com/"
+
+
 class Session:
     def __init__(self, session: Optional[aiohttp.ClientSession] = None) -> None:
         self._session = session or aiohttp.ClientSession()
-        self._cooldown: Dict[str, Any] = {
-            "DailyQuestInfo": 0.0,
-            "LatestNews": 0.0,
-            "DailyQuestLeaderboards": {},
-            "SkillPointLeaderboard": 0.0,
-            "BasicLevelsTopLeaderboards": {},
-            "Leaderboards": {},
-            "seasonal": 0.0,
-        }
-        self._DailyQuestLeaderboards: Dict[str, Leaderboard] = {}
-        self._BasicLevelsTopLeaderboards: Dict[str, Leaderboard] = {}
-        self._Leaderboards: Dict[str, Leaderboard] = {}
-        self._SkillPointLeaderboard: Leaderboard
-        self._seasonal: Leaderboard
 
     # async enter and exit allow for the fancy "with" statements
     # useful so you don't have to close the session yourself
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
@@ -83,31 +74,28 @@
         mode: Optional[str] = None,
         difficulty: Optional[str] = None,
     ) -> None:
         if mapname is not None and str(mapname) not in LEVELS:
             raise BadArgument("Invalid map: " + mapname)
         if playerid is not None and not ID_REGEX.match(playerid):
             raise BadArgument("Invalid playerid: " + playerid)
-        if mode is not None and not mode in ("score", "waves"):
-            raise BadArgument(
-                "Invalid mode (must be either 'score' or 'waves'): " + mode
-            )
-        if difficulty is not None and not difficulty in ("EASY", "NORMAL", "ENDLESS_I"):
+        if mode is not None and not mode in MODES:
+            raise BadArgument(f"Invalid mode (must be one of {MODES}): " + mode)
+        if difficulty is not None and not difficulty in DIFFICULTIES:
             raise BadArgument(
-                "Invalid difficulty (must be one of 'EASY', 'NORMAL', 'ENDLESS_I': "
-                + difficulty
+                f"Invalid difficulty (must be one of {DIFFICULTIES}): " + difficulty
             )
 
     # not being more specific with the payload type
     # so the typechecker stops annoying me
     async def _post(
-        self, arg: str, data: Optional[Dict[str, Any]] = None
+        self, arg: str, data: Optional[Dict[str, Any]] = None, *, beta: bool = False
     ) -> Dict[str, Any]:
         """Internal post method to communicate with Rainy's API"""
-        url = f"https://infinitode.prineside.com/?m=api&a={arg}&apiv=1&g=com.prineside.tdi2&v=282"
+        url = _base_url(beta) + f"?m=api&a={arg}&apiv=1&g=com.prineside.tdi2&v=282"
         _log.info("Sending POST request %s with data %s", arg, data)
         async with self._session.post(url, data=data) as r:
             try:
                 r.raise_for_status()
             except aiohttp.ClientResponseError:
                 raise APIError("Something went wrong. Try again later")
 
@@ -115,21 +103,23 @@
             _log.debug("Response to POST request %s: %s", arg, payload)
 
             if payload["status"] == "success":
                 return payload
             else:
                 raise APIError(f'Error response from server: {payload["message"]}')
 
-    # all the mapnames are Any because any python object can be converted to a str
+    @async_expiring_cache()
     async def leaderboards_rank(
         self,
         mapname: Any,
         playerid: str,
         mode: str = "score",
         difficulty: str = "NORMAL",
+        *,
+        beta: bool = False,
     ) -> Score:
         """
         Retrieves a Score of the given player.
         A valid playerid needs to be specified.
         """
         self._kwarg_check(
             mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty
@@ -139,62 +129,64 @@
             data={
                 "gamemode": "BASIC_LEVELS",
                 "difficulty": difficulty,
                 "playerid": playerid,
                 "mapname": str(mapname),
                 "mode": mode,
             },
+            beta=beta,
         )
         return Score.from_payload(
             "leaderboards_rank", mapname, mode, difficulty, playerid, payload
         )
 
+    @async_expiring_cache()
     async def leaderboards(
         self,
         mapname: Any,
         playerid: Optional[str] = None,
         mode: str = "score",
         difficulty: str = "NORMAL",
+        *,
+        beta: bool = False,
     ) -> Leaderboard:
         """
         Retrieves a Leaderboard.
         The leaderboard contains the top 200 scores of the specified map.
         """
         self._kwarg_check(
             mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty
         )
-        key = f"{difficulty}{mode}{mapname}"
-        if not playerid and (
-            time.time() < self._cooldown["Leaderboards"].get(key, 0) + 60
-        ):
-            return self._Leaderboards[key]
+
         payload = await self._post(
             "getLeaderboards",
             data={
                 "gamemode": "BASIC_LEVELS",
                 "difficulty": difficulty,
                 "playerid": playerid,
                 "mapname": str(mapname),
                 "mode": mode,
             },
+            beta=beta,
         )
         lb = Leaderboard.from_payload(
             "leaderboards", mapname, mode, difficulty, playerid, payload
         )
-        if lb.player is None:
-            self._Leaderboards[key] = lb
-            self._cooldown["Leaderboards"][key] = time.time()
+
         return lb
 
+    @async_expiring_cache()
     async def runtime_leaderboards(
         self,
         mapname: Any,
         playerid: str,
         mode: str = "score",
         difficulty: str = "NORMAL",
+        *,
+        beta: bool = False,
     ) -> Leaderboard:
         """
         Retrieves a Runtime Leaderboard (The one displayed top right in-game).
         A valid playerid needs to be specified.
         The leaderboard contains the top 200 scores and one Score for each top% of the specified map.
         """
         self._kwarg_check(
@@ -205,110 +197,111 @@
             data={
                 "gamemode": "BASIC_LEVELS",
                 "difficulty": difficulty,
                 "playerid": playerid,
                 "mapname": str(mapname),
                 "mode": mode,
             },
+            beta=beta,
         )
         return Leaderboard.from_payload(
             "runtime_leaderboards", mapname, mode, difficulty, playerid, payload
         )
 
+    @async_expiring_cache()
     async def skill_point_leaderboard(
-        self, playerid: Optional[str] = None
+        self, playerid: Optional[str] = None, *, beta: bool = False
     ) -> Leaderboard:
         """
         Retrieves the Skill Point Leaderboard.
         The leaderboard contains the top 3 skill point owners (looking at you, Eupho!).
         """
         if playerid is not None:
             self._kwarg_check(playerid=playerid)
-        elif time.time() < self._cooldown["SkillPointLeaderboard"] + 60:
-            return self._SkillPointLeaderboard
+
         payload = await self._post(
-            "getSkillPointLeaderboard", data={"playerid": playerid}
+            "getSkillPointLeaderboard", data={"playerid": playerid}, beta=beta
         )
         lb = Leaderboard.from_payload(
             "skill_point_leaderboard", "SP", "score", "NORMAL", playerid, payload
         )
-        if lb.player is None:
-            self._SkillPointLeaderboard = lb
-            self._cooldown["SkillPointLeaderboard"] = time.time()
+
         return lb
 
+    @async_expiring_cache()
     async def daily_quest_leaderboards(
         self,
         date: Union[datetime.datetime, str, None] = None,
         playerid: Optional[str] = None,
+        *,
+        beta: bool = False,
         warning: bool = True,
     ) -> Leaderboard:
         """
         Retrieves the Daily Quest Leaderboard for the given date.
         If an invalid or no date is provided, the date will be set to the current date.
         You may disable the invalid date warning by setting the warning param to False.
         The leaderboard contains the top 200 DQ players of the given date.
         """
         if date is None:
-            date = datetime.datetime.utcnow().strftime("%Y-%m-%d")
+            date = datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d")
         elif isinstance(date, datetime.datetime):
             date = date.strftime("%Y-%m-%d")
         else:
             try:
                 datetime.datetime.strptime(date, "%Y-%m-%d")
             except ValueError:
-                if warning == True:
+                if warning is True:
                     _log.warning(
                         "Invalid date in daily_quest_leaderboards (Use YYYY-MM-DD format): %s",
                         date,
                     )
-                date = datetime.datetime.utcnow().strftime("%Y-%m-%d")
-        if not playerid and (
-            time.time() < self._cooldown["DailyQuestLeaderboards"].get(date, 0) + 60
-        ):
-            return self._DailyQuestLeaderboards[date]
+                date = datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d")
+
         if playerid is not None:
             self._kwarg_check(playerid=playerid)
+
         payload = await self._post(
-            "getDailyQuestLeaderboards", data={"date": date, "playerid": playerid}
+            "getDailyQuestLeaderboards",
+            data={"date": date, "playerid": playerid},
+            beta=beta,
         )
         lb = Leaderboard.from_payload(
             "daily_quest_leaderboards",
             "DQ",
             "score",
             "NORMAL",
             playerid,
             payload,
             date=date,
         )
-        if lb.player is None:
-            self._DailyQuestLeaderboards[date] = lb
-            self._cooldown["DailyQuestLeaderboards"][date] = time.time()
+
         return lb
 
-    async def seasonal_leaderboard(self) -> Leaderboard:
+    @async_expiring_cache()
+    async def seasonal_leaderboard(self, beta: bool = False) -> Leaderboard:
         """
         Retrieves the season Leaderboard.
         The leaderboard contains the top 100 scores in the season.
         This coroutine never takes arguments.
         """
-        if time.time() < self._cooldown["seasonal"] + 60:
-            return self._seasonal
-        url = "https://infinitode.prineside.com/xdx/?url=seasonal_leaderboard"
+        url = _base_url(beta) + "xdx/?url=seasonal_leaderboard"
         _log.info("Sending GET request to %s", url)
+
         r = await self._session.get(url=url)
         try:
             r.raise_for_status()
         except aiohttp.ClientResponseError:
             raise APIError("Bad Gateway.")
+
         seasonal = bs4.BeautifulSoup(await r.text(), features="lxml")
 
         # fmt: off
         season = int(seasonal.select_one('label[i18n="season_formatted"]')['i18nf'].replace('["', '').replace('"]', ''))  # type: ignore
-        player_count = int(seasonal.select('label[i18n="player_count_formatted"]')[  # type: ignore
+        player_count = int(seasonal.select('label[i18n="player_count_formatted"]')[
             0]['i18nf'].replace('["', '').replace('"]', '').replace(',', ''))  # type: ignore
         lb = Leaderboard.from_payload(
             'seasonal_leaderboard', 'season', 'score', 'NORMAL', None, {
                 'status': 'success',
                 'player': {'total': player_count},
                 'leaderboards': [
                     {
@@ -317,22 +310,21 @@
                         'score': seasonal.select('label[nowrap="true"][text-align="right"]')[x].text.replace(',', '')
                     } for x in range(len(seasonal.select('div[x="90"]')))
                 ]
             }, season=season
         )
         # fmt: on
 
-        self._seasonal = lb
-        self._cooldown["seasonal"] = time.time()
         return lb
 
-    def _parse_player(self, content: str, playerid: str) -> Player:
+    def _parse_player(self, content: str, playerid: str, beta: bool) -> Player:
         data = bs4.BeautifulSoup(content, features="lxml")
         t: Dict[str, Any] = {}
         t["playerid"] = playerid
+        t["beta"] = beta
         t["nickname"] = data.select_one("label:not([i18n])").text  # type: ignore
         totals = data.select_one('div[width="522"][height="140"][align="center"]')
         if totals is None:
             t.update({"total_score": 0, "total_rank": 0, "total_top": 0})
         else:
             totals = totals.select("label")
             if len(totals) >= 4:
@@ -343,35 +335,39 @@
                 t.update({"total_score": 0, "total_rank": 0, "total_top": "0%"})
         comments = data.findAll(text=lambda text: isinstance(text, bs4.Comment))
         for x in comments:
             if "Level:" in x:
                 t["level"] = int(x.split(">")[3].split("<")[0])
                 break
         else:
-            t["level"] = 0
+            t["level"] = 1
         xp_data = data.select_one('div[width="330"][height="64"]')
         if xp_data is None:
             raise BadArgument("Invalid playerid: " + playerid)
         xp_data = xp_data.select_one("label").text.split(" / ")  # type: ignore
         t["xp"] = int(xp_data[0])
         t["xp_max"] = int(xp_data[1])
         season_xp_data = data.select_one(
             'div[width="530"][align="center"][height="64"][pad-bottom="10"]'
         )
         if season_xp_data is None:
-            raise BadArgument("Invalid playerid: " + playerid)
-        season_xp_borders = season_xp_data.select_one("label").text.split(" / ")  # type: ignore
-        t["season_xp"] = int(season_xp_borders[0])
-        t["season_xp_max"] = int(season_xp_borders[1])
-        season_level_data = season_xp_data.select_one(
-            'div[x="466"][width="64"][height="64"]'
-        )
-        if season_level_data is None:
-            raise BadArgument("Invalid playerid: " + playerid)
-        t["season_level"] = season_level_data["data"].split(":")[1]  # type: ignore
+            t["season_xp"] = 0
+            t["season_xp_max"] = 500
+            t["season_level"] = 1
+        else:
+            season_xp_borders = season_xp_data.select_one("label").text.split(" / ")  # type: ignore
+            t["season_xp"] = int(season_xp_borders[0])
+            t["season_xp_max"] = int(season_xp_borders[1])
+            season_level_data = season_xp_data.select_one(
+                'div[x="466"][width="64"][height="64"]'
+            )
+            if season_level_data is None:
+                t["season_level"] = 1
+            else:
+                t["season_level"] = int(season_level_data["data"].split(":")[1])  # type: ignore
 
         t["levels"] = {}
         for x in data.select('div[width="800"][height="40"]')[1:]:
             level_data = x.select("label")
             level = level_data[0].text
             if not x.select_one('label[i18n="not_ranked"]'):
                 rank = int(level_data[2].text.replace(",", ""))
@@ -398,15 +394,15 @@
             "daily-game",
             "invited-players",
             "killed-enemies",
             "mined-resources",
             "skillful",
             "of-merit",
             "beta-tester-season-2",
-            f"high-leveled-{t['level'] // 10}",
+            f"high-leveled-{t['level'] // 10 if t['level'] < 100 else 10}",
         ]
         for x in data.select('div[width="80"][height="80"]'):
             rar: str = x.select("img")[0]["src"].split("bg-")[1]  # type: ignore
             if rar in [
                 "not-received",
                 "common",
                 "rare",
@@ -437,27 +433,30 @@
         day = sp[0][:-2] if len(sp[0][:2]) == 2 else "0" + sp[0][:2]
         t["created_at"] = datetime.datetime.strptime(
             day + " " + sp[-2] + " " + sp[-1], "%d %B %Y"
         ).strftime("%Y-%m-%d")
 
         return Player(**t)
 
-    async def player(self, playerid: str) -> Player:
+    @async_expiring_cache()
+    async def player(self, playerid: str, beta: bool = False) -> Player:
         """
         Retrieves the Player.
         A valid playerid needs to be specified.
         """
         self._kwarg_check(playerid=playerid)
-        url = f"https://infinitode.prineside.com/xdx/index.php?url=profile/view&id={playerid}"
+        url = _base_url(beta) + "xdx/index.php?url=profile/view&id=" + playerid
         _log.info("Sending GET request to %s", url)
+
         r = await self._session.get(url=url)
         try:
             r.raise_for_status()
         except aiohttp.ClientResponseError:
             raise APIError("Bad Gateway.")
+
         loop = asyncio.get_event_loop()
         try:
             return await loop.run_in_executor(
-                None, self._parse_player, await r.text(), playerid
+                None, self._parse_player, await r.text(), playerid, beta
             )
         except Exception as exc:
             raise BadArgument("Invalid playerid: " + playerid) from exc
```

### Comparing `infinitode.py-1.0.5/infinitode/leaderboard.py` & `infinitode.py-1.1.0/infinitode/leaderboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         """Builds an instance with the given payload."""
         player: Dict[str, Any] = payload["player"]
         total: int = player["total"]
         if playerid is not None and (player["score"] and player["rank"] and total):
             player_score = Score(method, mapname, mode, difficulty, playerid, **player)
         else:
             player_score = None
+
         instance = cls(
             method,
             mapname,
             mode,
             difficulty,
             total,
             raw=payload,
@@ -102,14 +103,15 @@
             player=player_score,
             season=season,
         )
         for rank, score in enumerate(payload["leaderboards"], start=1):
             instance._append(
                 Score(method, mapname, mode, difficulty, rank=rank, **score)
             )
+            
         return instance
 
     @property
     def method(self) -> str:
         """The name of the method responsible for creating this leaderboard."""
         return self._method
```

### Comparing `infinitode.py-1.0.5/infinitode/player.py` & `infinitode.py-1.1.0/infinitode/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,39 @@
 __all__ = ("Player",)
 
 
 class Player:
     """Represents an in-game Player."""
 
     __slots__ = (
-        "_playerid",
-        "_nickname",
-        "_levels",
+        "_badges",
+        "_beta",
+        "_created_at",
+        "_daily_quest",
+        "_issues",
         "_level",
-        "_xp",
-        "_xp_max",
+        "_levels",
+        "_nickname",
+        "_playerid",
+        "_replays",
         "_season_level",
         "_season_xp",
         "_season_xp_max",
-        "_badges",
-        "_total_score",
+        "_skill_point",
         "_total_rank",
+        "_total_score",
         "_total_top",
-        "_replays",
-        "_issues",
         "_created_at",
-        "_daily_quest",
-        "_skill_point",
+        "_xp",
+        "_xp_max",
     )
 
     def __init__(
         self,
+        beta: bool,
         playerid: str,
         nickname: str,
         *,
         levels: Dict[str, Score],
         level: int,
         xp: int,
         xp_max: int,
@@ -55,14 +58,15 @@
         total_score: Union[int, str],
         total_rank: Union[int, str],
         total_top: str,
         replays: int,
         issues: int,
         created_at: str,
     ) -> None:
+        self._beta = beta
         self._playerid = playerid
         self._nickname = nickname
         self._levels = levels
         self._level = level
         self._xp = xp
         self._xp_max = xp_max
         self._season_level = season_level
@@ -155,15 +159,15 @@
     def created_at(self) -> str:
         """The player's creation date as a str in the format: '%Y-%m-%d'."""
         return self._created_at
 
     @property
     def avatar_link(self):
         """The link to the player's avatar. Invalid URL if the user doesn't have a pfp."""
-        return f"https://infinitode.prineside.com/img/avatars/{self._playerid}-128.png"
+        return f"https://{'beta.' if self._beta else ''}infinitode.prineside.com/img/avatars/{self._playerid}-128.png"
 
     @property
     def daily_quest(self):
         """Returns the player's daily quest score, or raises InfinitodeError if it wasn't fetched yet."""
         if self._daily_quest is MISSING:
             raise InfinitodeError(
                 "This score has not been fetched yet. Use ~.fetch_daily_quest first."
@@ -202,45 +206,49 @@
     async def fetch_daily_quest(
         self, session: Optional[Session] = None
     ) -> Optional[Score]:
         """
         Fetches the player's Daily Quest score if it wasn't fetched already.
         Returns None if the player is not ranked.
         """
-        if not self._daily_quest:
+        if not self._daily_quest:  # None or MISSING
             if session is None:
                 if self._daily_quest is MISSING:
                     raise InfinitodeError(
                         "You need to provide a Session to fetch the daily quest score."
                     )
                 else:
                     return self._daily_quest
+
             self._daily_quest = (
-                await session.daily_quest_leaderboards(playerid=self._playerid)
+                await session.daily_quest_leaderboards(playerid=self._playerid, beta=self._beta)
             ).player
+
         return self._daily_quest
 
     async def fetch_skill_point(
         self, session: Optional[Session] = None
     ) -> Optional[Score]:
         """
         Fetches the player's Skill Point score if it wasn't fetched already.
         Returns None if the player is not ranked.
         """
-        if not self._skill_point:
+        if not self._skill_point:  # None or MISSING
             if session is None:
                 if self._skill_point is MISSING:
                     raise InfinitodeError(
                         "You need to provide a Session to fetch the skill point score."
                     )
                 else:
                     return self._skill_point
+
             self._skill_point = (
-                await session.skill_point_leaderboard(playerid=self._playerid)
+                await session.skill_point_leaderboard(playerid=self._playerid, beta=self._beta)
             ).player
+
         return self._skill_point
 
     # magic methods
 
     def __repr__(self) -> str:
         attrs = {
             "playerid": self._playerid,
```

### Comparing `infinitode.py-1.0.5/infinitode/score.py` & `infinitode.py-1.1.0/infinitode/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 
     def format_score(self):
         """Formats the score the way i use it in my Advinas bot."""
         if self._nickname is None:
             raise InfinitodeError(
                 "The score is not valid for formatting (There is no nickname attached to this score)."
             )
+        
         return "#{:<5} {:<22} {:>0,}".format(
             self._rank,
             self._nickname if len(self._nickname) < 21 else f"{self._nickname[:19]}...",
             self._score,
         )
 
     def print_score(self):
```

### Comparing `infinitode.py-1.0.5/infinitode.py.egg-info/PKG-INFO` & `infinitode.py-1.1.0/infinitode.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitode.py
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python wrapper for the Infinitode 2 API.
 Home-page: https://github.com/Sprylos/infinitode.py
 Author: Sprylos
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `infinitode.py-1.0.5/setup.py` & `infinitode.py-1.1.0/setup.py`

 * *Files identical despite different names*

