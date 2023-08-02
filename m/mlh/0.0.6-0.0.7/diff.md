# Comparing `tmp/mlh-0.0.6.tar.gz` & `tmp/mlh-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlh-0.0.6.tar", last modified: Mon Jul 31 18:18:54 2023, max compression
+gzip compressed data, was "mlh-0.0.7.tar", last modified: Wed Aug  2 07:39:09 2023, max compression
```

## Comparing `mlh-0.0.6.tar` & `mlh-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:18:54.059581 mlh-0.0.6/
--rw-rw-rw-   0        0        0     3157 2023-07-31 18:18:54.059581 mlh-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2023-07-31 16:46:11.000000 mlh-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 18:18:54.043564 mlh-0.0.6/mlh/
--rw-rw-rw-   0        0        0     1278 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/__init__.py
--rw-rw-rw-   0        0        0     5896 2023-07-31 17:59:45.000000 mlh-0.0.6/mlh/common_utils.py
--rw-rw-rw-   0        0        0     2747 2023-07-31 17:59:43.000000 mlh-0.0.6/mlh/data_from_parquet.py
--rw-rw-rw-   0        0        0     5936 2023-07-31 17:59:41.000000 mlh-0.0.6/mlh/s3_connect.py
--rw-rw-rw-   0        0        0    13560 2023-07-31 17:59:38.000000 mlh-0.0.6/mlh/snowflake_connect.py
--rw-rw-rw-   0        0        0     9666 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/sqlite_functions.py
--rw-rw-rw-   0        0        0    16876 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/support.py
--rw-rw-rw-   0        0        0    21008 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/woe.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:18:54.059581 mlh-0.0.6/mlh.egg-info/
--rw-rw-rw-   0        0        0     3157 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 18:18:54.059581 mlh-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-07-31 18:17:09.000000 mlh-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:39:09.351399 mlh-0.0.7/
+-rw-rw-rw-   0        0        0     3157 2023-08-02 07:39:09.351399 mlh-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 07:39:09.335875 mlh-0.0.7/mlh/
+-rw-rw-rw-   0        0        0      269 2023-08-02 06:21:43.000000 mlh-0.0.7/mlh/__init__.py
+-rw-rw-rw-   0        0        0     6950 2023-08-02 06:50:30.000000 mlh-0.0.7/mlh/common_utils.py
+-rw-rw-rw-   0        0        0     2747 2023-08-02 05:28:22.000000 mlh-0.0.7/mlh/data_from_parquet.py
+-rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.0.7/mlh/s3_connect.py
+-rw-rw-rw-   0        0        0    13566 2023-08-02 06:25:41.000000 mlh-0.0.7/mlh/snowflake_connect.py
+-rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.0.7/mlh/sqlite_functions.py
+-rw-rw-rw-   0        0        0    15840 2023-08-02 06:55:50.000000 mlh-0.0.7/mlh/support.py
+-rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.0.7/mlh/woe.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:39:09.351399 mlh-0.0.7/mlh.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:39:09.351399 mlh-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-08-02 07:02:25.000000 mlh-0.0.7/setup.py
```

### Comparing `mlh-0.0.6/PKG-INFO` & `mlh-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.0.6/README.md` & `mlh-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mlh-0.0.6/mlh/common_utils.py` & `mlh-0.0.7/mlh/common_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import pandas as pd
 import dateutil
 from dateutil.relativedelta import relativedelta
 import calendar
 from datetime import datetime
+from openpyxl import load_workbook
 
 class common_utils:
     # !/usr/bin/env python
     # -*- coding: utf-8 -*-
     # Author: Devendra Kumar Sahu
     # Email: devsahu99@gmail.com
     # Sqliite DB related tasks
@@ -112,15 +113,15 @@
             cmf = common_utils()
             cmf.Get_Last_N_Quarter_Dates('202310', n=5)
         ------------------------------------------------------------    
         """
         dt = self.getLastNQuarters(quarterNG, n)
         return [self.Get_Quarter_End_Date(x) for x in pd.to_datetime(pd.Series(dt))]
 
-    def Date_to_Quarter_Start_Date(self, InputDate):
+    def Date_To_Quarter_Start_Date(self, InputDate):
         """
         This function returns any date to its quarter start date. Helpful in cases where quarterly trends are required
 
         ------------------------------------------------------------
         Parameters:
         InputDate: Datetime
             input date to be converted
