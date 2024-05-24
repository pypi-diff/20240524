# Comparing `tmp/syncedlyrics-0.8.0.tar.gz` & `tmp/syncedlyrics-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncedlyrics-0.8.0.tar", max compression
+gzip compressed data, was "syncedlyrics-0.9.0.tar", max compression
```

## Comparing `syncedlyrics-0.8.0.tar` & `syncedlyrics-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1061 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/LICENSE
--rw-r--r--   0        0        0     1569 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/README.md
--rw-r--r--   0        0        0      832 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2175 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/__init__.py
--rw-r--r--   0        0        0       87 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/__main__.py
--rw-r--r--   0        0        0     1332 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/cli.py
--rw-r--r--   0        0        0      221 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/__init__.py
--rw-r--r--   0        0        0     1040 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/base.py
--rw-r--r--   0        0        0     1921 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/deezer.py
--rw-r--r--   0        0        0     1434 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/lrclib.py
--rw-r--r--   0        0        0     1248 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/lyricsify.py
--rw-r--r--   0        0        0     1445 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/megalobiz.py
--rw-r--r--   0        0        0     4300 2024-01-14 15:24:34.529494 syncedlyrics-0.8.0/syncedlyrics/providers/musixmatch.py
--rw-r--r--   0        0        0     3324 2024-01-14 15:24:34.533494 syncedlyrics-0.8.0/syncedlyrics/providers/netease.py
--rw-r--r--   0        0        0      771 2024-01-14 15:24:34.533494 syncedlyrics-0.8.0/syncedlyrics/providers/spotify.py
--rw-r--r--   0        0        0     2863 2024-01-14 15:24:34.533494 syncedlyrics-0.8.0/syncedlyrics/utils.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 syncedlyrics-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2208 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/README.md
+-rw-r--r--   0        0        0      831 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2805 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/__init__.py
+-rw-r--r--   0        0        0       87 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/__main__.py
+-rw-r--r--   0        0        0     1664 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/cli.py
+-rw-r--r--   0        0        0      248 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/base.py
+-rw-r--r--   0        0        0     1962 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/deezer.py
+-rw-r--r--   0        0        0     1076 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/genius.py
+-rw-r--r--   0        0        0     1454 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/lrclib.py
+-rw-r--r--   0        0        0     1248 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/lyricsify.py
+-rw-r--r--   0        0        0     1463 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/megalobiz.py
+-rw-r--r--   0        0        0     5011 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/musixmatch.py
+-rw-r--r--   0        0        0     2772 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/netease.py
+-rw-r--r--   0        0        0      776 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/providers/spotify.py
+-rw-r--r--   0        0        0     3333 2024-03-22 13:10:02.601752 syncedlyrics-0.9.0/syncedlyrics/utils.py
+-rw-r--r--   0        0        0     3275 1970-01-01 00:00:00.000000 syncedlyrics-0.9.0/PKG-INFO
```

### Comparing `syncedlyrics-0.8.0/LICENSE` & `syncedlyrics-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syncedlyrics-0.8.0/README.md` & `syncedlyrics-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,37 +13,54 @@
 syncedlyrics "SEARCH_TERM"
 ```
 
 #### Available Options
 | Flag | Description |
 | --- | --- |
 | `-o` | Path to save `.lrc` lyrics, default="{search_term}.lrc" |
-| `-p` | Comma-separated list of providers to include in searching |
+| `-p` | Space-separated list of [providers](#providers) to include in searching |
 | `-l` | Language code of the translation ([ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) format) |
 | `-v` | Use this flag to show the logs |
 | `--allow-plain` | Return a plain text (not synced) lyrics if no LRC format was found |
+| `--enhanced` | Return an [Enhanced](https://en.wikipedia.org/wiki/LRC_(file_format)#A2_extension:_word_time_tag) (word-level karaoke) format
 
 ### Python
 ```py
+# This simple
 lrc = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
