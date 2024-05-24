# Comparing `tmp/haniwers-0.14.2.tar.gz` & `tmp/haniwers-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haniwers-0.14.2.tar", max compression
+gzip compressed data, was "haniwers-0.14.3.tar", max compression
```

## Comparing `haniwers-0.14.2.tar` & `haniwers-0.14.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.14.2/LICENSE
--rw-r--r--   0        0        0     5453 2024-05-21 07:08:23.440410 haniwers-0.14.2/README.md
--rw-r--r--   0        0        0       23 2024-05-21 07:08:23.442069 haniwers-0.14.2/haniwers/__init__.py
--rw-r--r--   0        0        0    12664 2024-05-18 01:48:36.884335 haniwers-0.14.2/haniwers/cli.py
--rw-r--r--   0        0        0    16312 2024-05-03 07:11:57.413718 haniwers-0.14.2/haniwers/config.py
--rw-r--r--   0        0        0    21139 2024-05-21 07:08:23.442954 haniwers-0.14.2/haniwers/daq.py
--rw-r--r--   0        0        0     4140 2023-08-13 06:32:10.841100 haniwers-0.14.2/haniwers/dataset.py
--rw-r--r--   0        0        0     3443 2024-05-21 07:08:23.444836 haniwers-0.14.2/haniwers/mimic.py
--rw-r--r--   0        0        0      774 2024-05-20 10:19:33.481471 haniwers-0.14.2/haniwers/postprocess.py
--rw-r--r--   0        0        0    10384 2024-05-18 01:48:36.885113 haniwers-0.14.2/haniwers/preprocess.py
--rw-r--r--   0        0        0     5952 2023-08-26 21:18:52.192190 haniwers-0.14.2/haniwers/raw2csv.py
--rw-r--r--   0        0        0     7600 2024-05-21 07:08:23.446352 haniwers-0.14.2/haniwers/threshold.py
--rw-r--r--   0        0        0     1319 2024-05-21 07:08:23.448992 haniwers-0.14.2/pyproject.toml
--rw-r--r--   0        0        0     6775 1970-01-01 00:00:00.000000 haniwers-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.14.3/LICENSE
+-rw-r--r--   0        0        0     6183 2024-05-22 14:20:19.674777 haniwers-0.14.3/README.md
+-rw-r--r--   0        0        0       23 2024-05-24 08:36:33.598734 haniwers-0.14.3/haniwers/__init__.py
+-rw-r--r--   0        0        0    11788 2024-05-22 14:20:19.753181 haniwers-0.14.3/haniwers/cli.py
+-rw-r--r--   0        0        0    16312 2024-05-22 14:19:28.812153 haniwers-0.14.3/haniwers/config.py
+-rw-r--r--   0        0        0    17700 2024-05-23 11:03:00.877951 haniwers-0.14.3/haniwers/daq.py
+-rw-r--r--   0        0        0     4140 2023-08-13 06:32:10.841100 haniwers-0.14.3/haniwers/dataset.py
+-rw-r--r--   0        0        0     3443 2024-05-23 11:03:00.878115 haniwers-0.14.3/haniwers/mimic.py
+-rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.14.3/haniwers/postprocess.py
+-rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.14.3/haniwers/preprocess.py
+-rw-r--r--   0        0        0     7600 2024-05-23 11:03:00.878451 haniwers-0.14.3/haniwers/threshold.py
+-rw-r--r--   0        0        0     1450 2024-05-24 08:36:33.609997 haniwers-0.14.3/pyproject.toml
+-rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 haniwers-0.14.3/PKG-INFO
```

### Comparing `haniwers-0.14.2/LICENSE` & `haniwers-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.2/README.md` & `haniwers-0.14.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,60 @@
 # Haniwers : ハニワーズ
 
 墳Qの解析コード（個人用）
 
 ![w:300](../docs/_static/haniwer.png)
 
-# ドキュメント
+# インストール
 
-関連するドキュメントは、このリポジトリのGitLab Pagesで公開
+```console
+$ pipx install haniwers
+$ which haniwers
+~/.local/bin/haniwers
 
-- ``haniwers``の使い方（built with sphinx）: https://qumasan.gitlab.io/haniwers/docs/
-- 解析ログブック（built with mystmd）: https://qumasan.gitlab.io/haniwers/
+$ haniwers --help
+```
 
+- ``pipx``（もしくは``pip3``）を使ってインストールできます
 
 ---
 
-# できること／したいこと
+# セットアップ
 
