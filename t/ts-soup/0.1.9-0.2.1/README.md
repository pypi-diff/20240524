# Comparing `tmp/ts_soup-0.1.9.tar.gz` & `tmp/ts_soup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-_y0zjito\ts_soup-0.1.9.tar", last modified: Tue Apr 16 04:44:53 2024, max compression
+gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-q5p_zyxf\ts_soup-0.2.1.tar", last modified: Fri May 24 01:48:54 2024, max compression
```

## Comparing `ts_soup-0.1.9.tar` & `ts_soup-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.097109 ts_soup-0.1.9/
--rw-rw-rw-   0        0        0     1028 2024-04-16 04:44:53.096108 ts_soup-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts_soup-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 04:44:53.097109 ts_soup-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-16 04:44:43.000000 ts_soup-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.082282 ts_soup-0.1.9/ts_soup/
--rw-rw-rw-   0        0        0      373 2024-04-09 03:17:12.000000 ts_soup-0.1.9/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts_soup-0.1.9/ts_soup/app.py
--rw-rw-rw-   0        0        0    15395 2024-04-16 04:44:23.000000 ts_soup-0.1.9/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.093267 ts_soup-0.1.9/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts_soup-0.1.9/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-11 09:09:47.000000 ts_soup-0.1.9/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5595 2024-04-16 04:43:29.000000 ts_soup-0.1.9/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.094268 ts_soup-0.1.9/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 01:48:54.437238 ts_soup-0.2.1/
+-rw-rw-rw-   0        0        0     1028 2024-05-24 01:48:54.435233 ts_soup-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts_soup-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 01:48:54.437238 ts_soup-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-05-24 01:48:38.000000 ts_soup-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:48:54.420120 ts_soup-0.2.1/ts_soup/
+-rw-rw-rw-   0        0        0      373 2024-04-09 03:17:12.000000 ts_soup-0.2.1/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts_soup-0.2.1/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15453 2024-05-24 01:48:17.000000 ts_soup-0.2.1/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:48:54.432225 ts_soup-0.2.1/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts_soup-0.2.1/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     4265 2024-04-18 04:38:01.000000 ts_soup-0.2.1/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5931 2024-04-17 04:46:34.000000 ts_soup-0.2.1/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:48:54.434229 ts_soup-0.2.1/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-05-24 01:48:54.000000 ts_soup-0.2.1/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-24 01:48:54.000000 ts_soup-0.2.1/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 01:48:54.000000 ts_soup-0.2.1/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 01:48:54.000000 ts_soup-0.2.1/ts_soup.egg-info/top_level.txt
```

### Comparing `ts_soup-0.1.9/PKG-INFO` & `ts_soup-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.9
+Version: 0.2.1
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts_soup-0.1.9/README.md` & `ts_soup-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.9/setup.py` & `ts_soup-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.1.9",
+  version="0.2.1",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts_soup-0.1.9/ts_soup/app.py` & `ts_soup-0.2.1/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.9/ts_soup/common.py` & `ts_soup-0.2.1/ts_soup/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,32 +24,25 @@
 DATA_UPDATED_STATE = None
 
 
 def query_in_sql(list_):
     return ','.join(list(map(lambda x: '"' + x + '"', list_)))
 
 
-def get_sqlalchemy_engine(db_info, db_type):
+def get_sqlalchemy_engine(db_info, db_type,engine_index):
     global USABLE_DBS
-    engine = create_engine(
-        f'mysql+pymysql://{db_info["user"]}:{parse.quote_plus(db_info["pwd"])}@{db_info["ip"]}:3306/{db_info["db"]}')
+    engine = db_info['engine'][engine_index]
     USABLE_DBS[db_info['alias']] = engine
     if db_info['default']:
         USABLE_DBS[f'{db_type}_default'] = engine
 
 
-def get_pymsql_engine(db_info, db_type):
+def get_pymsql_engine(db_info, db_type,engine_index):
     global USABLE_DBS
