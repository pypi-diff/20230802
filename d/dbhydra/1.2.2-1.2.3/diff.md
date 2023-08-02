# Comparing `tmp/dbhydra-1.2.2.tar.gz` & `tmp/dbhydra-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.2.2.tar", last modified: Sun Jul 30 16:18:07 2023, max compression
+gzip compressed data, was "dbhydra-1.2.3.tar", last modified: Wed Aug  2 14:54:40 2023, max compression
```

## Comparing `dbhydra-1.2.2.tar` & `dbhydra-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.980954 dbhydra-1.2.2/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-07-30 16:18:07.979956 dbhydra-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.964996 dbhydra-1.2.2/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.2/dbhydra/__init__.py
--rw-rw-rw-   0        0        0    69180 2023-07-30 16:17:27.000000 dbhydra-1.2.2/dbhydra/dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.979956 dbhydra-1.2.2/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.976964 dbhydra-1.2.2/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 16:18:07.980954 dbhydra-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-07-30 16:17:38.000000 dbhydra-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.680045 dbhydra-1.2.3/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-08-02 14:54:40.680045 dbhydra-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.647133 dbhydra-1.2.3/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.3/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0    69488 2023-08-02 14:51:30.000000 dbhydra-1.2.3/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.679048 dbhydra-1.2.3/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.662099 dbhydra-1.2.3/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:54:40.680045 dbhydra-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-08-02 14:54:37.000000 dbhydra-1.2.3/setup.py
```

### Comparing `dbhydra-1.2.2/LICENSE` & `dbhydra-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.2/PKG-INFO` & `dbhydra-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.2.2
+Version: 1.2.3
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.2.2/README.md` & `dbhydra-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.2/dbhydra/dbhydra_core.py` & `dbhydra-1.2.3/dbhydra/dbhydra_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "date": "date",
     "timestamp": "timestamp"
 }
 
 PYTHON_TO_MYSQL_DATA_MAPPING = {
     'int': "int",
     'float': "double",
-    'str': "varchar(255)",
+    'str': "nvarchar(2047)",
     'bool': "bit",
     'datetime': "datetime"
 }
 
 def read_file(file):
     """Reads txt file -> list"""
 
@@ -461,17 +461,17 @@
 
 class Mysqldb(AbstractDB):
 
     python_database_type_mapping = PYTHON_TO_MYSQL_DATA_MAPPING = \
     {
     'int': "int",
     'float': "double",
-    'str': "varchar(255)",
-    'list': "varchar(255)",
-    'dict': "varchar(255)",
+    'str': "nvarchar(2047)",
+    'list': "nvarchar(2047)",
+    'dict': "nvarchar(2047)",
     'bool': "tinyint",
     'datetime': "datetime"
     }
 
     def connect_to_db(self):
         self.connection = MySQLdb.connect(host=self.DB_SERVER, port=self.DB_PORT, user=self.DB_USERNAME, password=self.DB_PASSWORD, database=self.DB_DATABASE)
         self.cursor = self.connection.cursor()
@@ -1436,16 +1436,16 @@
                 data_types[i] = data_types[i] + f"({data_lengths[i]})"
         return (data_types)
 
 
     """
         Returns a list of data types, where each element represents the category of the data ('varchar', 'int', etc.). 
         If a data type has an associated length, the length value will be included in a corresponding element of the
-        data_lengths list, otherwise the element will have a None value. For example, 'varchar(255)' would return
-        'varchar' in the data_types list and 255 in the data_lengths list.
+        data_lengths list, otherwise the element will have a None value. For example, 'nvarchar(2047)' would return
+        'varchar' in the data_types list and 2047 in the data_lengths list.
     """
     def get_data_types_and_character_lengths(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
         query = f"SELECT DATA_TYPE,character_maximum_length FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND TABLE_NAME  = '" + self.name + "'"
         types = information_schema_table.select(query)
         data_types = [x[0] for x in types]
         data_lengths = [x[1] for x in types]
@@ -1532,14 +1532,15 @@
             print("Check the specification of table columns and their types")
 
     def insert(self, rows, batch=1, replace_apostrophes=True, try_mode=False, debug_mode=False, insert_id=False):
         start_index = 0 if insert_id else 1
         print("INSERTING!!!")
         assert len(self.columns) == len(self.types)
         print(self.types)
+        total_output=[]
         for k in range(len(rows)):
             if k % batch == 0:
                 query = "INSERT INTO " + self.name + " ("
                 for i in range(start_index, len(self.columns)):
                     if i < len(rows[k]) + 1:
                         query += self.columns[i] + ","
                 if len(rows) < len(self.columns):
@@ -1587,26 +1588,34 @@
             if k % batch == batch - 1 or k == len(rows) - 1:
                 query = query[:-1]
 
                 if debug_mode:
                     print(query)
 
                 if not try_mode:
-                    return self.db1.execute(query)
+                    output=self.db1.execute(query)
+                    total_output.append(output)
                 else:
                     try:
-                        return self.db1.execute(query)
+                        output=self.db1.execute(query)
+                        total_output.append(output)
                     except Exception as e:
 
                         print("Query", query, "Could not be inserted:", e)
 
                         # Write to logs only in debug mode
                         if debug_mode:
                             with open("log.txt", "a") as file:
                                 file.write("Query " + str(query) + " could not be inserted:" + str(e) + "\n")
+            
+            elif len(total_output)==1:
+                return(total_output[0])
+            else:
+                return(total_output)
+                
 
     def add_foreign_key(self, foreign_key):
         parent_id = foreign_key['parent_id']
         parent = foreign_key['parent']
         query = "ALTER TABLE " + self.name + " MODIFY " + parent_id + " INT UNSIGNED"
         print(query)
         self.db1.execute(query)
```

### Comparing `dbhydra-1.2.2/dbhydra/tests/test_mongo.py` & `dbhydra-1.2.3/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.2/dbhydra/tests/test_sql.py` & `dbhydra-1.2.3/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.2/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.2.3/dbhydra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.2.2
+Version: 1.2.3
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.2.2/setup.py` & `dbhydra-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.2.2',
+    version='1.2.3',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

