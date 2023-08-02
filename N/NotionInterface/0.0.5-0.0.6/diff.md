# Comparing `tmp/NotionInterface-0.0.5.tar.gz` & `tmp/NotionInterface-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotionInterface-0.0.5.tar", last modified: Mon Jul 31 19:40:52 2023, max compression
+gzip compressed data, was "NotionInterface-0.0.6.tar", last modified: Wed Aug  2 14:20:45 2023, max compression
```

## Comparing `NotionInterface-0.0.5.tar` & `NotionInterface-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-31 19:40:52.848262 NotionInterface-0.0.5/
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-31 19:40:52.846736 NotionInterface-0.0.5/NotionInterface/
--rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/__init__.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/constants.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     6845 2023-07-28 23:03:12.000000 NotionInterface-0.0.5/NotionInterface/notion_database.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/notion_database_types.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/notion_header.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/notion_page.py
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-31 19:40:52.847715 NotionInterface-0.0.5/NotionInterface.egg-info/
--rw-r--r--   0 lukapedra   (501) staff       (20)      509 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/SOURCES.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/dependency_links.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/requires.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/top_level.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      509 2023-07-31 19:40:52.848108 NotionInterface-0.0.5/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.5/README.md
--rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-31 19:40:52.848306 NotionInterface-0.0.5/setup.cfg
--rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-31 19:40:30.000000 NotionInterface-0.0.5/setup.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-08-02 14:20:45.779226 NotionInterface-0.0.6/
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-08-02 14:20:45.778138 NotionInterface-0.0.6/NotionInterface/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-26 16:55:50.000000 NotionInterface-0.0.6/NotionInterface/__init__.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-07-26 16:55:50.000000 NotionInterface-0.0.6/NotionInterface/constants.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     6966 2023-08-02 14:19:42.000000 NotionInterface-0.0.6/NotionInterface/notion_database.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     5014 2023-08-02 14:19:26.000000 NotionInterface-0.0.6/NotionInterface/notion_database_types.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-07-26 16:55:50.000000 NotionInterface-0.0.6/NotionInterface/notion_header.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-26 16:55:50.000000 NotionInterface-0.0.6/NotionInterface/notion_page.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-08-02 14:20:45.778907 NotionInterface-0.0.6/NotionInterface.egg-info/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-08-02 14:20:45.000000 NotionInterface-0.0.6/NotionInterface.egg-info/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-08-02 14:20:45.000000 NotionInterface-0.0.6/NotionInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-08-02 14:20:45.000000 NotionInterface-0.0.6/NotionInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-08-02 14:20:45.000000 NotionInterface-0.0.6/NotionInterface.egg-info/requires.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-08-02 14:20:45.000000 NotionInterface-0.0.6/NotionInterface.egg-info/top_level.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-08-02 14:20:45.779105 NotionInterface-0.0.6/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.6/README.md
+-rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-08-02 14:20:45.779271 NotionInterface-0.0.6/setup.cfg
+-rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-08-02 14:20:25.000000 NotionInterface-0.0.6/setup.py
```

### Comparing `NotionInterface-0.0.5/NotionInterface/notion_database.py` & `NotionInterface-0.0.6/NotionInterface/notion_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,18 @@
             properties = {}
             linha['id'] = res['id']
             linha['created_time'] = res['created_time']
             linha['last_edited_time'] = res['last_edited_time']
 
 
             for key in res['properties'].keys():
-                properties[key] = getValue(res['properties'][key])
+                aux = {}
+                aux['value'] = getValue(res['properties'][key])
+                aux['type'] = res['properties'][key]['type']
+                properties[key] = aux
             linha['properties'] = properties
 
             result.append(linha)
 
         # RECURSÃO PARA PRÓXIMO CURSOR
         if res_dict['next_cursor'] != None:
             result_rec = self.getAllRecordsSince(next_cursor=res_dict['next_cursor'],Updated_Since=Updated_Since)
```

### Comparing `NotionInterface-0.0.5/NotionInterface/notion_database_types.py` & `NotionInterface-0.0.6/NotionInterface/notion_database_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,23 @@
         elif (item["type"])=='relation':
             return item['relation']
         elif (item["type"])=='files':
             vet_aux = []
             for aux in item['files']:
                 aux_item = {
                     'name' : aux['name'],
-                    'file' : aux['file']['url']
                 }
+                if aux['type'] == 'external':
+                    aux_item['file'] = aux['external']['url']
+                else:
+                    aux_item['file'] = aux['file']['url']
                 vet_aux.append(aux_item)
             result = vet_aux
-        else:
-            print(str(item))
+        '''else:
+         print(str(item))'''
     except:
         result = None
     return result
 
 def generateNotionProperty(key, value, columns):
     if not (key in columns['properties']):
         raise Exception(constants.ERROR_PROPERTY_NOT_EXISTS + key)
```

### Comparing `NotionInterface-0.0.5/NotionInterface/notion_page.py` & `NotionInterface-0.0.6/NotionInterface/notion_page.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.5/setup.py` & `NotionInterface-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A simple Notion db interface for Python'
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 # Setting up
 setup(
```

