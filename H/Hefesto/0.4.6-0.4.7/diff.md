# Comparing `tmp/Hefesto-0.4.6.tar.gz` & `tmp/Hefesto-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.6.tar", last modified: Thu Jul 27 09:10:40 2023, max compression
+gzip compressed data, was "Hefesto-0.4.7.tar", last modified: Wed Aug  2 17:27:46 2023, max compression
```

## Comparing `Hefesto-0.4.6.tar` & `Hefesto-0.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-07-27 09:10:40.936933 Hefesto-0.4.6/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-07-27 09:10:40.936933 Hefesto-0.4.6/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.6/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12403 2023-07-27 09:09:46.000000 Hefesto-0.4.6/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    17218 2023-07-27 08:35:48.000000 Hefesto-0.4.6/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-07-27 09:10:40.936933 Hefesto-0.4.6/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.6/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-07-27 09:10:40.936933 Hefesto-0.4.6/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2581 2023-06-19 08:51:18.000000 Hefesto-0.4.6/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.6/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-07-27 09:10:40.936933 Hefesto-0.4.6/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-07-27 09:09:56.000000 Hefesto-0.4.6/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-08-02 17:27:46.477451 Hefesto-0.4.7/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-08-02 17:27:46.477451 Hefesto-0.4.7/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.7/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12397 2023-08-02 17:26:41.000000 Hefesto-0.4.7/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    17218 2023-08-02 14:13:23.000000 Hefesto-0.4.7/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-08-02 17:27:46.477451 Hefesto-0.4.7/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-08-02 17:27:46.000000 Hefesto-0.4.7/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-08-02 17:27:46.000000 Hefesto-0.4.7/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-08-02 17:27:46.000000 Hefesto-0.4.7/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-08-02 17:27:46.000000 Hefesto-0.4.7/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.7/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-08-02 17:27:46.477451 Hefesto-0.4.7/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2588 2023-08-02 11:11:05.000000 Hefesto-0.4.7/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.7/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-08-02 17:27:46.477451 Hefesto-0.4.7/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-08-02 17:27:21.000000 Hefesto-0.4.7/setup.py
```

### Comparing `Hefesto-0.4.6/Hefesto/main.py` & `Hefesto-0.4.7/Hefesto/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,11 +306,11 @@
 # # Test 2:
 
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
 
 # test = Hefesto(datainput = "../data/INPUT_DATA2.csv")
 # transform = test.transformShape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
-# # label = test.get_label("output_type")
-# # url_from_label= test.get_uri("output_type_label","ncit")
-# # repl= test.replacement("output_type_label", "Date","DateXXX", duplicate=False)
+# label = test.get_label("output_type")
+# url_from_label= test.get_uri("output_type_label","ncit")
+# repl= test.replacement("output_type_label", "Date","DateXXX", duplicate=False)
 # transform.to_csv ("../data/OUTPUT_DATA2_new.csv", index = False, header=True)
```

### Comparing `Hefesto-0.4.6/Hefesto/template.py` & `Hefesto-0.4.7/Hefesto/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,16 @@
     Sex = dict( 
 
       pid = None,
       context_id = None,
       comments = None,
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C28421",
-      attribute_type2 = None,
+      attribute_type = None,
+      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C28421",
       agent_id = None,
       input_type = None,
       target_type = None,
       unit_type = None,
       agent_type = None,
       frequency_type = None,
       frequency_value = None,
@@ -166,16 +166,16 @@
     Status = dict(
 
       pid = None,
       context_id = None,
       comments = None,
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C166244",
-      attribute_type2 = None,
+      attribute_type = None,
+      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C166244",
       agent_id = None,
       input_type = None,
       target_type = None,
       unit_type = None,
       agent_type = None,
       frequency_type = None,
       frequency_value = None,
@@ -228,16 +228,16 @@
 
     Symptoms = dict(
       pid = None,
       context_id = None,
       comments = None,
       process_type = "http://purl.obolibrary.org/obo/NCIT_C15220",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C100104",
-      attribute_type2 = None,
+      attribute_type = None,
+      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C100104",
       agent_id = None,
       input_type = None,
       target_type = None,
       unit_type = None,
       agent_type = None,
       frequency_type = None,
       frequency_value = None,
```

### Comparing `Hefesto-0.4.6/README.md` & `Hefesto-0.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 
 * Conducting a sanity check on the `stardate` and `enddate` columns to ensure data consistency and validity.
 
 * Eliminating any input rows that lack of the minimal required data to minimize the generation of incomplete RDF transformations.
 
 * Creation of the column called `uniqid` that assigns a unique identifier to each observation. This prevents the RDF instances from overlapping with one another, ensuring their distinctiveness and integrity.
 
+## Dockerized implementation:
+
+There's a Docker-based implementation controlled via API (using FastAPI) that you can use for mounting this data transformation step as a part of your CDE implementation. Use our docker compose to control your Docker image, ports where its located and volumes in order to pass your CSV-based CDE patient data:
+
+```yaml
+version: "3.3"
+
+services:
+  api:
+    image: pabloalarconm/hefesto_fiab:0.0.6
+    ports:
+      - "8000:8000"
+    volumes:
+      - ./data:/code/data
+```
+
+## Local usage:
 
-##  Installation:
+###  Installation:
 
 ```bash
 pip install Hefesto
 ```
-## Usage:
 **Requirements:**
 
 - CSV datatable with your CDE data based on [CDE implementation glossary](https://github.com/ejp-rd-vp/CDE-semantic-model-implementations/blob/master/CDE_version_2.0.0/CSV_docs/glossary.md)
 
 **Test:**
 
 ```py
 from Hefesto.main import Hefesto
 import yaml
 
 test = Hefesto(datainput = "../data/preCDE.csv") # Use your own path for your CSV input data
 transform = test.transform_Fiab()
 transform.to_csv ("../data/CDE.csv", index = False, header=True) # Change this path to the location where your resulting data should be located
-```
-
-## Dockerized implementation:
-
-There's a Docker-based implementation controlled via API (using FastAPI) that you can use for mounting this data transformation step as a part of your CDE implementation. Use our docker compose to control your Docker image, ports where its located and volumes in order to pass your CSV-based CDE patient data:
-
-```yaml
-version: "3.3"
-
-services:
-  api:
-    image: pabloalarconm/hefesto_fiab:0.0.5
-    ports:
-      - "8000:8000"
-    volumes:
-      - ./data:/code/data
 ```
```

### Comparing `Hefesto-0.4.6/setup.py` & `Hefesto-0.4.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.6",
+    version="0.4.7",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

