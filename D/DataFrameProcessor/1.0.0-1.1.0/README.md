# Comparing `tmp/DataFrameProcessor-1.0.0-py3-none-any.whl.zip` & `tmp/DataFrameProcessor-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8849 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      376 b- defN 24-May-23 17:28 my_library/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-May-23 15:37 my_library/categorical_encoder.py
--rw-rw-rw-  2.0 fat     1706 b- defN 24-May-23 17:34 my_library/date_time_handler.py
--rw-rw-rw-  2.0 fat     5166 b- defN 24-May-23 16:06 my_library/feature_engineer.py
--rw-rw-rw-  2.0 fat     3826 b- defN 24-May-23 15:06 my_library/missing_value_handler.py
--rw-rw-rw-  2.0 fat     4420 b- defN 24-May-23 15:45 my_library/outlier_handler.py
--rw-rw-rw-  2.0 fat     6908 b- defN 24-May-22 18:02 my_library/scaler.py
--rw-rw-rw-  2.0 fat     3240 b- defN 24-May-23 15:54 my_library/search.py
--rw-rw-rw-  2.0 fat     5160 b- defN 24-May-22 17:09 my_library/text_cleaner.py
--rw-rw-rw-  2.0 fat      112 b- defN 24-May-23 18:00 DataFrameProcessor-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 18:00 DataFrameProcessor-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-23 18:00 DataFrameProcessor-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1099 b- defN 24-May-23 18:00 DataFrameProcessor-1.0.0.dist-info/RECORD
-13 files, 33201 bytes uncompressed, 7003 bytes compressed:  78.9%
+Zip file size: 8958 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      376 b- defN 24-May-23 17:28 DataFrameProcessor/__init__.py
+-rw-rw-rw-  2.0 fat     1065 b- defN 24-May-23 18:22 DataFrameProcessor/categorical_encoder.py
+-rw-rw-rw-  2.0 fat     1686 b- defN 24-May-23 18:22 DataFrameProcessor/date_time_handler.py
+-rw-rw-rw-  2.0 fat     5146 b- defN 24-May-23 18:22 DataFrameProcessor/feature_engineer.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 24-May-23 18:21 DataFrameProcessor/missing_value_handler.py
+-rw-rw-rw-  2.0 fat     4387 b- defN 24-May-23 18:22 DataFrameProcessor/outlier_handler.py
+-rw-rw-rw-  2.0 fat     6908 b- defN 24-May-22 18:02 DataFrameProcessor/scaler.py
+-rw-rw-rw-  2.0 fat     3220 b- defN 24-May-23 18:22 DataFrameProcessor/search.py
+-rw-rw-rw-  2.0 fat     5145 b- defN 24-May-23 18:22 DataFrameProcessor/text_cleaner.py
+-rw-rw-rw-  2.0 fat      186 b- defN 24-May-24 09:20 DataFrameProcessor-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 09:20 DataFrameProcessor-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 24-May-24 09:20 DataFrameProcessor-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1171 b- defN 24-May-24 09:20 DataFrameProcessor-1.1.0.dist-info/RECORD
+13 files, 33207 bytes uncompressed, 6968 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -1,40 +1,40 @@
-Filename: my_library/__init__.py
+Filename: DataFrameProcessor/__init__.py
 Comment: 
 
-Filename: my_library/categorical_encoder.py
+Filename: DataFrameProcessor/categorical_encoder.py
 Comment: 
 
-Filename: my_library/date_time_handler.py
+Filename: DataFrameProcessor/date_time_handler.py
 Comment: 
 
-Filename: my_library/feature_engineer.py
+Filename: DataFrameProcessor/feature_engineer.py
 Comment: 
 
-Filename: my_library/missing_value_handler.py
+Filename: DataFrameProcessor/missing_value_handler.py
 Comment: 
 
-Filename: my_library/outlier_handler.py
+Filename: DataFrameProcessor/outlier_handler.py
 Comment: 
 
-Filename: my_library/scaler.py
+Filename: DataFrameProcessor/scaler.py
 Comment: 
 
-Filename: my_library/search.py
+Filename: DataFrameProcessor/search.py
 Comment: 
 
-Filename: my_library/text_cleaner.py
+Filename: DataFrameProcessor/text_cleaner.py
 Comment: 
 
-Filename: DataFrameProcessor-1.0.0.dist-info/METADATA
+Filename: DataFrameProcessor-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: DataFrameProcessor-1.0.0.dist-info/WHEEL
+Filename: DataFrameProcessor-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: DataFrameProcessor-1.0.0.dist-info/top_level.txt
+Filename: DataFrameProcessor-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: DataFrameProcessor-1.0.0.dist-info/RECORD
+Filename: DataFrameProcessor-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `my_library/categorical_encoder.py` & `DataFrameProcessor/categorical_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import numpy as np
 from sklearn.preprocessing import LabelEncoder   
 
 class CategoricalEncoder:
     @staticmethod
     def hot_encode(dataframe, columns):
         """
         One-hot encode categorical columns in a DataFrame.
```

## Comparing `my_library/date_time_handler.py` & `DataFrameProcessor/date_time_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import numpy as np
 from datetime import datetime
 
 
 class DateTimeHandeler:
     @staticmethod
     def calculate_years_passed(dataframe, column):
         """
```

## Comparing `my_library/feature_engineer.py` & `DataFrameProcessor/feature_engineer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import numpy as np
 
 class FeatureEngineer:
     @staticmethod
     def create_interaction_features(dataframe, new_faeture_name , feature1, feature2 , replace = False):
         """
         Create interaction features by multiplying two specified numeric features element-wise.
```

## Comparing `my_library/missing_value_handler.py` & `DataFrameProcessor/missing_value_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd 
-import numpy as np
 from .outlier_handler import OutlierHandler as oh
 import math
 
 class MissingValueHandler:
     @staticmethod
     def impute_mean(dataframe, column):
         """
```

## Comparing `my_library/outlier_handler.py` & `DataFrameProcessor/outlier_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import pandas as pd 
-import numpy as np
-import math
 
 class OutlierHandler:
     @staticmethod
     def get_bounds(df, column):
         """
         Calculate the lower and upper bounds for outliers in a numeric column using the IQR method.
```

## Comparing `my_library/scaler.py` & `DataFrameProcessor/scaler.py`

 * *Files identical despite different names*

## Comparing `my_library/search.py` & `DataFrameProcessor/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import numpy as np
 
 class Search:
     @staticmethod
     def search_value(dataframe, value, column=None):
         """
         Search for rows that contain the specified value in any column or in a specified column.
```

## Comparing `my_library/text_cleaner.py` & `DataFrameProcessor/text_cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import string
 from nltk.corpus import stopwords
 
 
 class TextCleaner:
 
     @staticmethod
     def to_lowercase(dataframe, column):
```