@@ -141,7 +142,32 @@
 
         except Exception as ex:
             sys.stdout = open("log.txt", "w")
             print(datetime.now().replace(microsecond=0), " Date conversion to Quarter failed - exiting run")
             print(datetime.now().replace(microsecond=0), ex)
             sys.exit()
         return None
+
+    def Write_To_Excel(self, df, workbook, sheet_name='Sheet1'):
+        """
+        This utility helps in saving the output into excel file worksheets.
+
+        Parameters:
+        ------------------------------------------------------------
+        df: Pandas Dataframe
+            The reference to pandas dataframe
+        workbook: Excel Path
+            Reference to excel workbook
+        sheet_name: String
+            name of the worksheet in which the dataframe should be saved. Default is 'Sheet1'
+        """
+        try:
+            book = load_workbook(workbook)
+            writer = pd.ExcelWriter(workbook, engine = 'openpyxl')
+            writer.book = book
+            writer.sheets = dict((ws.title, ws) for ws in book.worksheets)  
+            df.to_excel(writer, sheet_name = sheet_name, index=False)
+        except:
+            writer = pd.ExcelWriter(workbook, engine = 'openpyxl')
+            df.to_excel(writer, sheet_name = sheet_name, index=False)
+        writer.save()
+        writer.close()
```

### Comparing `mlh-0.0.6/mlh/data_from_parquet.py` & `mlh-0.0.7/mlh/data_from_parquet.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.6/mlh/s3_connect.py` & `mlh-0.0.7/mlh/s3_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.6/mlh/snowflake_connect.py` & `mlh-0.0.7/mlh/snowflake_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     
     def __checkDBTables(self, cursor, tablename):
         stmt = "SHOW TABLES LIKE '%s' "% ('%'+str(tablename)+'%')
         cursor.execute(stmt)
         result = cursor.fetchone()
         return result
 
-    def getAllSFTablesList(self, d_params=None):
+    def Fetch_All_Table_Names(self, d_params=None):
         """
         This Function returns the list of tables in the database schema
         
         Parameters:
         ------------------------------------------------------------
         d_params: Dict, optional
             Default, None. It is required if configuration information is not provided during initial function call. The below mentioned keys should be provided in the dictionary format
@@ -250,15 +250,15 @@
         
         """
         ctx = self.__Connect_To_Snowflake(d_params)
         all_tables = ctx.cursor().execute("show tables")
         ctx.close()
         return [x[1] for x in all_tables]
 
-    def dropSFTablesList(self, tables_list, d_params=None):
+    def Drop_Tables_From_DB(self, tables_list, d_params=None):
         """
         This Function drops the mentioned tables from the snowflake database
         
         Parameters:
         ------------------------------------------------------------
         tables_list: List
             list of table names to be dropped
```

### Comparing `mlh-0.0.6/mlh/sqlite_functions.py` & `mlh-0.0.7/mlh/sqlite_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     ------------------------------------------------------------
     Approach:
 
     1. Create an instance of SQL function
          mysql = sqlite_functions(db_path)
 
     2. Call table creation function
-         mysql.create_db_table(db_table_schema)
+         mysql.Create_DB_Table(db_table_schema)
 
     3. Insert values to the created table
-        mysql.insert_values_to_table(df, table_name)
+        mysql.Insert_Values_To_Table(df, table_name)
     
     4. Extract saved data
-        mysql.db_extract_records(query)
+        mysql.Extract_DB_Records(query)
         
     ------------------------------------------------------------    
     """
     def __init__(self, db_path):
         self.__db_path = db_path
         
     def __connect_to_db(self):
@@ -51,15 +51,15 @@
             return sqlite3_conn
         except sqlite3.Error as err:
             print(f"Error in Connection: {err}")
             if sqlite3_conn is not None:
                 sqlite3_conn.close()
         return None
     