-    engine = pymysql.connect(
-        host=db_info['ip'],
-        user=db_info['user'],
-        password=db_info['pwd'],
-        port=int(db_info['port']),
-        database=db_info['db']
-    )
+    engine = db_info['engine'][engine_index]
     USABLE_DBS[db_info['alias'] + '_pym'] = engine
     if db_info['default']:
         USABLE_DBS[f'{db_type}_default_pym'] = engine
 
 
 def __init(customized_table, customized_time, sync_start, sync_end, db_infos):
     """
@@ -77,19 +70,19 @@
     global DATA_UPDATED_STATE, SYNC_FROM_DATE, CURRENT_DATE, USABLE_DBS
 
     for db_type in ['sources', 'targets']:  # 加载数据源配置 设置数据库连接
         for db_info in db_infos[db_type]:
             engine_types = db_info.get('engine_type')
 
             if engine_types:
-                for engine_type in engine_types:
+                for engine_index,engine_type in enumerate(engine_types):
                     if engine_type == 'sqlalchemy':
-                        get_sqlalchemy_engine(db_info, db_type)
+                        get_sqlalchemy_engine(db_info, db_type,engine_index)
                     else:
-                        get_pymsql_engine(db_info, db_type)
+                        get_pymsql_engine(db_info, db_type,engine_index)
 
             else:
                 raise ValueError('未配置engine类型')
 
     SYNC_FROM_DATE = sync_start
     CURRENT_DATE = sync_end
     to_update_tables = pd.read_sql('select * from to_update_tables', con=USABLE_DBS['targets_default'])['table_name']
@@ -314,27 +307,31 @@
             try:
                 executor = Executor(targets=targets,
                                     sources=sources,
                                     executed_table=func.__name__)
 
                 # 表示该方法已同步完所有数据，则不再执行后续操作
                 if len(executor.to_update_date) == 0:
-                    print(f'{func.__name__} 方法已同步至最新')
+                    print(f'{func.__name__} 方法已同步至最新\n\n')
                     return
 
-                print('>' * 20 + f' {func.__name__} 开始' + '>' * 20)
+                msg_len = len(f' {func.__name__} 开始 ')
+                before_white_len = int((110-msg_len)/2)
+                after_white_len = 110-msg_len-before_white_len
+
+                print('>'*before_white_len + f' {func.__name__} 开始 ' +'>'*after_white_len)
                 if len(sources) != 0:
                     executor.make_source_data()
 
                 # empty_check为True且有一天数据源为空则不执行数据处理函数
                 if not executor.any_source_empty:
                     func(executor)
 
                 executor.handle_result()
-                print('<' * 20 + f' {func.__name__} 结束' + '<' * 20)
+                print('<'*before_white_len+ f' {func.__name__} 结束 '+'<'*after_white_len+'\n'*2)
             except Exception:
                 global EXECUTE_STATE
                 EXECUTE_STATE = False
                 print(executor.executed_table + '同步失败')
                 print(traceback.format_exc())
 
         return inner_wrapper
```

### Comparing `ts_soup-0.1.9/ts_soup/workers/sources.py` & `ts_soup-0.2.1/ts_soup/workers/sources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,66 @@
 import pandas as pd
-from ts_soup.common import query_in_sql,BaseSource
+from ts_soup.common import query_in_sql, BaseSource
 
 
 class Source(BaseSource):
     def __init__(self,
                  tb: str,
                  db: str = None,
                  empty_check=True,
                  query_field: str = '*',
                  index_field='date',
-                 other_condition: str = None):
+                 other_condition: str = None,
+                 order_index: list = None,
+                 order_desc: bool = False
+                 ):
         """
         单表查询数据源信息
         :param tb: 数据表名
         :param db: 数据库名
         :param query_field:要查询的字段，默认为 *
         :param index_field: 日期字段，如果不提供则默认"date",如果需要查询全表，则index_field需要设置为 None。
         :param other_condition: 其他查询条件，直接拼接到 from table 后，覆盖date_field
         :param empty_check: 是否为当前方法主要数据源（除了配置信息的数据源），判空时使用，若不想使当前数据源参与判空，可设为 False
         """
         super().__init__(db, index_field, empty_check)
         self.tb = tb
         self.query_field = query_field
         self.other_condition = other_condition
-
+        self.order_index = order_index
+        self.order_desc = order_desc
 
     def build_source(self, to_update_date):
         base_sql = f'select {self.query_field} from {self.tb} where 1=1 '
         if self.other_condition:
             base_sql += f' and {self.other_condition} '
         if self.index_field:
-            base_sql += f' and {self.index_field} in ({query_in_sql(to_update_date.values.tolist())}) order by {self.index_field}'
+            base_sql += f' and {self.index_field} in ({query_in_sql(to_update_date.values.tolist())})'
+
+        # 处理排序
+        if self.order_index is not None:
+            base_sql += f' order by {",".join(self.order_index)}'
+            if self.order_desc:
+                base_sql += ' desc'
+        elif self.index_field:
+            base_sql += f' order by {self.index_field}'
+            if self.order_desc:
+                base_sql += ' desc'
+
         return pd.read_sql(base_sql, con=self.db)
 
 
 class MultiSource(BaseSource):
     """
     多数据源联合查询时使用
     """
+
     def __init__(self,
                  relations: list,
-                 db: str=None ,
+                 db: str = None,
                  empty_check=True,
                  index_field='date'):
         """
         :param relations:连接条件模板如下：
         {'left':'','right':'','l_on':'','r_on':'','how':'','lquery_field':'','rquery_field':' ','l_cons':'','r_cons':''},
         :param db:
         :param empty_check:
@@ -53,30 +69,33 @@
         super().__init__(db, index_field, empty_check)
         self.relations = relations
 
     def build_source(self, to_update_date):
         query_params = []
         join_stm = ''
         where_clause = ''
