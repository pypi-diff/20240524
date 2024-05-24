# Comparing `tmp/ng_data_pipelines_sdk-1.5.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.5.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.5.1.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.5.0.tar` & `ng_data_pipelines_sdk-1.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-23 15:32:36.284885 ng_data_pipelines_sdk-1.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 15:32:36.317884 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-23 15:32:36.284885 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-23 15:32:36.284885 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    27572 2024-05-23 15:32:36.284885 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    20557 2024-05-23 15:32:36.284885 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-23 15:32:36.285884 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-23 15:32:36.285884 ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-23 15:32:36.288884 ng_data_pipelines_sdk-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-24 16:35:29.679502 ng_data_pipelines_sdk-1.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 16:35:29.712502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-24 16:35:29.679502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-24 16:35:29.679502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    27736 2024-05-24 16:35:29.680502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    20557 2024-05-24 16:35:29.680502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-24 16:35:29.680502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-24 16:35:29.680502 ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-24 16:35:29.683502 ng_data_pipelines_sdk-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.5.1/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,23 +197,27 @@
             # Convert date partitions to string and add leading zeros because PySpark reads them as integers
             if input_df_params.read_date_params and full_base_path:
                 date_partitions = input_df_params.read_date_params.date_partitions
                 year_col_name = date_partitions.get(DatePartition.YEAR, "year")
                 month_col_name = date_partitions.get(DatePartition.MONTH, "month")
                 day_col_name = date_partitions.get(DatePartition.DAY, "day")
 
-                df = df.withColumn(
-                    year_col_name,
-                    format_string("%04d", df[year_col_name]),
-                ).withColumn(
-                    month_col_name,
-                    format_string("%02d", df[month_col_name]),
-                ).withColumn(
-                    day_col_name,
-                    format_string("%02d", df[day_col_name]),
+                df = (
+                    df.withColumn(
+                        year_col_name,
+                        format_string("%04d", df[year_col_name]),
+                    )
+                    .withColumn(
+                        month_col_name,
+                        format_string("%02d", df[month_col_name]),
+                    )
+                    .withColumn(
+                        day_col_name,
+                        format_string("%02d", df[day_col_name]),
+                    )
                 )
 
         return df
 
     def write_schema(
         self, df: DataFrame, output_df_params: OutputDataFrameParams
     ) -> None:
@@ -310,36 +314,36 @@
         """
         bucket_url = self._get_bucket_url(output_df_params.dataframe_bucket_params)
         write_base_path_url = f"{bucket_url}/{output_df_params.dataframe_base_path}"
         logger.debug(f"Write base path: {write_base_path_url}")
 
         df_to_write = df
         if output_df_params.single_write_date:
-            # Add the date partitions columns to the DataFrame
             date_partition_path = ""
             for (
                 date_partition,
                 date_partition_name,
             ) in (
                 output_df_params.single_write_date.single_write_date_partitions.items()
             ):
-                date_partition_path += f"{date_partition_name}={date_partition.value}/"
-
                 formatted_date_part_value = DATE_FORMATTER[date_partition.value](
                     output_df_params.single_write_date.single_write_date
                 )
-
+                # Add the date partition column to the DataFrame
                 df_to_write = df_to_write.withColumn(
                     date_partition_name, lit(formatted_date_part_value)
                 )
+                date_partition_path += (
+                    f"{date_partition_name}={formatted_date_part_value}/"
+                )
 
             if output_df_params.overwrite:
                 full_path = f"{write_base_path_url}/{date_partition_path}"
                 logger.info(
-                    f"Overwrite is set to True. Deleting existing objects under path {full_path}"
+                    f"Overwrite is set to True. Deleting existing objects under path x{full_path}"
                 )
                 try:
                     self.aws_interface.delete_objects_aws(
                         env=output_df_params.dataframe_bucket_params.env,
                         bucket_name=output_df_params.dataframe_bucket_params.bucket_name,
                         path=f"{output_df_params.dataframe_base_path}/{date_partition_path}",
                     )
```

### Comparing `ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.5.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.5.1/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.5.0/pyproject.toml` & `ng_data_pipelines_sdk-1.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.5.0"
+version = "1.5.1"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.5.0/PKG-INFO` & `ng_data_pipelines_sdk-1.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.5.0
+Version: 1.5.1
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