-    def create_db_table(self, tablemaps):
+    def Create_DB_Table(self, tablemaps):
         """
         This Function creates database table.
         
         Parameters:
         ------------------------------------------------------------
         tablemaps: string
             Database table definition
@@ -67,96 +67,96 @@
         Returns:
         An empty table is created in the database file
         
         Example:
         
         mysql = sqlite_functions(db_path)
         table_schema = 'users(USERID INTEGER, USER_NAME TXT, LAST_NAME TXT, ENTER_DATE REAL)'
-        mysql.create_db_table(table_schema)
+        mysql.Create_DB_Table(table_schema)
         """
         conn = self.__connect_to_db()
         if conn is not None:
             conn.execute("CREATE TABLE IF NOT EXISTS "  + tablemaps)
             print("Table Created")
             conn.close()
             return None
         print("Table Not Created!")
         conn.close()
         return None
     
-    def drop_db_table(self, table_name):
+    def Drop_DB_Table(self, table_name):
         """
         This Function drops the created database table.
         
         Parameters:
         ------------------------------------------------------------
         table_name: string
             Database table name
         ------------------------------------------------------------
         Returns:
         None
         
         Example:
         
         mysql = sqlite_functions(db_path)
-        mysql.drop_db_table('users')
+        mysql.Drop_DB_Table('users')
         """
         conn = self.__connect_to_db()
         try:
             conn.execute("DROP TABLE "+ table_name)
             conn.close()
             print(f"{table_name} Deleted")
         except sqlite3.Error as err:
             conn.close()
             print(f"Can Not Delete {table_name} due to:- {err}")
         return None
     
-    def db_delete_records(self, query, args=[]):
+    def Delete_DB_Records(self, query, args=[]):
         """
         This Function delete certain records from the database table.
         
         Parameters:
         ------------------------------------------------------------
         query: string
             Database query string
         ------------------------------------------------------------
         Returns:
         None
         
         Example:
         
         query = 'DELETE FROM USERS where USERID>=5'
-        mysql.db_delete_records(query)
+        mysql.Delete_DB_Records(query)
         """
         conn = self.__connect_to_db()
         try:
             qury_result = conn.execute(query,args)
             conn.commit()
             conn.close()
             return None
         except sqlite3.Error as err:
             print(f"Cannot delete records for {query} due to:- {err}")
         return None
     
-    def db_extract_records(self, query, args=[]):
+    def Extract_DB_Records(self, query, args=[]):
         """
         This Function queries the database table and return the results into a pandas dataframe.
         
         Parameters:
         ------------------------------------------------------------
         query: string
             Database query string
         ------------------------------------------------------------
         Returns:
         Pandas dataframe
         
         Example:
         
         query = 'select * from USERS where USERID>=2'
-        mysql.db_extract_records(query)
+        mysql.Extract_DB_Records(query)
         """
         conn = self.__connect_to_db()
         try:
             qury_result = conn.execute(query,args)
             if str(qury_result.description)=='None':
                 conn.close()
                 return None
@@ -173,15 +173,15 @@
         sql_cursor.execute(table_column_names)
         table_column_names = sql_cursor.fetchall()
         column_names = list()
         for name in table_column_names:
             column_names.append(name[1])
         return column_names
     
-    def insert_values_to_table(self, df, table_name):
+    def Insert_Values_To_Table(self, df, table_name):
         """
         This Function inserts records to the database table.
         
         Parameters:
         ------------------------------------------------------------
         df: Pandas dataframe
             Pandas dataframe to be inserted into the database table
@@ -189,15 +189,15 @@
             Table name to which the data should be inserted
         ------------------------------------------------------------
         
         Returns:
         None
         
         Example:
-        mysql.insert_values_to_table(df, 'USERS')
+        mysql.Insert_Values_To_Table(df, 'USERS')
         """
         conn = self.__connect_to_db()
         if conn is not None:
             cur = conn.cursor()
 
             db_columns = self.__get_column_names_from_db_table(cur, table_name)
             try:
@@ -207,15 +207,15 @@
                 print(f'Value Insersion Failed due to {err}')
             finally:
                 conn.close()   
         else:
             print('Connection to database failed')
         return None
     