-        for index,rel in enumerate(self.relations):
-            query_params.append(','.join([f'{rel["left"]}.'+i if i!='' else '' for i in rel['lquery_field'].split(',')])\
-                            +(',' if rel['lquery_field']!='' else '')+\
-                            ','.join([f'{rel["right"]}.'+i if i!='' else '' for i in rel['rquery_field'].split(',')]))
-            join_stm+=f"{rel['how']} join {rel['right']} on {rel['left']}.{rel['l_on']}={rel['right']}.{rel['r_on']} "
-            where_clause += (f" and {rel['left']+'.'+rel['l_cons']}" if rel['l_cons']!='' else '')+(f"and {rel['right']+'.'+rel['r_cons']}" if rel['r_cons']!='' else '')
+        for index, rel in enumerate(self.relations):
+            query_params.append(
+                ','.join([f'{rel["left"]}.' + i if i != '' else '' for i in rel['lquery_field'].split(',')]) \
+                + (',' if rel['lquery_field'] != '' else '') + \
+                ','.join([f'{rel["right"]}.' + i if i != '' else '' for i in rel['rquery_field'].split(',')]))
+            join_stm += f"{rel['how']} join {rel['right']} on {rel['left']}.{rel['l_on']}={rel['right']}.{rel['r_on']} "
+            where_clause += (f" and {rel['left'] + '.' + rel['l_cons']}" if rel['l_cons'] != '' else '') + (
+                f"and {rel['right'] + '.' + rel['r_cons']}" if rel['r_cons'] != '' else '')
         base_sql = f'select {",".join(query_params)} from {self.relations[0]["left"]} {join_stm} where 1=1 {where_clause} and {self.index_field} in ({query_in_sql(to_update_date)})'
-        return pd.read_sql(base_sql,con=self.db)
+        return pd.read_sql(base_sql, con=self.db)
 
 
 class RawSqlSource(BaseSource):
-    def __init__(self,  index_field,sql,db:str=None, empty_check=True):
+    def __init__(self, index_field, sql, db: str = None, empty_check=True):
         """
         直接使用sql的源
         :param db:
         :param index_field:
         :param empty_check:
         :param sql:
         """
         super().__init__(db, index_field, empty_check)
         self.sql = sql
+
     def build_source(self, to_update_date):
-        return pd.read_sql(self.sql.format(query_in_sql(to_update_date)),con=self.db)
+        return pd.read_sql(self.sql.format(query_in_sql(to_update_date)), con=self.db)
```

### Comparing `ts_soup-0.1.9/ts_soup/workers/targets.py` & `ts_soup-0.2.1/ts_soup/workers/targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,21 +52,23 @@
         if str(cur_result[self.index_field].dtypes) == 'datetime64' or str(
                 cur_result[self.index_field].dtypes).lower() == 'object':
             cur_result[self.index_field] = pd.to_datetime(cur_result[self.index_field]).apply(
                 lambda x: x.strftime('%Y-%m-%d'))
 
         self.__execute_sql(cur_result)
 
-        """如果是多个数据源合并到一个表，多个字段有若干个为空，或者一个日期内多行为空，
+        """如果是多个数据源合并到一个表，多个字段有若干个为空，或者一个日期内多行内有字段为空，
         则需要在插入前删除为空的字段的日期，保证下次执行还能同步该日期
+        可以通过 drop_na_subset,drop_na_thresh 参数控制是否执行该步骤，若是因此而被删除的日期，
+        在同步日志中会有 "因数据不全(多个字段有至少一个字段为Null)导致update_state当天日期未更新" 提示
         # e.g  
-        index       b   c   d
-        2023-01     na  2   3
-        2023-01     1   2   3
-        2023-02     1   3   4
+        pdate       period  value1  value2   
+        2023-01     1       2       na
+        2023-01     1       na      3
+        2023-02     1       3       4
         2023-01日期有Na，则不作为更新完成的日期
         """
         params = {'axis': self.drop_axis}
         if self.drop_na_subset:
             params['subset'] = self.drop_na_subset
         if self.drop_na_thresh:
             params['thresh'] = self.drop_na_thresh
@@ -106,11 +108,11 @@
                 import traceback
                 print(traceback.format_exc())
                 self.db_pym.rollback()
                 raise Exception('数据库操作错误!')
         else:
             with self.db.begin() as conn:
                 conn.execute(
-                    f'delete from {self.tb} where {self.index_field} in ({query_in_sql(cur_result[self.index_field].values.tolist())})')
+                    f'delete from {self.tb} where {self.index_field} in ({query_in_sql(cur_result[self.index_field].drop_duplicates().values.tolist())})')
                 cur_result.to_sql(self.tb, con=conn, if_exists='append', index=False)
         print(
             f'{self.tb} 更新成功，更新日期为：\n{",".join(cur_result[self.index_field].drop_duplicates().sort_values(ascending=False).values.tolist())}')
```

### Comparing `ts_soup-0.1.9/ts_soup.egg-info/PKG-INFO` & `ts_soup-0.2.1/ts_soup.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.9
+Version: 0.2.1
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