-- [x] 宇宙線検出器OSECHIで取得したデータを、解析可能なCSVファイルに変換する
-- [ ] データを理解するのに必要は基本プロットを作成する
-- [ ] まとめスライドのテンプレートを作成する
+## 作業ディレクトリを作成
+
+```console
+$ mkdir ~/repos/hnw-daq/
+```
+
+データを取得するディレクトリを作成してください。
+以後、このディレクトリをデータ取得するときのルートディレクトリとします。
+
+## 設定ファイルを作成
 
+[haniwers/examples](https://gitlab.com/qumasan/haniwers/-/tree/main/examples)にある設定ファイルをダウンロードして、
+作業ディレクトリに配置してください。
+（とてもめんどくさくてすみません。そのうちデフォルト設定を自動で生成できるようにしようと思います）
 
 ---
 
-# インストール
+# ドキュメント
 
-```console
-$ pipx install -i https://test.pypi.org/simple/ haniwers
-$ which haniwers
-```
+関連ドキュメントはGitLab Pagesで公開しています。
+
+- ``haniwers``の使い方（built with sphinx）: https://qumasan.gitlab.io/haniwers/docs/
+- 解析ログブック（built with mystmd）: https://qumasan.gitlab.io/haniwers/
 
+---
+
+# できること／したいこと
+
+- [x] 宇宙線検出器OSECHIで取得したデータを、解析可能なCSVファイルに変換する
+- [ ] データを理解するのに必要は基本プロットを作成する
+- [ ] まとめスライドのテンプレートを作成する
 
 ---
 
 # 開発者向け
 
 ## インストール＆ビルド
```

### Comparing `haniwers-0.14.2/haniwers/cli.py` & `haniwers-0.14.3/haniwers/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,46 +127,14 @@
     else:
         logger.warning("No data saved. Add --save to save data.")
         logger.debug(f"gzip: {len(gzip)}.")
         logger.debug(f"csv:  {len(csv)}.")
 
 
 @app.command()
-def raw2csv(load_from: str = "config.toml", force: bool = False) -> None:
-    """(Will be deprecated) Parse raw_data into .csv/.csv.gz
-
-    設定ファイルにあるファイルを変換します。
-    変換したくないファイルは skip/parseをfalseにしてください。
-    """
-    from .config import Config
-    from .raw2csv import parser
-
-    c = Config(load_from)
-    info = f"Loaded config : {c.fname}"
-    logger.info(info)
-
-    rules = c.rules
-
-    for data in c.runs:
-        # logger.debug(data)
-
-        if force:
-            logger.warning("Parse files forced")
-            data.parse = True
-
-        if data.parse:
-            msg = f"{data.name} : Parse files in {data.srcd}."
-            logger.info(msg)
-            parser(data, rules=rules)
-        else:
-            msg = f"{data.name} : Skipped."
-            logger.info(msg)
-
-
-@app.command()
 def ports() -> None:
     """Search available ports and show device names.
 
     :Note:
     - Linuxの場合: `/dev/ttyUSB0`
     - macOSの場合: `/dev/cu.usbserial-*` （CP2102N USB to UART Bridge Controller）
     - Windowsの場合: `COM3`
```

### Comparing `haniwers-0.14.2/haniwers/config.py` & `haniwers-0.14.3/haniwers/config.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.2/haniwers/daq.py` & `haniwers-0.14.3/haniwers/daq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-#! /usr/bin/env python3
-
-import argparse
 import csv
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import pandas as pd
 import pendulum
 import serial
 from deprecated import deprecated
-from icecream import ic
 from loguru import logger
 from pydantic import BaseModel
 from tqdm import tqdm
 
 from .config import Daq
 
 
@@ -35,91 +31,14 @@
     """BME280で測定した気温。[degC]"""
     atm: float = 0.0
     """BME280で測定した気圧。[Pa]"""
     hmd: float = 0.0
     """BME280で測定した湿度。[%]"""
 
 
-@deprecated(version="0.6.0", reason="Use typer.Typer for CLIs.")
-def init_parser():
-    """[deprecated] Initialize argument parser
-
-    :deprecated: `0.6.0`. Replaced with typer.Typer for CLIs.
-
-    """
-
-    now = pendulum.now().strftime("%Y%m%d")
-
-    parser = argparse.ArgumentParser(description="OSECHI DAQ")
-    parser.add_argument(
-        "--saved",
-        default=Path(now),
-        type=Path,
-        help=f"path to save data. (default={now})",
-    )
-    parser.add_argument(
-        "-q", action="count", default=0, help="decrease verbosity. (default=0)"
-    )
-    parser.add_argument(
-        "--skip", type=int, default=10, help="skip rows to print. (default=10)"
-    )
-
-    group1 = parser.add_argument_group("FILE", description="Options for files.")
-    group1.add_argument(
-        "--prefix",
-        default="osechi_data",
-        help="set prefix of filename. (default='osechi_data')",
-    )
-    group1.add_argument(
-        "--suffix",
-        choices=[".csv", ".dat"],
-        default=".csv",
-        help="set suffix of filename. (default='.csv')",
-    )
-    group1.add_argument(
-        "--max-rows",
-        metavar="ROWS",
-        type=int,
-        default=10000,
-        help="set max. rows per file. (default=10000)",
-    )
-    group1.add_argument(
-        "--max-files",
-        metavar="FILES",
-        type=int,
-        default=100,
-        help="set max. files to create. (default=100)",
-    )
-    group1.add_argument(
-        "--append",
-        action="store_true",
-        help="append data to existing file. (default=False)",
-    )
-
-    group2 = parser.add_argument_group(
-        "CONNECTION", description="Options for serial connection."
-    )
-    group2.add_argument(
-        "--device",
-        default="/dev/ttyUSB0",
-        help="set USB device name. (default='/dev/ttyUSB0')",
-    )
-    group2.add_argument(
-        "--baudrate", type=int, default=115200, help="set baudrate. (default=115200)"
-    )
-    group2.add_argument(
-        "--timeout",
-        type=int,
-        default=1000,
-        help="set read timeout in seconds. (default=1000)",
-    )
-
-    return parser
-
-
 def init_saved(daq: Daq) -> None:
     """Initialize destination directory to save data files
 
     保存先のディレクトリを初期化します。
     ディレクトリが存在しない場合は、作成します。
     ディレクトリが存在する場合は、``FileExistsError``を発行し、終了（``sys.exit``）します。
     ただし。DAQオブジェクトの``--append``オプションが有効な場合は、終了せずに追記を許可します。
@@ -211,55 +130,14 @@
     ts = pendulum.now().format("YYYY-MM-DDTHH[h]mm[m]ss[s]")
     stem = f"{args.prefix}_{ts}_{n:06}"
     fname = Path(stem).with_suffix(args.suffix)
     savef = Path(args.saved, fname)
     return savef
 
 
-@deprecated(version="0.6.0", reason="Use run.")
-def daq():
-    """[deprecated] Main DAQ
-
-    :deprecated: `0.6.0`. Use `run` instead.
-
-
-    """
-    ic.configureOutput(prefix="[running daq] | ")
-
-    parser = init_parser()
-    args = parser.parse_args()
-    init_saved(args)
-
-    ic(args)
-
-    # Open serial connection
-
-    with serial.Serial(
-        args.device, baudrate=args.baudrate, timeout=args.timeout
-    ) as port:
-        port.rts = False
-        port.dtr = False
-
-        for nfile in tqdm(range(args.max_files), desc="files"):
-            savef = get_savef(args, nfile)
-            ic(savef)
-
-            with savef.open("a") as f:
-                for nrow in tqdm(range(args.max_rows), leave=False, desc="rows"):
-                    now = pendulum.now().to_iso8601_string()
-                    data = port.readline().decode("utf-8").strip()
-                    row = f"{now} {data}"
-                    if args.suffix == ".csv":
-                        row = (",").join(row.split())
-                    f.write(row + "\n")
-
-                    if args.q == 0 and nrow % args.skip == 0:
-                        ic(nrow, row)
-
-
 def open_serial_connection(daq: Daq) -> serial.Serial:
     """Open and return a serial connection.
 
     シリアル通信（UART）に使うポートを準備します。
     ``with``構文で使う想定です。
 
     通信に使うUSBポート名（``device``）、
@@ -701,15 +579,7 @@
         msg = "-" * 40 + f"[{i+1:2d}/{n:2d}: {vth}]"
         logger.info(msg)
         row = scan_ch_vth(daq, duration, ch, vth)
         if row:
             rows.append(row)
 
     return rows
-
-
-if __name__ == "__main__":
-    try:
-        daq()
-    except KeyboardInterrupt as e:
-        ic(e)
-        sys.exit()
```

### Comparing `haniwers-0.14.2/haniwers/dataset.py` & `haniwers-0.14.3/haniwers/dataset.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.2/haniwers/mimic.py` & `haniwers-0.14.3/haniwers/mimic.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     """擬似イベントの気温。25度くらいのランダム値"""
     atm: float = 0.0
     """擬似イベントの気圧。1気圧（101800 Pa）くらいのランダム値"""
     hmd: float = 0.0
     """擬似イベントの湿度。50%くらいのランダム値"""
     seed: int | None = None
     """乱数シード。デフォルト値は`None`"""
-    is_real: bool = False
-    """データ種類のフラグ。擬似イベントの場合は常に`False`に設定"""
+    is_fake: bool = True
+    """データ種類のフラグ。FakeEventオブジェクトは常に``True``に設定"""
 
     def model_post_init(self, __context) -> None:
         """メンバー変数を初期化する"""
         random.seed(self.seed)
         self.timestamp = pendulum.now()
         self.top = random.randint(0, 10)
         self.mid = random.randint(0, 10)
```

### Comparing `haniwers-0.14.2/haniwers/postprocess.py` & `haniwers-0.14.3/haniwers/postprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.2/haniwers/threshold.py` & `haniwers-0.14.3/haniwers/threshold.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.2/pyproject.toml` & `haniwers-0.14.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.14.2"
+version = "0.14.3"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "haniwers/__init__.py:__version__",
 ]
 
 [tool.poetry]
 name = "haniwers"
-version = "0.14.2"
-description = "Analysis tool for FunQ project"
+version = "0.14.3"
+description = "Analysis tool for TanQ/FunQ project"
 authors = ["Shota Takahashi (KMI) <shotakaha@kmi.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://qumasan.gitlab.io/haniwers/docs/"
+repository = "https://gitlab.com/qumasan/haniwers/"
+keywords = ["muon"]
 
 [tool.poetry.scripts]
 haniwers = "haniwers.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13 "
 plotly = "^5.7.0"
```

### Comparing `haniwers-0.14.2/PKG-INFO` & `haniwers-0.14.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: haniwers
-Version: 0.14.2
-Summary: Analysis tool for FunQ project
+Version: 0.14.3
+Summary: Analysis tool for TanQ/FunQ project
+Home-page: https://qumasan.gitlab.io/haniwers/docs/
 License: MIT
+Keywords: muon
 Author: Shota Takahashi (KMI)
 Author-email: shotakaha@kmi.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,48 +29,70 @@
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.12.0,<0.13.0)
 Requires-Dist: vl-convert-python (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://gitlab.com/qumasan/haniwers/
 Description-Content-Type: text/markdown
 
 # Haniwers : ハニワーズ
 
 墳Qの解析コード（個人用）
 
 ![w:300](../docs/_static/haniwer.png)
 
-# ドキュメント
+# インストール
 
-関連するドキュメントは、このリポジトリのGitLab Pagesで公開
+```console
+$ pipx install haniwers
+$ which haniwers
+~/.local/bin/haniwers
 
-- ``haniwers``の使い方（built with sphinx）: https://qumasan.gitlab.io/haniwers/docs/
-- 解析ログブック（built with mystmd）: https://qumasan.gitlab.io/haniwers/
+$ haniwers --help
+```
 
+- ``pipx``（もしくは``pip3``）を使ってインストールできます
 
 ---
 
-# できること／したいこと
+# セットアップ
 
-- [x] 宇宙線検出器OSECHIで取得したデータを、解析可能なCSVファイルに変換する
-- [ ] データを理解するのに必要は基本プロットを作成する
-- [ ] まとめスライドのテンプレートを作成する
+## 作業ディレクトリを作成
+
+```console
+$ mkdir ~/repos/hnw-daq/
+```
+
+データを取得するディレクトリを作成してください。
+以後、このディレクトリをデータ取得するときのルートディレクトリとします。
+
+## 設定ファイルを作成
 
+[haniwers/examples](https://gitlab.com/qumasan/haniwers/-/tree/main/examples)にある設定ファイルをダウンロードして、
+作業ディレクトリに配置してください。
+（とてもめんどくさくてすみません。そのうちデフォルト設定を自動で生成できるようにしようと思います）
 
 ---
 
-# インストール
+# ドキュメント
 
-```console
-$ pipx install -i https://test.pypi.org/simple/ haniwers
-$ which haniwers
-```
+関連ドキュメントはGitLab Pagesで公開しています。
+
+- ``haniwers``の使い方（built with sphinx）: https://qumasan.gitlab.io/haniwers/docs/
+- 解析ログブック（built with mystmd）: https://qumasan.gitlab.io/haniwers/
 
+---
+
+# できること／したいこと
+
+- [x] 宇宙線検出器OSECHIで取得したデータを、解析可能なCSVファイルに変換する
+- [ ] データを理解するのに必要は基本プロットを作成する
+- [ ] まとめスライドのテンプレートを作成する
 
 ---
 
 # 開発者向け
 
 ## インストール＆ビルド
```

