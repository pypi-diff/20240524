# Comparing `tmp/beancount_multitool-0.3.0.tar.gz` & `tmp/beancount_multitool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_multitool-0.3.0.tar", max compression
+gzip compressed data, was "beancount_multitool-0.4.0.tar", max compression
```

## Comparing `beancount_multitool-0.3.0.tar` & `beancount_multitool-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.3.0/LICENSE
--rw-r--r--   0        0        0     2659 2024-05-20 00:34:34.734674 beancount_multitool-0.3.0/README.md
--rw-r--r--   0        0        0     1755 2024-05-20 00:37:50.244210 beancount_multitool-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      151 2024-05-20 00:11:51.835703 beancount_multitool-0.3.0/src/beancount_multitool/Institution.py
--rw-r--r--   0        0        0     4777 2024-05-20 00:15:30.523940 beancount_multitool-0.3.0/src/beancount_multitool/JABank.py
--rw-r--r--   0        0        0     4012 2024-05-20 00:15:30.524910 beancount_multitool-0.3.0/src/beancount_multitool/RakutenBank.py
--rw-r--r--   0        0        0     3843 2024-05-20 00:15:30.523918 beancount_multitool-0.3.0/src/beancount_multitool/RakutenCard.py
--rw-r--r--   0        0        0     4673 2024-05-20 00:15:30.524781 beancount_multitool-0.3.0/src/beancount_multitool/ShinseiBank.py
--rw-r--r--   0        0        0      454 2024-05-19 23:39:41.029470 beancount_multitool-0.3.0/src/beancount_multitool/__init__.py
--rw-r--r--   0        0        0      120 2024-05-20 00:15:30.523620 beancount_multitool-0.3.0/src/beancount_multitool/__main__.py
--rw-r--r--   0        0        0       22 2024-05-20 00:37:58.505169 beancount_multitool-0.3.0/src/beancount_multitool/__version__.py
--rw-r--r--   0        0        0     1219 2024-05-20 00:15:30.524259 beancount_multitool-0.3.0/src/beancount_multitool/as_transaction.py
--rw-r--r--   0        0        0     1662 2024-05-20 00:15:30.523942 beancount_multitool-0.3.0/src/beancount_multitool/cli.py
--rw-r--r--   0        0        0      588 2024-05-20 00:15:30.523657 beancount_multitool-0.3.0/src/beancount_multitool/read_config.py
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 beancount_multitool-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2696 2024-05-24 04:29:10.491065 beancount_multitool-0.4.0/README.md
+-rw-r--r--   0        0        0     1772 2024-05-24 03:24:29.912035 beancount_multitool-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-05-23 01:27:44.241769 beancount_multitool-0.4.0/src/beancount_multitool/Institution.py
+-rw-r--r--   0        0        0     5284 2024-05-24 04:10:42.855202 beancount_multitool-0.4.0/src/beancount_multitool/JABank.py
+-rw-r--r--   0        0        0     2268 2024-05-24 03:31:45.263121 beancount_multitool-0.4.0/src/beancount_multitool/MappingDatabase.py
+-rw-r--r--   0        0        0     4480 2024-05-24 03:32:40.768342 beancount_multitool-0.4.0/src/beancount_multitool/RakutenBank.py
+-rw-r--r--   0        0        0     4781 2024-05-24 03:32:40.768228 beancount_multitool-0.4.0/src/beancount_multitool/RakutenCard.py
+-rw-r--r--   0        0        0     5154 2024-05-24 04:06:12.816630 beancount_multitool-0.4.0/src/beancount_multitool/ShinseiBank.py
+-rw-r--r--   0        0        0      454 2024-05-19 23:39:41.029470 beancount_multitool-0.4.0/src/beancount_multitool/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-20 00:15:30.523620 beancount_multitool-0.4.0/src/beancount_multitool/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-24 03:24:20.721033 beancount_multitool-0.4.0/src/beancount_multitool/__version__.py
+-rw-r--r--   0        0        0     1475 2024-05-24 04:17:14.821049 beancount_multitool-0.4.0/src/beancount_multitool/as_transaction.py
+-rw-r--r--   0        0        0     1684 2024-05-23 14:57:04.901452 beancount_multitool-0.4.0/src/beancount_multitool/cli.py
+-rw-r--r--   0        0        0      421 2024-05-24 04:13:04.378795 beancount_multitool-0.4.0/src/beancount_multitool/get_beancount_config.py
+-rw-r--r--   0        0        0      557 2024-05-24 03:18:42.671213 beancount_multitool-0.4.0/src/beancount_multitool/get_value.py
+-rw-r--r--   0        0        0      654 2024-05-24 03:57:41.742099 beancount_multitool-0.4.0/src/beancount_multitool/read_config.py
+-rw-r--r--   0        0        0      380 2024-05-24 04:16:15.921218 beancount_multitool-0.4.0/src/beancount_multitool/tests/test_get_beancount_config.py
+-rw-r--r--   0        0        0      536 2024-05-24 04:02:22.544032 beancount_multitool-0.4.0/src/beancount_multitool/tests/test_get_value.py
+-rw-r--r--   0        0        0      231 2024-05-24 03:52:22.609021 beancount_multitool-0.4.0/src/beancount_multitool/tests/test_read_config.py
+-rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 beancount_multitool-0.4.0/PKG-INFO
```

### Comparing `beancount_multitool-0.3.0/LICENSE` & `beancount_multitool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.3.0/README.md` & `beancount_multitool-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Beancount Multitool
 
 [![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/beancount-multitool)](https://pypi.org/project/beancount-multitool/)
 ![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool)
-![static coverage badge](https://img.shields.io/badge/Coverage-97%25-blue)
+![static coverage badge](https://img.shields.io/badge/Coverage-89%25-blue)
 
 [Beancount Multitool](https://github.com/rlan/beancount-multitool/) is a command-line-interface (CLI) tool that converts financial data from financial institutions to Beancount files.
 
 The following institutions are supported:
 
 * Japan
   * [JA Bank ＪＡネットバンク](https://www.jabank.jp/)
   * [Rakuten Card 楽天カード](https://www.rakuten-card.co.jp/)
   * [Rakuten Bank 楽天銀行](https://www.rakuten-bank.co.jp/)
   * [SBI Shinsei Bank 新生銀行](https://www.sbishinseibank.co.jp/)
 
 What these scripts __can__ do:
 
 * Read raw CSV files downloaded from each institution's website.
-* Label debit and credit transactions to respective account types.
+* Label transactions with different sub-accounts, e.g., `Expenses:JP:Food:Grocery` or `Expenses:JP:Food:Restaurant`.
+  * Documentation is incoming.
+* Label unknown transactions to respective account types.
   * Debit: `Expenses:JP:Unknown:NameOfInstitution`
   * Credit: `Income:JP:Unknown:NameOfInstitution`
 
 What these scripts __can not__ (yet) do:
 
-* Label transactions with different sub-accounts, e.g., `Expenses:JP:Food:Grocery` or `Expenses:JP:Food:Restaurant`.
+* To be added.
 
 Installation:
 
 ```sh
 pip install beancount-multitool
 ```
```

### Comparing `beancount_multitool-0.3.0/pyproject.toml` & `beancount_multitool-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-multitool"
-version = "0.3.0"
+version = "0.4.0"
 description = "A CLI tool that converts financial data to Beancount files"
 authors = ["Rick Lan <rlan@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rlan/beancount-multitool"
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -22,14 +22,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
 click = "^8.1.7"
 tomli = { version = "^2.0.1", python = "<3.11" }
+tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
 pytest-cov = "^4.0"
 
 [tool.poetry.scripts]
 bean-mt = "beancount_multitool.cli:main"
```

### Comparing `beancount_multitool-0.3.0/src/beancount_multitool/JABank.py` & `beancount_multitool-0.4.0/src/beancount_multitool/ShinseiBank.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,85 @@
-from datetime import datetime
 import pandas as pd
+from pathlib import Path
+import uuid
 
 from .Institution import Institution
+from .MappingDatabase import MappingDatabase
 from .read_config import read_config
 from .as_transaction import as_transaction
+from .get_value import get_value
+from .get_beancount_config import get_beancount_config
 
 
-class JABank(Institution):
-    NAME = "ja_bank"  # used in cli.py and in tests
+class ShinseiBank(Institution):
+    NAME = "shinsei_bank"  # used in cli.py and in tests
 
     def __init__(self, config_file: str):
         # params
         self.config_file = config_file
-
+        # attributes
         self.config = read_config(config_file)
+        self.beancount_config = get_beancount_config(self.config)
+        # Use basedir of config_file to read mapping database files
+        base_dir = Path(config_file).parent
+        credit_file = get_value(self.config, "database", "credit_mapping")
+        self.credit_file = str(base_dir / credit_file)
+        debit_file = get_value(self.config, "database", "debit_mapping")
+        self.debit_file = str(base_dir / debit_file)
+        self.credit_db = MappingDatabase(self.credit_file)
+        self.debit_db = MappingDatabase(self.debit_file)
 
-    def read_transaction(self, file_name: str, year: int) -> pd.DataFrame:
+    def read_transaction(self, file_name: str) -> pd.DataFrame:
         """Read financial transactions into a Pandas DataFrame.
 
         Parameters
         ----------
         file_name : str
             Input file name.
 
         Returns
         -------
         pd.DataFrame
             A dataframe after pre-processing.
         """
-        df = pd.read_csv(file_name, encoding="shift_jis_2004")
+        df = pd.read_csv(file_name)
         print(f"Found {len(df.index)} transactions in {file_name}")
 
-        # Rename column names to English
+        # Rename column names to English.
+        # Column names can be English or Japanese
+        # "取引日","摘要","出金金額","入金金額","残高"
+        # "Value Date","Description","Debit","Credit","Balance"
+        # Lowercase names will be keyword arguments later.
         column_names = {
-            "番号": "Number",
-            "明細区分": "Detail Classification",
-            "取扱日付": "Handling Date",  # full name "Handling Date"
-            "起算日": "Starting Date",
-            "お支払金額": "Debit",  # full name = "Debit Amount"
-            "お預り金額": "Credit",  # full name = "Credit Amount"
-            "取引区分": "Transaction Classification",
+            "取引日": "date",
+            "摘要": "memo",
+            "出金金額": "Debit",
+            "入金金額": "Credit",
             "残高": "Balance",
-            "摘要": "Description",
+            "Value Date": "date",
+            "Description": "memo",
+            # "Debit": "Debit",
+            # "Credit": "Credit",
+            # "Balance": "Balance",
         }
         df.rename(columns=column_names, inplace=True)
 
         # Convert date column to a datetime object
-        df["Date"] = pd.to_datetime(
-            str(year) + "." + df["Handling Date"], format="%Y.%m月%d日"
-        )
-
-        cols = ["Debit", "Credit", "Balance"]
-        df[cols] = df[cols].replace({"\¥": "", ",": ""}, regex=True)
-        df.fillna({"Debit": 0, "Credit": 0}, inplace=True)
+        df["date"] = pd.to_datetime(df["date"], format="%Y/%m/%d")
+        # Fill empty cells with zeros
+        df.fillna(0, inplace=True)
         # Convert float to int
-        df[cols] = df[cols].astype(int)
+        df["Debit"] = df["Debit"].astype(int)
+        df["Credit"] = df["Credit"].astype(int)
+        df["amount"] = df["Credit"] - df["Debit"]
+
+        # Reverse row order because the oldest transaction is on the bottom
+        # Note: the index column is also reversed
+        df = df[::-1]
+
         # print(df.dtypes) # debug
         # print(df) # debug
         return df
 
     def write_bean(self, df: pd.DataFrame, file_name: str) -> None:
         """Write Beancount transactions to file
 
@@ -69,63 +90,51 @@
         file_name : str
             Output file name.
 
         Returns
         -------
         None
         """
+        try:
+            with open(file_name, "w", encoding="utf-8") as f:
+                for row in df.index:
+                    date = df["date"][row]
+                    amount = df["amount"][row]
+                    memo = df["memo"][row]
+                    metadata = {"memo": memo}
+
+                    if amount < 0:  # a debit
+                        accounts = self.debit_db.match(memo)
+                    else:  # a credit
+                        accounts = self.credit_db.match(memo)
+
+                    # Add UUID for manual transactions reconcilation between accounts
+                    if "#reconcile" in accounts[0]["tags"]:
+                        if amount > 0:  # a credit
+                            metadata["uuid"] = ""
+                        else:  # a debit
+                            metadata["uuid"] = str(uuid.uuid4())
+
+                    account_metadata = {}
+                    for x in range(1, len(accounts)):
+                        account_metadata[f"match{x+1}"] = str(accounts[x])
 
-        currency = self.config["currency"]
-        source_account = self.config["source_account"]
-        credit_target_account = self.config["default"]["credit"]["account"]
-        credit_narration = self.config["default"]["credit"]["narration"]
-        credit_tag = self.config["default"]["credit"]["tag"]
-        credit_flag = self.config["default"]["credit"]["flag"]
-        debit_target_account = self.config["default"]["debit"]["account"]
-        debit_narration = self.config["default"]["debit"]["narration"]
-        debit_tag = self.config["default"]["debit"]["tag"]
-        debit_flag = self.config["default"]["debit"]["flag"]
-
-        with open(file_name, "w", encoding="utf-8") as f:
-            for row in df.index:
-                date = df["Date"][row]
-                classification = df["Transaction Classification"][row]
-                description = df["Description"][row]
-                payee = classification + description
-                debit = df["Debit"][row]
-                credit = df["Credit"][row]
-
-                if credit == 0:  # a debit
                     output = as_transaction(
-                        date,
-                        payee,
-                        debit_narration,
-                        debit_tag,
-                        source_account,
-                        debit_target_account,
-                        debit,
-                        currency,
-                        debit_flag,
+                        date=date,
+                        amount=-amount,
+                        metadata=metadata,
+                        account_metadata=account_metadata,
+                        **accounts[0],
+                        **self.beancount_config,
                     )
-                else:  # a credit
-                    output = as_transaction(
-                        date,
-                        payee,
-                        credit_narration,
-                        credit_tag,
-                        source_account,
-                        credit_target_account,
-                        -credit,
-                        currency,
-                        credit_flag,
-                    )
-
-                # print(output) # debug
-                f.write(output)
-            print(f"Written {file_name}")
+                    # print(output) # debug
+                    f.write(output)
+                print(f"Written {file_name}")
+        except IOError as e:
+            print(e)
 
     def convert(self, csv_file: str, bean_file: str):
         """Convert transactions in a CSV file to a Beancount file
 
         Parameters
         ----------
         csv_file : str
@@ -134,10 +143,9 @@
         bean_file : str
             Output Beancount file name.
 
         Returns
         -------
         None
         """
-        year = datetime.now().year
-        df = self.read_transaction(csv_file, year)
+        df = self.read_transaction(csv_file)
         self.write_bean(df, bean_file)
```

### Comparing `beancount_multitool-0.3.0/src/beancount_multitool/RakutenCard.py` & `beancount_multitool-0.4.0/src/beancount_multitool/RakutenBank.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 import pandas as pd
+from pathlib import Path
+import uuid
 
 from .Institution import Institution
+from .MappingDatabase import MappingDatabase
 from .read_config import read_config
 from .as_transaction import as_transaction
+from .get_value import get_value
+from .get_beancount_config import get_beancount_config
 
 
-class RakutenCard(Institution):
-    NAME = "rakuten_card"  # used in cli.py and in tests
+class RakutenBank(Institution):
+    NAME = "rakuten_bank"  # used in cli.py and in tests
 
     def __init__(self, config_file: str):
         # params
         self.config_file = config_file
-
+        # attributes
         self.config = read_config(config_file)
+        self.beancount_config = get_beancount_config(self.config)
+        # Use basedir of config_file to read mapping database files
+        base_dir = Path(config_file).parent
+        credit_file = get_value(self.config, "database", "credit_mapping")
+        self.credit_file = str(base_dir / credit_file)
+        debit_file = get_value(self.config, "database", "debit_mapping")
+        self.debit_file = str(base_dir / debit_file)
+        self.credit_db = MappingDatabase(self.credit_file)
+        self.debit_db = MappingDatabase(self.debit_file)
 
     def read_transaction(self, file_name: str) -> pd.DataFrame:
         """Read financial transactions into a Pandas DataFrame.
 
         Parameters
         ----------
         file_name : str
             Input file name.
 
         Returns
         -------
         pd.DataFrame
             A dataframe after pre-processing.
         """
-        df = pd.read_csv(file_name)
+        df = pd.read_csv(file_name, encoding="shiftjis")
         print(f"Found {len(df.index)} transactions in {file_name}")
 
         # Rename column names to English.
+        # 取引日,入出金(円),取引後残高(円),入出金内容
+        # Lowercase names will be keyword arguments later.
         column_names = {
-            "利用日": "Date",
-            "利用店名・商品名": "Description",
-            # "利用者": "User",
-            # "支払方法": "Payment method",
-            # "利用金額": "Amount",
-            # "支払手数料": "Commission paid",
-            "支払総額": "Total",
-            # "新規サイン": "New sign",
+            "取引日": "date",
+            "入出金(円)": "amount",
+            "入出金内容": "memo",
+            "取引後残高(円)": "Balance",
         }
         df.rename(columns=column_names, inplace=True)
 
-        df["Date"] = pd.to_datetime(df["Date"], format="%Y/%m/%d")
-
-        # Remove rows with empty 支払総額 cell.
-        # These are extra info such as name of ETC gate or currency exchange rate.
-        # TODO record as metadata
-        extra = df.loc[pd.isnull(df["Total"])]
-        df.drop(extra.index, inplace=True)
-        # Convert to int type because currency is JPY
-        df = df.astype({"Total": int})
-
-        # Remove rows with zero 支払総額. These are refunds.
-        # TODO record as metadata.
-        refund = df.loc[df["Total"] == 0]
-        df.drop(refund.index, inplace=True)
-
-        # Reverse row order because the oldest transaction is on the bottom
-        # Note: the index column is also reversed
-        df = df[::-1]
-
+        # Convert date column to a datetime object
+        df["date"] = pd.to_datetime(df["date"], format="%Y%m%d")
         # print(df.dtypes) # debug
         # print(df) # debug
         return df
 
     def write_bean(self, df: pd.DataFrame, file_name: str) -> None:
         """Write Beancount transactions to file
 
@@ -76,41 +71,51 @@
         file_name : str
             Output file name.
 
         Returns
         -------
         None
         """
-
-        currency = self.config["currency"]
-        source_account = self.config["source_account"]
-        target_account = self.config["default"]["account"]
-        narration = self.config["default"]["narration"]
-        tag = self.config["default"]["tag"]
-        flag = self.config["default"]["flag"]
-
-        with open(file_name, "w", encoding="utf-8") as f:
-            for row in df.index:
-                date = df["Date"][row]
-                amount = df["Total"][row]
-                payee = df["Description"][row]
-                output = as_transaction(
-                    date,
-                    payee,
-                    narration,
-                    tag,
-                    source_account,
-                    target_account,
-                    amount,
-                    currency,
-                    flag,
-                )
-                # print(output) # debug
-                f.write(output)
-            print(f"Written {file_name}")
+        try:
+            with open(file_name, "w", encoding="utf-8") as f:
+                for row in df.index:
+                    date = df["date"][row]
+                    amount = df["amount"][row]
+                    memo = df["memo"][row]
+                    metadata = {"memo": memo}
+
+                    if amount < 0:  # a debit
+                        accounts = self.debit_db.match(memo)
+                    else:  # a credit
+                        accounts = self.credit_db.match(memo)
+
+                    # Add UUID for manual transactions reconcilation between accounts
+                    if "#reconcile" in accounts[0]["tags"]:
+                        if amount > 0:  # a credit
+                            metadata["uuid"] = ""
+                        else:  # a debit
+                            metadata["uuid"] = str(uuid.uuid4())
+
+                    account_metadata = {}
+                    for x in range(1, len(accounts)):
+                        account_metadata[f"match{x+1}"] = str(accounts[x])
+
+                    output = as_transaction(
+                        date=date,
+                        amount=-amount,
+                        metadata=metadata,
+                        account_metadata=account_metadata,
+                        **accounts[0],
+                        **self.beancount_config,
+                    )
+                    # print(output) # debug
+                    f.write(output)
+                print(f"Written {file_name}")
+        except IOError as e:
+            print(e)
 
     def convert(self, csv_file: str, bean_file: str):
         """Convert transactions in a CSV file to a Beancount file
 
         Parameters
         ----------
         csv_file : str
```

### Comparing `beancount_multitool-0.3.0/src/beancount_multitool/as_transaction.py` & `beancount_multitool-0.4.0/src/beancount_multitool/as_transaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,30 +4,37 @@
 
 def as_transaction(
     date: datetime.datetime,
     payee: str,
     narration: str,
     tags: list[str],
     source_account: str,
-    target_account: str,
+    account: str,
     amount: decimal.Decimal,
     currency: str,
-    flag: str = "",
+    flag: str,
+    metadata: dict,
+    account_metadata: dict,
+    **kwargs,
 ) -> str:
     """
     Given transaction details, returns a beancount transaction entry.
 
     Returns
     -------
     str
         A beancount transaction entry:
 
         {date} * "{payee}" "{narration}" {" ".join(tags)}
+          for key, value in metadata:
+            {key}: "{value}"
           {source_account}
-          {flag}{target_account}  {amount} {currency}
+          {flag}{account}  {amount} {currency}
+            for key, value in metadata:
+              {key}: "{value}"
     """
     # Add "#" prefix if does not exist
     hashtags = []
     for x in tags:
         if len(x):
             if x.startswith("#"):
                 hashtags.append(x)
@@ -41,10 +48,12 @@
     # prepare flag
     flag_str = flag.strip()
     if len(flag_str):
         flag_str = flag_str + "  "
 
     output = "\n"
     output += f'{date.strftime("%Y-%m-%d")} * "{payee}" "{narration}"{tags_str}\n'
+    for key, value in metadata.items():
+        output += f'  {key}: "{value}"\n'
     output += f"  {source_account}\n"
-    output += f"  {flag_str}{target_account}  {amount} {currency}\n"
+    output += f"  {flag_str}{account}  {amount} {currency}\n"
     return output
```

### Comparing `beancount_multitool-0.3.0/src/beancount_multitool/cli.py` & `beancount_multitool-0.4.0/src/beancount_multitool/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @click.option(
     "--output",
     default="output.bean",
     type=click.Path(),
     help="Resulting Beancount file",
 )
 @click.version_option()
-def main(name: str, config, data, output):
+def main(name: str, config: str, data: str, output: str):
     """Read financial data and output a Beancount file.
 
     NAME is the name of the financial institution.
     See Note below for a list of supported names.
 
     CONFIG is a .toml file with run-time configurations, e.g. config.toml.
 
@@ -46,12 +46,12 @@
     elif name == RakutenBank.NAME:
         tool = RakutenBank(config)
     elif name == RakutenCard.NAME:
         tool = RakutenCard(config)
     elif name == ShinseiBank.NAME:
         tool = ShinseiBank(config)
 
-    tool.convert(data, output)
+    return tool.convert(data, output)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `beancount_multitool-0.3.0/src/beancount_multitool/read_config.py` & `beancount_multitool-0.4.0/src/beancount_multitool/read_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     try:
         import tomli as tomllib
-    except ImportError:
-        raise ImportError("Is tomli module installed?")
+    except ImportError as e:
+        raise ImportError("Is tomli module installed?") from e
 
 
 def read_config(file_name: str) -> dict:
     """Reads a TOML config file
 
     Parameters
     ----------
@@ -20,10 +20,11 @@
     Returns
     -------
     dict
         TOML file content
     """
     with open(file_name, "rb") as f:
         config = tomllib.load(f)
+        # Exception will be thrown if file not found.
         # print(config) # debug
         # print(type(config)) # debug
         return config
```

### Comparing `beancount_multitool-0.3.0/PKG-INFO` & `beancount_multitool-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-multitool
-Version: 0.3.0
+Version: 0.4.0
 Summary: A CLI tool that converts financial data to Beancount files
 Home-page: https://github.com/rlan/beancount-multitool
 License: MIT
 Author: Rick Lan
 Author-email: rlan@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -22,44 +22,47 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Repository, https://github.com/rlan/beancount-multitool
 Description-Content-Type: text/markdown
 
 # Beancount Multitool
 
 [![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/beancount-multitool)](https://pypi.org/project/beancount-multitool/)
 ![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool)
-![static coverage badge](https://img.shields.io/badge/Coverage-97%25-blue)
+![static coverage badge](https://img.shields.io/badge/Coverage-89%25-blue)
 
 [Beancount Multitool](https://github.com/rlan/beancount-multitool/) is a command-line-interface (CLI) tool that converts financial data from financial institutions to Beancount files.
 
 The following institutions are supported:
 
 * Japan
   * [JA Bank ＪＡネットバンク](https://www.jabank.jp/)
   * [Rakuten Card 楽天カード](https://www.rakuten-card.co.jp/)
   * [Rakuten Bank 楽天銀行](https://www.rakuten-bank.co.jp/)
   * [SBI Shinsei Bank 新生銀行](https://www.sbishinseibank.co.jp/)
 
 What these scripts __can__ do:
 
 * Read raw CSV files downloaded from each institution's website.
-* Label debit and credit transactions to respective account types.
+* Label transactions with different sub-accounts, e.g., `Expenses:JP:Food:Grocery` or `Expenses:JP:Food:Restaurant`.
+  * Documentation is incoming.
+* Label unknown transactions to respective account types.
   * Debit: `Expenses:JP:Unknown:NameOfInstitution`
   * Credit: `Income:JP:Unknown:NameOfInstitution`
 
 What these scripts __can not__ (yet) do:
 
-* Label transactions with different sub-accounts, e.g., `Expenses:JP:Food:Grocery` or `Expenses:JP:Food:Restaurant`.
+* To be added.
 
 Installation:
 
 ```sh
 pip install beancount-multitool
 ```
```