-    def insert_unique_to_table(self, df, table_name):
+    def Insert_Unique_To_Table(self, df, table_name):
         """
         This Function inserts unique records to the database table.
         
         Parameters:
         ------------------------------------------------------------
         df: Pandas dataframe
             Pandas dataframe to be inserted into the database table
@@ -223,15 +223,15 @@
             Table name to which the data should be inserted
         ------------------------------------------------------------
         
         Returns:
         None
         
         Example:
-        mysql.insert_unique_to_table(df, 'USERS')
+        mysql.Insert_Unique_To_Table(df, 'USERS')
         """
         conn = self.__connect_to_db()
         if conn is not None:
             cur = conn.cursor()
             db_columns = self.__get_column_names_from_db_table(cur, table_name)
             for i in range(len(df)):
                 try:
@@ -239,15 +239,15 @@
                 except sqlite3.Error as err:
                     pass #or any other action
             conn.close()
         else:
             print('Connection to database failed')
         return None
     
-    def killSqlCon(self):
+    def Kill_Sql_Connection(self):
         """
         This Function kills the sql connection.
 
         ------------------------------------------------------------
         """
         sqlite3_conn = None
         try:
@@ -255,15 +255,15 @@
         except sqlite3.Error as err:
             print(err)
             if sqlite3_conn is not None:
                 pass
         sqlite3_conn.close()
         return 'Connection Closed'
 
-    def pandas_to_sql_query(self, df, tableName):
+    def Pandas_To_Sql_Query(self, df, tableName):
         """
         This Function converts the dataframe to sql queries schema for creating SQL table schema
         
         Parameters:
         ------------------------------------------------------------
         df: Pandas dataframe
             
@@ -272,14 +272,14 @@
         ------------------------------------------------------------
         
         Returns:
         Querystring which can be used for creating data table schema
         
         Example:
         
-        mysql.pandas_to_sql_query(df, 'USERS')
+        mysql.Pandas_To_Sql_Query(df, 'USERS')
         
         """
         df_dict = df.dtypes.to_dict()
         dtypeDict = {'object':' TEXT','float64':' REAL'}
         clintop_data_keys = [x+dtypeDict[str(df_dict[x])] for x in df_dict.keys()]
         return f"""{tableName.strip()}({','.join(clintop_data_keys)})"""
```

### Comparing `mlh-0.0.6/mlh/support.py` & `mlh-0.0.7/mlh/support.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pandas import Series
 import numpy as np
 import random
 from IPython.display import display, HTML, Markdown
 import matplotlib.pyplot as plt
 from sklearn.model_selection import GridSearchCV, StratifiedKFold, RandomizedSearchCV, train_test_split
 from sklearn.metrics import accuracy_score,classification_report,confusion_matrix,roc_curve,auc,precision_recall_curve,make_scorer,recall_score,precision_score
-from openpyxl import load_workbook
 import scikitplot as skplt
 
 class support:
     #!/usr/bin/env python
     # -*- coding: utf-8 -*-
     # Author: Devendra Kumar Sahu
     # Email: devsahu99@gmail.com
@@ -34,15 +33,15 @@
     df = pd.read_csv(r'Kaggle_Titanic_Train.csv')
 
     df = df[['Survived', 'Pclass', 'Sex', 'Age', 'SibSp', 'Parch','Fare', 'Embarked']]
 
     pred_var='Survived'
 
     # To get the dropping features
-    myhelp.dropFeatures(df,pred_var,missing_threshold=.09)
+    myhelp.Get_Drop_Feature_Names(df,pred_var,missing_threshold=.09)
 
     # For grid search to obtain best hyper-parameters
     df = pd.get_dummies(df,drop_first=True)
     df.fillna(method='ffill',inplace=True)
 
     model_xgb = XGBClassifier(objective='binary:logistic',eval_metric='error',seed=42,
                    max_depth=10,colsample_bytree=.9,n_estimators=100)
@@ -59,27 +58,24 @@
     X_train, X_test, y_train, y_test = train_test_split(df.drop(pred_var,axis=1), df[pred_var], test_size=0.30, random_state=42)
     model_xgb.fit(X_train,y_train)
 
     # Predict the probabilities
     pred_prob = model_xgb.predict_proba(X_test)
 
     # Get Precision-Recall Scores
-    pr_scores = myhelp.getPRA(pred_prob,y_test)
-
-    # Save the precision-recall scores into excel sheet
-    myhelp.save_excel(pr_scores,'text.xlsx')
+    pr_scores = myhelp.Get_Precision_Recall_Values(pred_prob,y_test)
 
     # Get confusion-matrix and other plots
