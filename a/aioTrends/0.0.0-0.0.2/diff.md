# Comparing `tmp/aioTrends-0.0.0.tar.gz` & `tmp/aioTrends-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioTrends-0.0.0.tar", last modified: Mon Jul 24 17:43:48 2023, max compression
+gzip compressed data, was "aioTrends-0.0.2.tar", last modified: Tue Aug  1 23:09:35 2023, max compression
```

## Comparing `aioTrends-0.0.0.tar` & `aioTrends-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,12 @@
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.766132 aioTrends-0.0.0/
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.725382 aioTrends-0.0.0/.github/
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.744333 aioTrends-0.0.0/.github/ISSUE_TEMPLATE/
--rwx------   0 stephencheung   (501) staff       (20)      872 2023-01-18 14:13:30.000000 aioTrends-0.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rwx------   0 stephencheung   (501) staff       (20)      136 2023-01-18 14:13:30.000000 aioTrends-0.0.0/.github/ISSUE_TEMPLATE/custom.md
--rwx------   0 stephencheung   (501) staff       (20)      615 2023-01-18 14:13:30.000000 aioTrends-0.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-13 12:09:51.000000 aioTrends-0.0.0/LICENSE
--rw-r--r--   0 stephencheung   (501) staff       (20)     6188 2023-07-24 17:43:48.766529 aioTrends-0.0.0/PKG-INFO
--rwx------   0 stephencheung   (501) staff       (20)     5498 2023-07-24 17:39:00.000000 aioTrends-0.0.0/README.md
--rwx------   0 stephencheung   (501) staff       (20)      640 2023-01-13 12:09:51.000000 aioTrends-0.0.0/SECURITY.md
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.749806 aioTrends-0.0.0/aioTrends/
--rwx------   0 stephencheung   (501) staff       (20)      477 2023-01-18 14:13:31.000000 aioTrends-0.0.0/aioTrends/HandleExceptions.py
--rwx------   0 stephencheung   (501) staff       (20)     6562 2023-07-24 14:41:43.000000 aioTrends-0.0.0/aioTrends/Settings.py
--rwx------   0 stephencheung   (501) staff       (20)    19887 2023-07-24 17:32:39.000000 aioTrends-0.0.0/aioTrends/Trends.py
--rwx------   0 stephencheung   (501) staff       (20)      377 2023-07-24 15:43:56.000000 aioTrends-0.0.0/aioTrends/__init__.py
--rwx------   0 stephencheung   (501) staff       (20)     4692 2023-01-31 14:15:34.000000 aioTrends-0.0.0/aioTrends/processData.py
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.754937 aioTrends-0.0.0/aioTrends.egg-info/
--rw-r--r--   0 stephencheung   (501) staff       (20)     6188 2023-07-24 17:43:48.000000 aioTrends-0.0.0/aioTrends.egg-info/PKG-INFO
--rw-r--r--   0 stephencheung   (501) staff       (20)      581 2023-07-24 17:43:48.000000 aioTrends-0.0.0/aioTrends.egg-info/SOURCES.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-07-24 17:43:48.000000 aioTrends-0.0.0/aioTrends.egg-info/dependency_links.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       48 2023-07-24 17:43:48.000000 aioTrends-0.0.0/aioTrends.egg-info/requires.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       10 2023-07-24 17:43:48.000000 aioTrends-0.0.0/aioTrends.egg-info/top_level.txt
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.756241 aioTrends-0.0.0/data/
--rwx------   0 stephencheung   (501) staff       (20)        0 2023-01-11 11:54:13.000000 aioTrends-0.0.0/data/IOT
--rwx------   0 stephencheung   (501) staff       (20)      206 2023-01-05 23:43:54.000000 aioTrends-0.0.0/data/qrys.pkl
--rw-r--r--   0 stephencheung   (501) staff       (20)     7576 2023-07-24 16:08:11.000000 aioTrends-0.0.0/example_scaled_daily_data.png
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.757401 aioTrends-0.0.0/proxies/
--rwx------   0 stephencheung   (501) staff       (20)      118 2023-01-05 23:49:27.000000 aioTrends-0.0.0/proxies/proxies.txt
--rwx------   0 stephencheung   (501) staff       (20)       42 2023-07-24 13:27:06.000000 aioTrends-0.0.0/requirements.txt
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-07-24 17:43:48.762573 aioTrends-0.0.0/settings/
--rwx------   0 stephencheung   (501) staff       (20)      531 2023-01-31 11:00:36.000000 aioTrends-0.0.0/settings/settings.json
--rwx------   0 stephencheung   (501) staff       (20)   132936 2022-07-05 12:28:50.000000 aioTrends-0.0.0/settings/userAgents.json
--rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-07-24 17:43:48.768069 aioTrends-0.0.0/setup.cfg
--rw-r--r--   0 stephencheung   (501) staff       (20)     1349 2023-07-24 17:43:07.000000 aioTrends-0.0.0/setup.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:09:35.911794 aioTrends-0.0.2/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     6571 2023-08-01 23:09:35.910794 aioTrends-0.0.2/PKG-INFO
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:09:35.899302 aioTrends-0.0.2/aioTrends/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     1363 2023-08-01 23:09:07.000000 aioTrends-0.0.2/aioTrends/SETUP.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)      688 2023-08-01 22:49:00.000000 aioTrends-0.0.2/aioTrends/test_example.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:09:35.909461 aioTrends-0.0.2/aioTrends.egg-info/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     6571 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/PKG-INFO
+-rw-r--r--   0 stephencheung   (501) staff       (20)      208 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/SOURCES.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/dependency_links.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       59 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/requires.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       10 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/top_level.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       38 2023-08-01 23:09:35.912011 aioTrends-0.0.2/setup.cfg
```

### Comparing `aioTrends-0.0.0/PKG-INFO` & `aioTrends-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: aioTrends
-Version: 0.0.0
+Version: 0.0.2
 Summary: Library for fetching Google Trends in an async. way
 Home-page: https://github.com/yuz0101/aioTrends
