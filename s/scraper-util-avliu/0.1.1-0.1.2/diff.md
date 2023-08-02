# Comparing `tmp/scraper_util_avliu-0.1.1.tar.gz` & `tmp/scraper_util_avliu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraper_util_avliu-0.1.1.tar", last modified: Thu Jul 27 16:07:26 2023, max compression
+gzip compressed data, was "scraper_util_avliu-0.1.2.tar", last modified: Wed Aug  2 12:32:38 2023, max compression
```

## Comparing `scraper_util_avliu-0.1.1.tar` & `scraper_util_avliu-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.781619 scraper_util_avliu-0.1.1/
--rw-r--r--   0 avliu      (504) staff       (20)        5 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.1/LICENSE
--rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:07:26.781140 scraper_util_avliu-0.1.1/PKG-INFO
--rw-r--r--   0 avliu      (504) staff       (20)      228 2023-07-27 15:54:00.000000 scraper_util_avliu-0.1.1/README.md
--rw-r--r--   0 avliu      (504) staff       (20)      269 2023-07-27 16:07:17.000000 scraper_util_avliu-0.1.1/pyproject.toml
--rw-r--r--   0 avliu      (504) staff       (20)       38 2023-07-27 16:07:26.781741 scraper_util_avliu-0.1.1/setup.cfg
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.775346 scraper_util_avliu-0.1.1/src/
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.778013 scraper_util_avliu-0.1.1/src/scraper_util_avliu/
--rw-r--r--   0 avliu      (504) staff       (20)        1 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu/__init__.py
--rw-r--r--   0 avliu      (504) staff       (20)       36 2023-07-27 16:01:51.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu/example.py
--rw-r--r--   0 avliu      (504) staff       (20)     3243 2023-07-27 16:07:04.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu/util.py
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.780551 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/
--rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/PKG-INFO
--rw-r--r--   0 avliu      (504) staff       (20)      361 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/SOURCES.txt
--rw-r--r--   0 avliu      (504) staff       (20)        1 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/dependency_links.txt
--rw-r--r--   0 avliu      (504) staff       (20)       72 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/requires.txt
--rw-r--r--   0 avliu      (504) staff       (20)       19 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/top_level.txt
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-08-02 12:32:38.146548 scraper_util_avliu-0.1.2/
+-rw-r--r--   0 avliu      (504) staff       (20)        5 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.2/LICENSE
+-rw-r--r--   0 avliu      (504) staff       (20)       84 2023-08-02 12:32:38.146360 scraper_util_avliu-0.1.2/PKG-INFO
+-rw-r--r--   0 avliu      (504) staff       (20)      228 2023-07-27 15:54:00.000000 scraper_util_avliu-0.1.2/README.md
+-rw-r--r--   0 avliu      (504) staff       (20)      283 2023-08-02 12:32:31.000000 scraper_util_avliu-0.1.2/pyproject.toml
+-rw-r--r--   0 avliu      (504) staff       (20)       38 2023-08-02 12:32:38.146602 scraper_util_avliu-0.1.2/setup.cfg
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-08-02 12:32:38.142444 scraper_util_avliu-0.1.2/src/
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-08-02 12:32:38.144619 scraper_util_avliu-0.1.2/src/scraper_util_avliu/
+-rw-r--r--   0 avliu      (504) staff       (20)        1 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu/__init__.py
+-rw-r--r--   0 avliu      (504) staff       (20)       36 2023-07-27 16:01:51.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu/example.py
+-rw-r--r--   0 avliu      (504) staff       (20)     4077 2023-08-02 12:12:14.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu/util.py
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-08-02 12:32:38.145850 scraper_util_avliu-0.1.2/src/scraper_util_avliu.egg-info/
+-rw-r--r--   0 avliu      (504) staff       (20)       84 2023-08-02 12:32:38.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu.egg-info/PKG-INFO
+-rw-r--r--   0 avliu      (504) staff       (20)      375 2023-08-02 12:32:38.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu.egg-info/SOURCES.txt
+-rw-r--r--   0 avliu      (504) staff       (20)        1 2023-08-02 12:32:38.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu.egg-info/dependency_links.txt
+-rw-r--r--   0 avliu      (504) staff       (20)       79 2023-08-02 12:32:38.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu.egg-info/requires.txt
+-rw-r--r--   0 avliu      (504) staff       (20)       23 2023-08-02 12:32:38.000000 scraper_util_avliu-0.1.2/src/scraper_util_avliu.egg-info/top_level.txt
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-08-02 12:32:38.146041 scraper_util_avliu-0.1.2/tests/
+-rw-r--r--   0 avliu      (504) staff       (20)      100 2023-08-02 12:18:47.000000 scraper_util_avliu-0.1.2/tests/test.py
```

### Comparing `scraper_util_avliu-0.1.1/src/scraper_util_avliu/util.py` & `scraper_util_avliu-0.1.2/src/scraper_util_avliu/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from selenium import webdriver
 import undetected_chromedriver as uc
 from bs4 import BeautifulSoup
 from urllib.request import Request, urlopen
 import urllib.error
 
 import mysql.connector
-import os
+
+import boto3
 
 
 def get_selenium_driver(undetected=False):
 
-    print(os.getcwd())
-    adblock_filepath = './lib/adblock.crx'
+    # adblock_filepath = '../lib/adblock.crx'
 
     if undetected:
         chrome_options = uc.ChromeOptions()
         chrome_options.add_argument('--mute-audio')
-        chrome_options.add_extension(adblock_filepath)
+        # chrome_options.add_extension(adblock_filepath)
         driver = uc.Chrome(options=chrome_options)
 
     else:
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument('--mute-audio')
-        chrome_options.add_extension(adblock_filepath)
+        # chrome_options.add_extension(adblock_filepath)
         driver = webdriver.Chrome(options=chrome_options)
 
     return driver
 
 
 def get_soup(url):
     success = False
@@ -115,10 +115,41 @@
         f"location VARCHAR(255), "
         f"fuel VARCHAR(255),"
         f"ebay_item_id VARCHAR(255),"
         f"PRIMARY KEY (vin, date_accessed)"
         f")"
     )
 
+def test_write_logs():
+    AWS_REGION = "us-west-2" #TODO: Fill
+    client = boto3.client('cloudwatch', region_name=AWS_REGION)
+    response = client.put_log_events(
+        logGroupName='TODO',
+        logStreamName='TODO',
+        logEvents=[
+            {
+                'timestamp': 123,
+                'message': 'THIS IS A TEST LOG MESSAGE'
+            },
+        ],
+        sequenceToken='TODO'
+    )
+
+
+def write_to_bucket(aws_bucket, source, dest):
+    # Make sure to configure ~/.aws/configure file
+    s3 = boto3.resource('s3')
+    s3.Bucket(aws_bucket).upload_file(source, dest)
+
+
+def main():
+    bucket = 'test-youtube-audit-bucket'
+    f = open("test_result_file.txt", "a")
+    f.write("File content!")
+    f.close()
+    destination = 'test_folder/test_results_file.txt'
+
+    write_to_bucket(bucket, "./test_result_file.txt", destination)
+
 
 if __name__ == '__main__':
-    write_to_rds()
+    main()
```