-    myhelp.modelplot(pred_prob,y_test,rocplot=True)
+    myhelp.Model_Output_Plots(pred_prob,y_test,rocplot=True)
     
     """
     def __init__(self):
         #initiating the class
         self.__mode=1
-    def gs_find(self,df,pred_var,clf,param_grid,refit_score='precision_score',random_search=True,folds=10,iters=20,train_split=.3,split_state=99):
+    def Grid_Search(self,df,pred_var,clf,param_grid,refit_score='precision_score',random_search=True,folds=10,iters=20,train_split=.3,split_state=99):
         """
         This helps is doing grid search. The default functionality is defined to 
         work on all the available cores for faster searching.
 
         Parameters:
         ------------------------------------------------------------
         df: pandas dataframe
@@ -130,30 +126,30 @@
         df = pd.read_csv(r'Kaggle_Titanic_Train.csv')
 
         df = df[['Survived', 'Pclass', 'Sex', 'Age', 'SibSp', 'Parch','Fare', 'Embarked']]
 
         pred_var='Survived'
 
         # To get the dropping features
-        myhelp.dropFeatures(df,pred_var,missing_threshold=.09)
+        myhelp.Get_Drop_Feature_Names(df,pred_var,missing_threshold=.09)
 
         # For grid search to obtain best hyper-parameters
         df = pd.get_dummies(df,drop_first=True)
         df.fillna(method='ffill',inplace=True)
 
         model_xgb = XGBClassifier(objective='binary:logistic',eval_metric='error',seed=42,
                        max_depth=10,colsample_bytree=.9,n_estimators=100)
 
         param_grid = {'scale_pos_weight':[6],
         'learning_rate':[.4],
         'max_depth': [13],
         'min_child_weight': [.1,1,20], #.1,1,20
         }
 
-        grid_xg_ps = myhelp.gs_find(df,pred_var,model_xgb,param_grid,random_search=False)
+        grid_xg_ps = myhelp.Grid_Search(df,pred_var,model_xgb,param_grid,random_search=False)
         
         """
         X_train, X_test, y_train, y_test = train_test_split(df.drop(pred_var,axis=1), df[pred_var], test_size=train_split, random_state=split_state)
         scorers = {
             'precision_score': make_scorer(precision_score),
             'recall_score': make_scorer(recall_score),
             'accuracy_score': make_scorer(accuracy_score)
@@ -166,44 +162,19 @@
         grid_search.fit(X_train.values, y_train.values)
         y_pred = grid_search.predict(X_test.values)
         print('Best params for {refit_score}')
         print(grid_search.best_params_)
         print(f'\nConfusion matrix of Random Forest optimized for {refit_score} on the test data')
         print(pd.DataFrame(confusion_matrix(y_test, y_pred),columns=['pred_neg', 'pred_pos'], index=['neg', 'pos']))
         return grid_search
-
-    def save_excel(self,df,wrkbook,wrksheet='Sheet1'):
-        """
-        This utility helps in saving the output into excel file worksheets.
-
-        Parameters:
-        ------------------------------------------------------------
-        df: Pandas Dataframe
-            The reference to pandas dataframe
-        wrkbook: Excel Path
-            Reference to excel workbook
-        wrksheet: String
-            name of the worksheet in which the dataframe should be saved. Default is 'Sheet1'
-        """
-        try:
-            book = load_workbook(wrkbook)
-            writer = pd.ExcelWriter(wrkbook, engine = 'openpyxl')
-            writer.book = book
-            writer.sheets = dict((ws.title, ws) for ws in book.worksheets)  
-            df.to_excel(writer, sheet_name = wrksheet,index=False)
-        except:
-            writer = pd.ExcelWriter(wrkbook, engine = 'openpyxl')
-            df.to_excel(writer, sheet_name = wrksheet,index=False)
-        writer.save()
-        writer.close()
     
     def __adjusted_classes(self, y_scores, t):
         return [1 if y >= t else 0 for y in y_scores]
 
-    def modelplot(self,pred_probs,y_test,t=0.5,cf_matrix=True,rocplot=False,skplot=False,prcplot=False,thrplot=False):
+    def Model_Output_Plots(self,pred_probs,y_test,t=0.5,cf_matrix=True,rocplot=False,skplot=False,prcplot=False,thrplot=False):
         """
         This utility prints confusion matrix and displays multiple relevant charts.
 
         Parameters:
         ------------------------------------------------------------
         pred_prob: matrix
             The prediction probabilities obtained from the scikit-learn function pred_prob