-Download-URL: https://github.com/yuz0101/aioTrends/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/yuz0101/aioTrends/archive/refs/tags/v_02.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: google,trends,async,asyncio,aiohttp,googletrends,pytrends
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # aioTrends
 
 ## Intro.
 
 This is a project for asynchronously obtaining data from google trends in an efficient way. Inspired by [pytrends](https://github.com/GeneralMills/pytrends), I am developing this project based on a asynchronous framework, asyncio, and a related module, [aiohttp](https://github.com/aio-libs/aiohttp).
 
@@ -65,37 +64,39 @@
 where python3.11
 ```
 copy the path to python 3.11 and replace below path
 ```consol
 virtualenv -p /path/to/python3.11 atenv
 ```
 4. Activate the virtual environment
+
 On Windows:
 ```consol
 atenv\Scripts\activate
 ```
 On macOS and Linux:
 ```consol
 source atenv/bin/activate
 ```
-5. Install aioTrends********
+5. Install aioTrends ********
+
 the package must be installed under the environment of python 3.10+  
 ```consol
 pip install aioTrends
 ```
 
 6. Checking if installed properly. The programme will creat folders, please follow the instructions given by the programme.
 ```consol
 cd path/to/your/working/path
 python
 import aioTrends as at
 ```
-7. Amend the settings.json under the folder settings.
-8. Paste proxies to the proxies.txt under the folder proxies.
-9. Get userAgents.json file from [Said-Ait-Driss](https://github.com/Said-Ait-Driss/user-agents) and past it under
+7. Amend the settings.json under the folder 'settings'.
+8. Paste proxies to the proxies.txt under the folder 'proxies'.
+9. Get userAgents.json file from [Said-Ait-Driss](https://github.com/Said-Ait-Driss/user-agents) and past it under the folder 'settings'.
 
 ## Getting Started
 ### II. Setup a queries file
 
 ```python
 import pickle
 qrys = {
@@ -110,16 +111,18 @@
 
 pickle.dump(qrys, open('./data/qrys.pkl', 'wb'))
 ```
 
 Alternatively, function ```formQueries``` would form the query dataset based on the list of keywords you give.
 ```python
 from aioTrends import formQueries
+from datetime import date
+import pickle
 
-qrys = formQueries(keywords: ['AMZN', 'MSFN'], start='2004-01-01', end=date.today(), freq: str='D')
+qrys = formQueries(keywords=['AMZN', 'MSFN'], start='2004-01-01', end=date.today(), freq='D')
 pickle.dump(qrys, open('./data/qrys.pkl', 'wb'))
 ```
 
 ### III. Create a py script named as example.py
 
 ```python
 import aioTrends as at
@@ -139,28 +142,39 @@
 
 Alternatively, you can use below one line for forming queries and getting daily scaled data or monthly data.
 ```python
 
 import aioTrends as at
 from datetime import date
 
-qry_list = ['AMZN', 'MSFN']
+qry_list = ['AMZN', 'AAPL', 'MSFT']
 
-# running 100 cocurrent tasks
-df = at.Aio(100).getScaledDailyData(
+# running 50 cocurrent tasks
+ataio = at.Aio(50)
+
+df = ataio.getScaledDailyData(
     keywords=qry_list, # the query keyword list
-    filename='output.csv', # json and pickle are both supported
+    filename='test.csv', # json and pickle are both supported
     start='2004-01-01', # both datetime and str are supported
     end=date.today()
     )
-print(df)
 
-df_m = at.Aio(50).getMonthlyData(keywords=qry_list, start='2004-01-01', end='2022-12-31')
-print(df_m)
+fig = df.plot(figsize=(16,8), title='TEST_SCALED_DAILY_DATA').get_figure()
+fig.savefig('test_scaled_daily_data.png')
+
+df_m = ataio.getMonthlyData(
+    keywords=qry_list, 
+    start='2004-01-01', 
+    end='2022-12-31'
+    )
+fig = df_m.plot(figsize=(16,8), title='TEST_MONTHLY_DATA').get_figure()
+fig.savefig('test_monthly_data.png')
 ```
 
 ### IV. Run the above example.py file on your terminal or cmd (The code need to be running under the python 3.10+ environment)
 
 ```consol
 python example.py
 ```
 
+![Monthly Data](test_monthly_data.png)
+![Scaled Daily Data](test_scaled_daily_data.png)
```

### Comparing `aioTrends-0.0.0/README.md` & `aioTrends-0.0.2/aioTrends.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: aioTrends
+Version: 0.0.2
+Summary: Library for fetching Google Trends in an async. way
+Home-page: https://github.com/yuz0101/aioTrends
+Download-URL: https://github.com/yuz0101/aioTrends/archive/refs/tags/v_02.tar.gz
+Author: Stephen Zhang
+Author-email: stephen_se@outlook.com
+License: MIT
+Keywords: google,trends,async,asyncio,aiohttp,googletrends,pytrends
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # aioTrends
 
 ## Intro.
 
 This is a project for asynchronously obtaining data from google trends in an efficient way. Inspired by [pytrends](https://github.com/GeneralMills/pytrends), I am developing this project based on a asynchronous framework, asyncio, and a related module, [aiohttp](https://github.com/aio-libs/aiohttp).
 
 The logic behind this project is to firstly build a cookies pool, then obtain and store the tokenized queries (wrapped inside the widgets) in another pool, and lastly retreive the data with widgets from the widget pool.
@@ -47,37 +64,39 @@
 where python3.11
 ```
 copy the path to python 3.11 and replace below path
 ```consol
 virtualenv -p /path/to/python3.11 atenv
 ```
 4. Activate the virtual environment
+
 On Windows:
 ```consol
 atenv\Scripts\activate
 ```
 On macOS and Linux:
 ```consol
 source atenv/bin/activate
 ```
-5. Install aioTrends********
+5. Install aioTrends ********
+
 the package must be installed under the environment of python 3.10+  
 ```consol
 pip install aioTrends
 ```
 
 6. Checking if installed properly. The programme will creat folders, please follow the instructions given by the programme.
 ```consol
 cd path/to/your/working/path
 python
 import aioTrends as at
 ```
-7. Amend the settings.json under the folder settings.
-8. Paste proxies to the proxies.txt under the folder proxies.
-9. Get userAgents.json file from [Said-Ait-Driss](https://github.com/Said-Ait-Driss/user-agents) and past it under
+7. Amend the settings.json under the folder 'settings'.
+8. Paste proxies to the proxies.txt under the folder 'proxies'.
+9. Get userAgents.json file from [Said-Ait-Driss](https://github.com/Said-Ait-Driss/user-agents) and past it under the folder 'settings'.
 
 ## Getting Started
 ### II. Setup a queries file
 
 ```python
 import pickle
 qrys = {
@@ -92,16 +111,18 @@
 
 pickle.dump(qrys, open('./data/qrys.pkl', 'wb'))
 ```
 
 Alternatively, function ```formQueries``` would form the query dataset based on the list of keywords you give.
 ```python
 from aioTrends import formQueries
+from datetime import date
+import pickle
 
-qrys = formQueries(keywords: ['AMZN', 'MSFN'], start='2004-01-01', end=date.today(), freq: str='D')
+qrys = formQueries(keywords=['AMZN', 'MSFN'], start='2004-01-01', end=date.today(), freq='D')
 pickle.dump(qrys, open('./data/qrys.pkl', 'wb'))
 ```
 
 ### III. Create a py script named as example.py
 
 ```python
 import aioTrends as at
@@ -121,28 +142,39 @@
 
 Alternatively, you can use below one line for forming queries and getting daily scaled data or monthly data.
 ```python
 
 import aioTrends as at
 from datetime import date
 
-qry_list = ['AMZN', 'MSFN']
+qry_list = ['AMZN', 'AAPL', 'MSFT']
 
-# running 100 cocurrent tasks
-df = at.Aio(100).getScaledDailyData(
+# running 50 cocurrent tasks
+ataio = at.Aio(50)
+
+df = ataio.getScaledDailyData(
     keywords=qry_list, # the query keyword list
-    filename='output.csv', # json and pickle are both supported
+    filename='test.csv', # json and pickle are both supported
     start='2004-01-01', # both datetime and str are supported
     end=date.today()
     )
-print(df)
 
-df_m = at.Aio(50).getMonthlyData(keywords=qry_list, start='2004-01-01', end='2022-12-31')
-print(df_m)
+fig = df.plot(figsize=(16,8), title='TEST_SCALED_DAILY_DATA').get_figure()
+fig.savefig('test_scaled_daily_data.png')
+
+df_m = ataio.getMonthlyData(
+    keywords=qry_list, 
+    start='2004-01-01', 
+    end='2022-12-31'
+    )
+fig = df_m.plot(figsize=(16,8), title='TEST_MONTHLY_DATA').get_figure()
+fig.savefig('test_monthly_data.png')
 ```
 
 ### IV. Run the above example.py file on your terminal or cmd (The code need to be running under the python 3.10+ environment)
 
 ```consol
 python example.py
 ```
 
+![Monthly Data](test_monthly_data.png)
+![Scaled Daily Data](test_scaled_daily_data.png)
```

### Comparing `aioTrends-0.0.0/setup.py` & `aioTrends-0.0.2/aioTrends/SETUP.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="aioTrends",
     packages=["aioTrends"],
-    version="0.0.0",
+    version="0.0.2",
     license="MIT",
     description="Library for fetching Google Trends in an async. way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Stephen Zhang",
     author_email="stephen_se@outlook.com",
     url="https://github.com/yuz0101/aioTrends",
-    download_url='https://github.com/yuz0101/aioTrends/archive/refs/tags/v_01.tar.gz',
+    download_url='https://github.com/yuz0101/aioTrends/archive/refs/tags/v_02.tar.gz',
     keywords=['google', 'trends', 'async', 'asyncio', 'aiohttp', 'googletrends', 'pytrends'],
-    install_requires=["numpy", "pandas", "requests", "aiohttp", "aiofiles", "colorama"],
+    install_requires=["numpy", "pandas", "requests", "aiohttp", "aiofiles", "colorama", "matplotlib"],
     
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent"
```

