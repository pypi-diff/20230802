# Comparing `tmp/smart_factory_faker-0.8.0.tar.gz` & `tmp/smart_factory_faker-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_factory_faker-0.8.0.tar", last modified: Wed Aug  2 06:01:29 2023, max compression
+gzip compressed data, was "smart_factory_faker-0.8.1.tar", last modified: Wed Aug  2 06:38:05 2023, max compression
```

## Comparing `smart_factory_faker-0.8.0.tar` & `smart_factory_faker-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 06:01:29.236884 smart_factory_faker-0.8.0/
--rw-rw-rw-   0        0        0     1863 2023-08-02 06:01:29.235920 smart_factory_faker-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 06:01:29.236884 smart_factory_faker-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-08-02 06:01:22.000000 smart_factory_faker-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:01:29.233962 smart_factory_faker-0.8.0/smart_factory_faker.egg-info/
--rw-rw-rw-   0        0        0     1863 2023-08-02 06:01:29.000000 smart_factory_faker-0.8.0/smart_factory_faker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-08-02 06:01:29.000000 smart_factory_faker-0.8.0/smart_factory_faker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:01:29.000000 smart_factory_faker-0.8.0/smart_factory_faker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:01:29.000000 smart_factory_faker-0.8.0/smart_factory_faker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:05.359368 smart_factory_faker-0.8.1/
+-rw-rw-rw-   0        0        0     1091 2023-08-02 06:03:18.000000 smart_factory_faker-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     1894 2023-08-02 06:38:05.359368 smart_factory_faker-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-02 06:38:05.360256 smart_factory_faker-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-08-02 06:38:01.000000 smart_factory_faker-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:05.357339 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/
+-rw-rw-rw-   0        0        0     1894 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/top_level.txt
```

### Comparing `smart_factory_faker-0.8.0/PKG-INFO` & `smart_factory_faker-0.8.1/smart_factory_faker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: smart_factory_faker
-Version: 0.8.0
+Name: smart-factory-faker
+Version: 0.8.1
 Summary: Smart-Factory-Faker
 Home-page: https://github.com/HyoungSooo/smart-factory-faker
 Author: HyoungSooo
 Author-email: aaa57403@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Smart Factory Faker
 
 ### how to use
 ```shell
-<clone this repotitory>
+pip install smart-factory-faker
 ```
 
 This is a project that can build a fake data set with a process.
 You can define the route of the process and by defining the sensor, you can build a data set of the process in progress.
 
 ### Tutorial
 * [Tutorial](https://github.com/HyoungSooo/smart-factory-faker/blob/main/tutorial.ipynb)
```

### Comparing `smart_factory_faker-0.8.0/smart_factory_faker.egg-info/PKG-INFO` & `smart_factory_faker-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: smart-factory-faker
-Version: 0.8.0
+Name: smart_factory_faker
+Version: 0.8.1
 Summary: Smart-Factory-Faker
 Home-page: https://github.com/HyoungSooo/smart-factory-faker
 Author: HyoungSooo
 Author-email: aaa57403@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Smart Factory Faker
 
 ### how to use
 ```shell
-<clone this repotitory>
+pip install smart-factory-faker
 ```
 
 This is a project that can build a fake data set with a process.
 You can define the route of the process and by defining the sensor, you can build a data set of the process in progress.
 
 ### Tutorial
 * [Tutorial](https://github.com/HyoungSooo/smart-factory-faker/blob/main/tutorial.ipynb)
```