-```
-Or with options:
-```py
+
+# Or with options:
 syncedlyrics.search("...", allow_plain_format=True, save_path="{search_term}_1234.lrc", providers=["NetEase"])
-```
-Get a translation along with the original lyrics (seperated by `\n`):
-```
+
+# Get a translation along with the original lyrics (separated by `\n`):
 syncedlyrics.search("...", lang="de")
+
+# Get a word-by-word (karaoke) synced-lyrics if available
+syncedlyrics.search("...", enhanced=True)
 ```
 
 ## Providers
 - [Musixmatch](https://www.musixmatch.com/)
+- [Deezer](https://deezer.com/)
 - [Lrclib](https://github.com/tranxuanthang/lrcget/issues/2#issuecomment-1326925928)
 - [NetEase](https://music.163.com/)
-- [Megalobiz](https://www.megalobiz.com/)
+- [Genius](https://genius.com) (For plain format)
+- ~~[Megalobiz](https://www.megalobiz.com/)~~ (Website not working anymore)
 - ~~[Lyricsify](https://www.lyricsify.com/)~~ (Broken duo to Cloudflare protection)
-- ~~[Deezer](https://deezer.com/)~~ (Broken)
 
 Feel free to suggest more providers or make PRs to fix the broken ones.
 
 ## License
 [MIT](https://github.com/rtcq/syncedlyrics/blob/master/LICENSE)
+
+## Citation
+If you use this library in your research, you can cite as follows:
+```
+@misc{syncedlyrics,
+  author = {Momeni, Mohammad},
+  title = {syncedlyrics},
+  year = {2022},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/moehmeni/syncedlyrics}},
+}
+```
```