@@ -283,15 +254,15 @@
             plt.plot(thresholds[0:cutoff], p[0:cutoff], "b--", label="Precision")
             plt.plot(thresholds[0:cutoff], r[0:cutoff], "g-", label="Recall")
             plt.ylabel("Score")
             plt.xlabel("Decision Threshold")
             plt.legend(loc='best')
             plt.show()
     # Add prediction probability to dataframe
-    def getPRA(self,pred_prob,y_test):
+    def Get_Precision_Recall_Values(self,pred_prob,y_test):
         """
         This utility helps is getting precision-recall values at multiple thresholds.
 
         Parameters:
         ------------------------------------------------------------
         pred_prob: matrix
             The prediction probabilities obtained from the scikit-learn function pred_prob
@@ -379,15 +350,15 @@
         for col in cols:
             na_vals = df[col].isna().sum()
             na_per = na_vals/rows
             if na_per>self.__missing_threshold:
                 colsToRemove.append(col)
         return colsToRemove
     
-    def dropFeatures(self,df,pred_var,missing_threshold=.95):
+    def Get_Drop_Feature_Names(self,df,pred_var,missing_threshold=.95):
         """
         This utility helps is getting non-essential features in a dataframe for classification problems.
         The function takes evaluates each features and returns curated names of features to be removed.
         
         Parameters:
         ------------------------------------------------------------
         df: pandas dataframe
@@ -408,9 +379,9 @@
         self.__pred_var = pred_var
         self.__missing_threshold = missing_threshold
         self.__sparseCounts = 2
         colsRemove = []
         colsRemove.extend(self.__constance_columns())
         colsRemove.extend(self.__drop_sparse())
         colsRemove.extend(self.__getmissing())
-        dropCols = {'dropFeatures':list(set(colsRemove)),'duplicates':self.__duplicate_columns()}
+        dropCols = {'Drop_Features':list(set(colsRemove)),'duplicates':self.__duplicate_columns()}
         return dropCols
```

### Comparing `mlh-0.0.6/mlh/woe.py` & `mlh-0.0.7/mlh/woe.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class woe:
     #!/usr/bin/env python
     # -*- coding: utf-8 -*-
     # Author: Devendra Kumar Sahu
     # Email: devsahu99@gmail.com
     """
-    This function will help to calculate Weight of Evidence and Information Value, the charts can be displayed and coarse classing can also be done using reset_woe() function.
+    This function will help to calculate Weight of Evidence and Information Value, the charts can be displayed and coarse classing can also be done using Reset_Woe() function.
 
     Parameters:
     ------------------------------------------------------------
     max_bin: int
         Maximum number of bins for numeric variables. The default is 10
     iv_threshold: float
         Threshold value for Information Value. Variables with higher than threshold will be considered for transformation
@@ -64,18 +64,18 @@
     ### Create Instance of Weight of Evidence Package
     my_woe = woe()
     
     ### Fit the data with created instance
     my_woe.fit(df,'y')
     
     ### Display the relevant charts
-    my_woe.getWoeCharts()
+    my_woe.Display_WOE_Charts()
     
     ### Get Information Value
-    my_woe.get_IV()
+    my_woe.Get_Information_Values()
     
     ### Replace the original values in the Dataframe with Weight of Evidence
     transformed_df = my_woe.transform()
     """
     def __init__(self,max_bin=10,iv_threshold=0.02,ignore_threshold=True):
         self.__max_bin = max_bin
         self.__force_bin = 2
@@ -248,15 +248,15 @@
                     conv["VAR_NAME"] = i
                     count = count + 1
                 if count == 0:
                     iv_df = conv
                 else:
                     iv_df = iv_df.append(conv,ignore_index=True,sort=True)
         self.__all_iv_df = iv_df
-        iv = self.get_IV()
+        iv = self.Get_Information_Values()
         self.__all_iv = iv
         if self.__threshold_ignore:
             self.__rel_iv = iv.reset_index(drop = True)
         else:
             self.__rel_iv = iv[iv['IV']>self.__threshold].reset_index(drop = True)
         self.__rel_iv_vars = [i for i in self.__rel_iv['VAR_NAME']]  
     def transform(self,relevant_variable_sublist='All'):
