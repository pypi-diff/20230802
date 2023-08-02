# Comparing `tmp/berrydb-1.0.3.tar.gz` & `tmp/berrydb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berrydb-1.0.3.tar", last modified: Fri Jul 21 06:09:58 2023, max compression
+gzip compressed data, was "berrydb-1.0.4.tar", last modified: Wed Aug  2 10:55:42 2023, max compression
```

## Comparing `berrydb-1.0.3.tar` & `berrydb-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-21 06:09:58.648478 berrydb-1.0.3/
--rw-rw-r--   0 akash     (1000) akash     (1000)    11470 2023-07-21 06:05:47.000000 berrydb-1.0.3/BerryDB.py
--rw-rw-r--   0 akash     (1000) akash     (1000)      405 2023-07-21 06:09:58.648478 berrydb-1.0.3/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      151 2023-07-05 10:36:56.000000 berrydb-1.0.3/README.md
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-21 06:09:58.648478 berrydb-1.0.3/berrydb.egg-info/
--rw-rw-r--   0 akash     (1000) akash     (1000)      405 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      183 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        9 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/requires.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        8 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/top_level.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       38 2023-07-21 06:09:58.648478 berrydb-1.0.3/setup.cfg
--rw-rw-r--   0 akash     (1000) akash     (1000)      508 2023-07-21 06:09:20.000000 berrydb-1.0.3/setup.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-08-02 10:55:42.227097 berrydb-1.0.4/
+-rw-rw-r--   0 akash     (1000) akash     (1000)    11680 2023-08-02 10:17:21.000000 berrydb-1.0.4/BerryDB.py
+-rw-rw-r--   0 akash     (1000) akash     (1000)      459 2023-08-02 10:55:42.227097 berrydb-1.0.4/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      191 2023-08-02 10:16:10.000000 berrydb-1.0.4/README.md
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-08-02 10:55:42.223097 berrydb-1.0.4/berrydb.egg-info/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      459 2023-08-02 10:55:42.000000 berrydb-1.0.4/berrydb.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      183 2023-08-02 10:55:42.000000 berrydb-1.0.4/berrydb.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-08-02 10:55:42.000000 berrydb-1.0.4/berrydb.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        9 2023-08-02 10:55:42.000000 berrydb-1.0.4/berrydb.egg-info/requires.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        8 2023-08-02 10:55:42.000000 berrydb-1.0.4/berrydb.egg-info/top_level.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)       38 2023-08-02 10:55:42.227097 berrydb-1.0.4/setup.cfg
+-rw-rw-r--   0 akash     (1000) akash     (1000)      522 2023-08-02 10:55:09.000000 berrydb-1.0.4/setup.py
```

### Comparing `berrydb-1.0.3/BerryDB.py` & `berrydb-1.0.4/BerryDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def databases(self, api_key: str):
         """Function summary
 
         Args:
             arg1 (str): API Key
 
         Returns:
-            list: List of Databases
+            list: Dict of Databases
         """
 
         url = get_database_list_by_api_key_url
         params = {"apiKey": api_key}
 
         if debug_mode:
             print("url:", url)
@@ -74,15 +74,19 @@
             ):
                 databaseNames = {}
                 # print("\nDatabases:")
                 for db in jsonResponse["database"]["responseList"]:
                     name = db["name"] if db["name"] else ""
                     schemaName = db["schemaName"] if db["schemaName"] else ""
                     description = db["description"] if db["description"] else ""
+                    dbId = db["id"] if db["id"] else ""
+                    schemaId = db["schemaId"] if db["schemaId"] else ""
                     databaseNames[name] = {
+                        "id": dbId,
+                        "schemaId": schemaId,
                         "schemaName": schemaName,
                         "description": description,
                     }
                     # print(name + " : " + str(databaseNames[name]))
                 # print("\n")
                 return databaseNames
             return {}
```