### Comparing `syncedlyrics-0.8.0/pyproject.toml` & `syncedlyrics-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syncedlyrics"
-version = "0.8.0"
+version = "0.9.0"
 description = "Get an LRC format (synchronized) lyrics for your music"
 repository = "https://github.com/rtcq/syncedlyrics"
 urls = { "Bug Tracker" = "https://github.com/rtcq/syncedlyrics/issues" }
 authors = ["Momo <lo3me@proton.me>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
@@ -12,20 +12,20 @@
     "Topic :: Multimedia :: Sound/Audio :: Players",
     "Topic :: Multimedia :: Sound/Audio :: Speech",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 requests = "^2.31.0"
-rapidfuzz = "^3.5.2"
-beautifulsoup4 = "^4.12.2"
+beautifulsoup4 = "^4.12.3"
+rapidfuzz = "^3.6.2"
 
 [tool.poetry.scripts]
 syncedlyrics = "syncedlyrics.cli:cli_handler"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.11.0"
-pytest = "^7.4.3"
+black = "^24.2.0"
+pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/__init__.py` & `syncedlyrics-0.9.0/syncedlyrics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,60 +3,78 @@
 
 ```py
 import syncedlyrics
 lrc_text = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
 ```
 """
 
-from typing import Optional, List
 import logging
-from .providers import NetEase, Megalobiz, Musixmatch, Lrclib
+from typing import List, Optional
+
+from .providers import Deezer, Lrclib, Musixmatch, NetEase, Genius
 from .utils import is_lrc_valid, save_lrc_file
 
 logger = logging.getLogger(__name__)
 
 
 def search(
     search_term: str,
     allow_plain_format: bool = False,
-    save_path: str = None,
-    providers: List[str] = None,
-    lang: str = None,
+    save_path: Optional[str] = None,
+    providers: Optional[List[str]] = None,
+    lang: Optional[str] = None,
+    enhanced: bool = False,
 ) -> Optional[str]:
     """
     Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
     ### Arguments
     - `search_term`: The search term to find the track
     - `allow_normal_format`: Return a plain text (not synced) lyrics if not LRC was found
     - `save_path`: Path to save `.lrc` lyrics. No saving if `None`
     - `providers`: A list of provider names to include in searching; loops over all the providers as soon as an LRC is found
     - `lang`: Language of the translation along with the lyrics. **Only supported by Musixmatch**
+    - `enhanced`: Returns word by word synced lyrics if available. **Only supported by Musixmatch**
     """
-    _providers = [Musixmatch(lang=lang), Lrclib(), NetEase(), Megalobiz()]
+    _providers = [
+        Musixmatch(lang=lang, enhanced=enhanced),
+        Lrclib(),
+        Deezer(),
+        NetEase(),
+        Genius(),
+    ]
     if providers and any(providers):
         # Filtering the providers
         _providers = [
             p
             for p in _providers
             if p.__class__.__name__.lower() in [p.lower() for p in providers]
         ]
     if not _providers:
         logger.error(
             f"Providers {providers} not found in the list of available providers."
         )
-        return
+        return None
     lrc = None
     for provider in _providers:
         logger.debug(f"Looking for an LRC on {provider.__class__.__name__}")
-        lrc = provider.get_lrc(search_term)
-        if is_lrc_valid(lrc, allow_plain_format):
+        _l = provider.get_lrc(search_term)
+        if enhanced and not _l:
+            # Since enhanced is only supported by Musixmatch, break if no LRC is found
+            break
+        if is_lrc_valid(_l, allow_plain_format):
             logger.info(
                 f'synced-lyrics found for "{search_term}" on {provider.__class__.__name__}'
             )
+            lrc = _l
             break
+        else:
+            logger.debug(
+                f"Skip {provider.__class__.__name__} as the synced-lyrics is not valid. (allow_plain_format={allow_plain_format})"
+            )
+            logger.debug(f"Lyrics: {_l}")
     if not lrc:
         logger.info(f'No synced-lyrics found for "{search_term}" :(')
-        return
+        return None
     if save_path:
         save_path = save_path.format(search_term=search_term)
         save_lrc_file(save_path, lrc)
     return lrc
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/cli.py` & `syncedlyrics-0.9.0/syncedlyrics/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,45 @@
     """
     parser = argparse.ArgumentParser(
         description="Search for an LRC format (synchronized lyrics) of a music"
     )
     parser.add_argument("search_term", help="The search term to find the track.")
     parser.add_argument(
         "-p",
-        help="Comma-separated list of providers to include in searching",
+        help="Providers to include in the searching (separated by space). Default: all providers",
         default="",
+        choices=["deezer", "lrclib", "musixmatch", "netease", "genius"],
+        nargs="+",
+        type=str.lower,
+    )
+    parser.add_argument(
+        "-l", "--lang", help="Language of the translation along with the lyrics"
     )
-    parser.add_argument("-l", "--lang", help="Language of the translation along with the lyrics")
     parser.add_argument(
         "-o", "--output", help="Path to save '.lrc' lyrics", default="{search_term}.lrc"
     )
     parser.add_argument(
         "-v", "--verbose", help="Use this flag to show the logs", action="store_true"
     )
     parser.add_argument(
         "--allow-plain",
         help="Return a plain text (not synced) lyrics if not LRC was found",
         action="store_true",
     )
+    parser.add_argument(
+        "--enhanced",
+        help="Returns word by word synced lyrics (if available)",
+        action="store_true",
+    )
     args = parser.parse_args()
-    logging.basicConfig(level=logging.DEBUG if args.verbose else logging.INFO)
-    p = args.p.split(",") if args.p else None
-    lrc = search(args.search_term, args.allow_plain, args.output, p, lang=args.lang)
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
+    lrc = search(
+        args.search_term,
+        args.allow_plain,
+        args.output,
+        args.p,
+        lang=args.lang,
+        enhanced=args.enhanced,
+    )
     if lrc:
         print(lrc)
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/deezer.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/deezer.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,13 +40,14 @@
         lrc = ""
         for chunk in lrc_json_objs:
             if chunk.get("lrc_timestamp") and chunk.get("line"):
                 lrc += f"{chunk['lrc_timestamp']} {chunk['line']}\n"
         return lrc or None
 
     def get_lrc(self, search_term: str) -> Optional[str]:
-        search_results = self.session.get(self.SEARCH_ENDPOINT + search_term).json()
+        url = self.SEARCH_ENDPOINT + search_term.replace(" ", "+")
+        search_results = self.session.get(url).json()
         cmp_key = lambda t: f"{t.get('title')} {t.get('artist').get('name')}"
         track = get_best_match(search_results.get("data", []), search_term, cmp_key)
         if not track:
-            return
+            return None
         return self.get_lrc_by_id(track["id"])
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/lrclib.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/lrclib.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     def __init__(self) -> None:
         super().__init__()
 
     def get_lrc_by_id(self, track_id: str) -> Optional[str]:
         url = self.LRC_ENDPOINT + track_id
         r = self.session.get(url)
         if not r.ok:
-            return
+            return None
         track = r.json()
         return track.get("syncedLyrics", track.get("plainLyrics"))
 
     def get_lrc(self, search_term: str) -> Optional[str]:
         url = self.SEARCH_ENDPOINT
         r = self.session.get(url, params={"q": search_term})
         if not r.ok:
-            return
+            return None
         tracks = r.json()
         if not tracks:
-            return
+            return None
         tracks = sort_results(
             tracks, search_term, lambda t: f'{t["artistName"]} - {t["trackName"]}'
         )
         # _id = str(tracks[0]["id"])
         # Getting the first track that its `syncedLyrics` is not empty
         _id = None
         for track in tracks:
             if (track.get("syncedLyrics", "") or "").strip():
                 _id = str(track["id"])
                 break
         if not _id:
-            return
+            return None
         return self.get_lrc_by_id(_id)
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/lyricsify.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/lyricsify.py`

 * *Files identical despite different names*

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/megalobiz.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/megalobiz.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class Megalobiz(LRCProvider):
     """Megabolz provider class"""
 
     ROOT_URL = "https://www.megalobiz.com"
     SEARCH_ENDPOINT = ROOT_URL + "/search/all?qry={q}&searchButton.x=0&searchButton.y=0"
 
     def get_lrc(self, search_term: str) -> Optional[str]:
-        url = self.SEARCH_ENDPOINT.format(q=search_term)
+        url = self.SEARCH_ENDPOINT.format(q=search_term.replace(" ", "+"))
 
         def href_match(h: Optional[str]):
             if h and h.startswith("/lrc/maker/"):
                 return True
             return False
 
         a_tags_boud = SoupStrainer("a", href=href_match)
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/musixmatch.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/musixmatch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 """Musixmatch LRC provider"""
 
 from typing import Optional, List
 import time
 import json
 import os
 from .base import LRCProvider
-from ..utils import get_best_match
+from ..utils import get_best_match, format_time
 
 # Inspired from https://github.com/Marekkon5/onetagger/blob/0654131188c4df2b4b171ded7cdb927a4369746e/crates/onetagger-platforms/src/musixmatch.rs
 # Huge part converted from Rust to Py by ChatGPT :)
 
 
 class Musixmatch(LRCProvider):
     """Musixmatch provider class"""
 
     ROOT_URL = "https://apic-desktop.musixmatch.com/ws/1.1/"
 
-    def __init__(self, lang : str = None) -> None:
+    def __init__(self, lang: Optional[str] = None, enhanced: bool = False) -> None:
         super().__init__()
         self.lang = lang
+        self.enhanced = enhanced
         self.token = None
-        self.session.headers.update(
-            {
-                "authority": "apic-desktop.musixmatch.com",
-                "cookie": "AWSELBCORS=0; AWSELB=0",
-            }
-        )
 
     def _get(self, action: str, query: List[tuple]):
         if action != "token.get" and self.token is None:
             self._get_token()
         query.append(("app_id", "web-desktop-app-v1.0"))
         if self.token is not None:
             query.append(("usertoken", self.token))
@@ -78,25 +73,42 @@
                     ("subtitle_format", "lrc"),
                     ("translation_fields_set", "minimal"),
                     ("selected_language", self.lang),
                 ],
             )
             body_tr = r_tr.json()["message"]["body"]
         if not r.ok:
-            return
+            return None
         body = r.json()["message"]["body"]
         if not body:
-            return
+            return None
         lrc = body["subtitle"]["subtitle_body"]
         if self.lang is not None and body_tr:
             for i in body_tr["translations_list"]:
-                org, tr = i["translation"]["subtitle_matched_line"], i["translation"]["description"]
+                org, tr = (
+                    i["translation"]["subtitle_matched_line"],
+                    i["translation"]["description"],
+                )
                 lrc = lrc.replace(org, org + "\n" + f"({tr})")
         return lrc
 
+    def get_lrc_word_by_word(self, track_id: str) -> Optional[str]:
+        r = self._get("track.richsync.get", [("track_id", track_id)])
+        if r.ok and r.json()["message"]["header"]["status_code"] == 200:
+            lrc_raw = r.json()["message"]["body"]["richsync"]["richsync_body"]
+            lrc_raw = json.loads(lrc_raw)
+            lrc = ""
+            for i in lrc_raw:
+                lrc += f"[{format_time(i['ts'])}] "
+                for l in i["l"]:
+                    t = format_time(float(i["ts"]) + float(l["o"]))
+                    lrc += f"<{t}> {l['c']} "
+                lrc += "\n"
+            return lrc
+
     def get_lrc(self, search_term: str) -> Optional[str]:
         r = self._get(
             "track.search",
             [
                 ("q", search_term),
                 ("page_size", "5"),
                 ("page", "1"),
@@ -105,9 +117,12 @@
             ],
         )
         body = r.json()["message"]["body"]
         tracks = body["track_list"]
         cmp_key = lambda t: f"{t['track']['track_name']} {t['track']['artist_name']}"
         track = get_best_match(tracks, search_term, cmp_key)
         if not track:
-            return
-        return self.get_lrc_by_id(track["track"]["track_id"])
+            return None
+        track_id = track["track"]["track_id"]
+        if self.enhanced:
+            return self.get_lrc_word_by_word(track_id)
+        return self.get_lrc_by_id(track_id)
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/netease.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/netease.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,46 @@
 """NetEase (music.163.com) china-based provider"""
 
 from typing import Optional
 from .base import LRCProvider
 from ..utils import get_best_match
 
-headers = {
-    "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-    "accept-language": "en-US,en;q=0.9,fa;q=0.8",
-    "cache-control": "max-age=0",
-    "sec-ch-ua": '".Not/A)Brand";v="99", "Google Chrome";v="103", "Chromium";v="103"',
-    "sec-ch-ua-mobile": "?0",
-    "sec-ch-ua-platform": '"Windows"',
-    "sec-fetch-dest": "document",
-    "sec-fetch-mode": "navigate",
-    "sec-fetch-site": "none",
-    "sec-fetch-user": "?1",
-    "upgrade-insecure-requests": "1",
-    "cookie": "NMTID=00OAVK3xqDG726ITU6jopU6jF2yMk0AAAGCO8l1BA; JSESSIONID-WYYY=8KQo11YK2GZP45RMlz8Kn80vHZ9%2FGvwzRKQXXy0iQoFKycWdBlQjbfT0MJrFa6hwRfmpfBYKeHliUPH287JC3hNW99WQjrh9b9RmKT%2Fg1Exc2VwHZcsqi7ITxQgfEiee50po28x5xTTZXKoP%2FRMctN2jpDeg57kdZrXz%2FD%2FWghb%5C4DuZ%3A1659124633932; _iuqxldmzr_=32; _ntes_nnid=0db6667097883aa9596ecfe7f188c3ec,1659122833973; _ntes_nuid=0db6667097883aa9596ecfe7f188c3ec; WNMCID=xygast.1659122837568.01.0; WEVNSM=1.0.0; WM_NI=CwbjWAFbcIzPX3dsLP%2F52VB%2Bxr572gmqAYwvN9KU5X5f1nRzBYl0SNf%2BV9FTmmYZy%2FoJLADaZS0Q8TrKfNSBNOt0HLB8rRJh9DsvMOT7%2BCGCQLbvlWAcJBJeXb1P8yZ3RHA%3D; WM_NIKE=9ca17ae2e6ffcda170e2e6ee90c65b85ae87b9aa5483ef8ab3d14a939e9a83c459959caeadce47e991fbaee82af0fea7c3b92a81a9ae8bd64b86beadaaf95c9cedac94cf5cedebfeb7c121bcaefbd8b16dafaf8fbaf67e8ee785b6b854f7baff8fd1728287a4d1d246a6f59adac560afb397bbfc25ad9684a2c76b9a8d00b2bb60b295aaafd24a8e91bcd1cb4882e8beb3c964fb9cbd97d04598e9e5a4c6499394ae97ef5d83bd86a3c96f9cbeffb1bb739aed9ea9c437e2a3; WM_TID=AAkRFnl03RdABEBEQFOBWHCPOeMra4IL; playerid=94262567",
-}
-
 
 class NetEase(LRCProvider):
     """NetEase provider class"""
 
     API_ENDPOINT_METADATA = "https://music.163.com/api/search/pc"
     API_ENDPOINT_LYRICS = "https://music.163.com/api/song/lyric"
 
     def __init__(self) -> None:
         super().__init__()
-        self.session.headers.update(headers)
+        self.session.headers["cookie"] = (
+            "NMTID=00OAVK3xqDG726ITU6jopU6jF2yMk0AAAGCO8l1BA; JSESSIONID-WYYY=8KQo11YK2GZP45RMlz8Kn80vHZ9%2FGvwzRKQXXy0iQoFKycWdBlQjbfT0MJrFa6hwRfmpfBYKeHliUPH287JC3hNW99WQjrh9b9RmKT%2Fg1Exc2VwHZcsqi7ITxQgfEiee50po28x5xTTZXKoP%2FRMctN2jpDeg57kdZrXz%2FD%2FWghb%5C4DuZ%3A1659124633932; _iuqxldmzr_=32; _ntes_nnid=0db6667097883aa9596ecfe7f188c3ec,1659122833973; _ntes_nuid=0db6667097883aa9596ecfe7f188c3ec; WNMCID=xygast.1659122837568.01.0; WEVNSM=1.0.0; WM_NI=CwbjWAFbcIzPX3dsLP%2F52VB%2Bxr572gmqAYwvN9KU5X5f1nRzBYl0SNf%2BV9FTmmYZy%2FoJLADaZS0Q8TrKfNSBNOt0HLB8rRJh9DsvMOT7%2BCGCQLbvlWAcJBJeXb1P8yZ3RHA%3D; WM_NIKE=9ca17ae2e6ffcda170e2e6ee90c65b85ae87b9aa5483ef8ab3d14a939e9a83c459959caeadce47e991fbaee82af0fea7c3b92a81a9ae8bd64b86beadaaf95c9cedac94cf5cedebfeb7c121bcaefbd8b16dafaf8fbaf67e8ee785b6b854f7baff8fd1728287a4d1d246a6f59adac560afb397bbfc25ad9684a2c76b9a8d00b2bb60b295aaafd24a8e91bcd1cb4882e8beb3c964fb9cbd97d04598e9e5a4c6499394ae97ef5d83bd86a3c96f9cbeffb1bb739aed9ea9c437e2a3; WM_TID=AAkRFnl03RdABEBEQFOBWHCPOeMra4IL; playerid=94262567"
+        )
 
     def search_track(self, search_term: str) -> Optional[dict]:
         """Returns a `dict` containing some metadata for the found track."""
         params = {"limit": 10, "type": 1, "offset": 0, "s": search_term}
         response = self.session.get(self.API_ENDPOINT_METADATA, params=params)
         results = response.json().get("result", {}).get("songs")
         if not results:
-            return
+            return None
         cmp_key = lambda t: f"{t.get('name')} {t.get('artists')[0].get('name')}"
         track = get_best_match(results, search_term, cmp_key)
         # Update the session cookies from the new sent cookies for the next request.
         self.session.cookies.update(response.cookies)
         self.session.headers.update({"referer": response.url})
         return track
 
     def get_lrc_by_id(self, track_id: str) -> Optional[str]:
         params = {"id": track_id, "lv": 1}
         response = self.session.get(self.API_ENDPOINT_LYRICS, params=params)
         lrc = response.json().get("lrc", {}).get("lyric")
         if not lrc:
-            return
+            return None
         return lrc
 
     def get_lrc(self, search_term: str) -> Optional[str]:
         track = self.search_track(search_term)
         if not track:
-            return
+            return None
         return self.get_lrc_by_id(track["id"])
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/providers/spotify.py` & `syncedlyrics-0.9.0/syncedlyrics/providers/spotify.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Spotify(LRCProvider):
     """Spotify provider class"""
 
     def __init__(self) -> None:
         super().__init__()
 
     @classmethod
-    def get_track_id(search_term: str) -> Optional[str]:
+    def get_track_id(cls, search_term: str) -> Optional[str]:
         """Returns a Spotify track ID for given `search_term`"""
         # TODO: self.client.search(search_term) and processing the results
         raise NotImplementedError
 
     def get_lrc_by_id(self, track_id: str) -> Optional[str]:
         # TODO:
         raise NotImplementedError
```

### Comparing `syncedlyrics-0.8.0/syncedlyrics/utils.py` & `syncedlyrics-0.9.0/syncedlyrics/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Utility functions for `syncedlyrics` package"""
 
 from bs4 import BeautifulSoup, FeatureNotFound
 import rapidfuzz
 from typing import Union, Callable, Optional
+import datetime
 import re
 
 R_FEAT = re.compile(r"\((feat.+)\)", re.IGNORECASE)
 
 
 def is_lrc_valid(lrc: str, allow_plain_format: bool = False) -> bool:
     """Checks whether a given LRC string is valid or not."""
     if not lrc:
         return False
     if not allow_plain_format:
-        if not ("[" in lrc and "]" in lrc):
-            return False
+        conds = ["[" in l for l in lrc.split("\n")[5:8]]
+        return all(conds)
 
     return True
 
 
 def save_lrc_file(path: str, lrc_text: str):
     """Saves the `.lrc` file"""
     with open(path, "w", encoding="utf-8") as f:
@@ -33,14 +34,21 @@
     try:
         soup = BeautifulSoup(r.text, features="lxml", **kwargs)
     except FeatureNotFound:
         soup = BeautifulSoup(r.text, features="html.parser", **kwargs)
     return soup
 
 
+def format_time(time_in_seconds: float):
+    """Returns a [mm:ss.xx] formatted string from the given time in seconds."""
+    time = datetime.timedelta(seconds=time_in_seconds)
+    minutes, seconds = divmod(time.seconds, 60)
+    return f"{minutes:02}:{seconds:02}.{time.microseconds//10000:02}"
+
+
 def str_score(a: str, b: str) -> float:
     """Returns the similarity score of the two strings"""
     # if user does not specify any "feat" in the search term,
     # remove the "feat" from the search results' names
     a, b = a.lower(), b.lower()
     if "feat" not in b:
         a, b = R_FEAT.sub("", a), R_FEAT.sub("", b)
@@ -80,13 +88,19 @@
     min_score: int = 65,
 ) -> Optional[dict]:
     """
     Returns the best match from the API results based on the similarity score of the `compare_key`
     with the `search_term`.
     """
     if not results:
-        return
+        return None
     results = sort_results(results, search_term, compare_key=compare_key)
     best_match = results[0]
-    if not str_same(compare_key(best_match), search_term, n=min_score):
-        return
+
+    value_to_compare = (
+        best_match[compare_key]
+        if isinstance(compare_key, str)
+        else compare_key(best_match)
+    )
+    if not str_same(value_to_compare, search_term, n=min_score):
+        return None
     return best_match
```

### Comparing `syncedlyrics-0.8.0/PKG-INFO` & `syncedlyrics-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncedlyrics
-Version: 0.8.0
+Version: 0.9.0
 Summary: Get an LRC format (synchronized) lyrics for your music
 Home-page: https://github.com/rtcq/syncedlyrics
 License: MIT
 Author: Momo
 Author-email: lo3me@proton.me
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: rapidfuzz (>=3.5.2,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: rapidfuzz (>=3.6.2,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/rtcq/syncedlyrics/issues
 Project-URL: Repository, https://github.com/rtcq/syncedlyrics
 Description-Content-Type: text/markdown
 
 # syncedlyrics
  Get an LRC format (synchronized) lyrics for your music.
@@ -39,38 +39,55 @@
 syncedlyrics "SEARCH_TERM"
 ```
 
 #### Available Options
 | Flag | Description |
 | --- | --- |
 | `-o` | Path to save `.lrc` lyrics, default="{search_term}.lrc" |
-| `-p` | Comma-separated list of providers to include in searching |
+| `-p` | Space-separated list of [providers](#providers) to include in searching |
 | `-l` | Language code of the translation ([ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) format) |
 | `-v` | Use this flag to show the logs |
 | `--allow-plain` | Return a plain text (not synced) lyrics if no LRC format was found |
+| `--enhanced` | Return an [Enhanced](https://en.wikipedia.org/wiki/LRC_(file_format)#A2_extension:_word_time_tag) (word-level karaoke) format
 
 ### Python
 ```py
+# This simple
 lrc = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
-```
-Or with options:
-```py
+
+# Or with options:
 syncedlyrics.search("...", allow_plain_format=True, save_path="{search_term}_1234.lrc", providers=["NetEase"])
-```
-Get a translation along with the original lyrics (seperated by `\n`):
-```
+
+# Get a translation along with the original lyrics (separated by `\n`):
 syncedlyrics.search("...", lang="de")
+
+# Get a word-by-word (karaoke) synced-lyrics if available
+syncedlyrics.search("...", enhanced=True)
 ```
 
 ## Providers
 - [Musixmatch](https://www.musixmatch.com/)
+- [Deezer](https://deezer.com/)
 - [Lrclib](https://github.com/tranxuanthang/lrcget/issues/2#issuecomment-1326925928)
 - [NetEase](https://music.163.com/)
-- [Megalobiz](https://www.megalobiz.com/)
+- [Genius](https://genius.com) (For plain format)
+- ~~[Megalobiz](https://www.megalobiz.com/)~~ (Website not working anymore)
 - ~~[Lyricsify](https://www.lyricsify.com/)~~ (Broken duo to Cloudflare protection)
-- ~~[Deezer](https://deezer.com/)~~ (Broken)
 
 Feel free to suggest more providers or make PRs to fix the broken ones.
 
 ## License
 [MIT](https://github.com/rtcq/syncedlyrics/blob/master/LICENSE)
 
+## Citation
+If you use this library in your research, you can cite as follows:
+```
+@misc{syncedlyrics,
+  author = {Momeni, Mohammad},
+  title = {syncedlyrics},
+  year = {2022},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/moehmeni/syncedlyrics}},
+}
+```
+
```