@@ -284,23 +284,23 @@
             final_rel_vars = relevant_variable_sublist
         rel_var_dict = {key:value for (key,value) in zip(final_rel_vars,[i+'_woe' for i in final_rel_vars])}
         transf_df = self.__df[list(set(list(final_rel_vars+[self.__pred_var])))].copy()
         for i in range(len(final_rel_vars)):
             transf_df[rel_var_dict[final_rel_vars[i]]] = self.__replace_col(transf_df[final_rel_vars[i]],final_rel_vars[i])
         transf_df.drop(final_rel_vars,axis=1,inplace=True)
         return transf_df
-    def get_IV_df(self):
+    def Get_WOE_Values(self):
         """
         This Function returns the Information Values, Weight of Evidence and other details as a DataFrame
         
         """
         woe_max_iter = self.__all_iv_df.groupby(['VAR_NAME'])[['Iter']].agg('max').reset_index()
         latest_woe = pd.merge(self.__all_iv_df,woe_max_iter,on=['VAR_NAME','Iter'])
         return latest_woe
-    def set_threshold(self,iv_threshold=0.02,ignore_threshold=False):
+    def Set_Variable_Selection_Threshold(self, iv_threshold=0.02, ignore_threshold=False):
         """
         This Function sets the variable selection thresholds. The variables having Information Value higher 
         than this threshold are selected. 
         
         Parameters:
         ------------------------------------------------------------
         iv_threshold: float
@@ -313,27 +313,27 @@
         iv = self.__all_iv
         if ignore_threshold:
             self.__rel_iv = iv.reset_index(drop = True)
         else:
             self.__rel_iv = iv[iv['IV']>self.__threshold].reset_index(drop = True)
         self.__rel_iv_vars = [i for i in self.__rel_iv['VAR_NAME']]
         return None
-    def get_IV(self):
+    def Get_Information_Values(self):
         """
         This Function returns latest iteration Information Values as a pandas DataFrame. 
         
         """
         woe_max_iter = self.__all_iv_df.groupby(['VAR_NAME'])[['Iter']].agg('max').reset_index()
         latest_woe = pd.merge(self.__all_iv_df,woe_max_iter,on=['VAR_NAME','Iter'])
         latest_iv = latest_woe.groupby(['VAR_NAME'])[['IV']].agg('max').reset_index()
         return latest_iv
-    def reset_woe(self,variable_index = 0,reset_indexes=(0,1),previous_iteration=0):
+    def Reset_Woe(self,variable_index = 0,reset_indexes=(0,1),previous_iteration=0):
         """
         This Function resets the weight of evidence of adjancent values where the chart is not smooth.
-        The smoothness can be observed using the getWoeCharts() function.
+        The smoothness can be observed using the Display_WOE_Charts() function.
         
         Parameters:
         ------------------------------------------------------------
         variable_index: int
             The index of the variable displayed in the title of the charts. This index is maintained internally
             therefore, it is highly recommended to use the chart index only while using this reset function.
             
@@ -415,15 +415,15 @@
                     if pd.isnull(comval):
                         opval.append(round(nanmin,3))
                         break
                     elif minvec[i]<=comval<=maxvec[i]:
                         opval.append(minvec[i])
                         break
         return pd.Series(opval)
-    def getWoeCharts(self):
+    def Display_WOE_Charts(self):
         """
         This Function display all the WOE charts of the dataframe. The number of charts displayed depends
         upon the class hyper-parameter 'ignore_threshold'. To switch between all and relevant variables,
         change the hyper-parameter accordingly.
         """
         for i in range(len(self.__rel_iv_vars)):
             self.__getcompcharts(i)
```

### Comparing `mlh-0.0.6/mlh.egg-info/PKG-INFO` & `mlh-0.0.7/mlh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.0.6/setup.py` & `mlh-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlh",
-    version = '0.0.6',
+    version = '0.0.7',
     author="Devendra Kumar Sahu",
     author_email="devsahu99@gmail.com",
     description="This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/devsahu99/mlh",
     packages=['mlh'],
```

