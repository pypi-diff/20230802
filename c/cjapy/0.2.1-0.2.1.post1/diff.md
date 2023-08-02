# Comparing `tmp/cjapy-0.2.1.tar.gz` & `tmp/cjapy-0.2.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjapy-0.2.1.tar", last modified: Wed Jul  5 20:21:31 2023, max compression
+gzip compressed data, was "cjapy-0.2.1.post1.tar", last modified: Wed Aug  2 11:57:14 2023, max compression
```

## Comparing `cjapy-0.2.1.tar` & `cjapy-0.2.1.post1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.350092 cjapy-0.2.1/
--rw-rw-rw-   0        0        0    10337 2021-10-20 19:50:41.000000 cjapy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3565 2023-07-05 20:21:31.348097 cjapy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2469 2021-11-08 18:46:39.000000 cjapy-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.307878 cjapy-0.2.1/cjapy/
--rw-rw-rw-   0        0        0      107 2021-10-20 19:50:41.000000 cjapy-0.2.1/cjapy/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-05 06:14:05.000000 cjapy-0.2.1/cjapy/__version__.py
--rw-rw-rw-   0        0        0   109187 2023-07-05 09:31:15.000000 cjapy-0.2.1/cjapy/cjapy.py
--rw-rw-rw-   0        0        0      566 2023-06-26 06:55:22.000000 cjapy-0.2.1/cjapy/config.py
--rw-rw-rw-   0        0        0     7666 2023-06-26 06:48:55.000000 cjapy-0.2.1/cjapy/configs.py
--rw-rw-rw-   0        0        0    12821 2023-07-05 07:30:15.000000 cjapy-0.2.1/cjapy/connector.py
--rw-rw-rw-   0        0        0    12007 2021-11-08 18:46:39.000000 cjapy-0.2.1/cjapy/projects.py
--rw-rw-rw-   0        0        0    17279 2023-07-05 07:30:01.000000 cjapy-0.2.1/cjapy/requestCreator.py
--rw-rw-rw-   0        0        0     3463 2023-06-26 09:22:08.000000 cjapy-0.2.1/cjapy/token_provider.py
--rw-rw-rw-   0        0        0     9415 2023-07-05 06:15:53.000000 cjapy-0.2.1/cjapy/workspace.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.320064 cjapy-0.2.1/cjapy.egg-info/
--rw-rw-rw-   0        0        0     3565 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.346386 cjapy-0.2.1/docs/
--rw-rw-rw-   0        0        0     1805 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/authenticating_without_config_json.md
--rw-rw-rw-   0        0        0    27971 2023-05-11 12:56:12.000000 cjapy-0.2.1/docs/cja.md
--rw-rw-rw-   0        0        0     3664 2023-06-26 06:49:51.000000 cjapy-0.2.1/docs/getting_started.md
--rw-rw-rw-   0        0        0     3934 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/logging.md
--rw-rw-rw-   0        0        0     3335 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/main.md
--rw-rw-rw-   0        0        0     8595 2021-11-08 18:46:39.000000 cjapy-0.2.1/docs/projects.md
--rw-rw-rw-   0        0        0     1477 2023-07-05 07:15:10.000000 cjapy-0.2.1/docs/releases.md
--rw-rw-rw-   0        0        0     6126 2021-11-08 18:46:39.000000 cjapy-0.2.1/docs/requestCreator.md
--rw-rw-rw-   0        0        0     3348 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/workspace.md
--rw-rw-rw-   0        0        0     1364 2023-06-26 13:49:26.000000 cjapy-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      100 2021-10-20 19:50:41.000000 cjapy-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 20:21:31.350092 cjapy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1871 2021-10-20 19:50:41.000000 cjapy-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:57:14.930097 cjapy-0.2.1.post1/
+-rw-rw-rw-   0        0        0    10337 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/LICENSE
+-rw-rw-rw-   0        0        0     3571 2023-08-02 11:57:14.927277 cjapy-0.2.1.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2469 2021-11-08 18:46:39.000000 cjapy-0.2.1.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 11:57:14.723577 cjapy-0.2.1.post1/cjapy/
+-rw-rw-rw-   0        0        0      107 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/cjapy/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-08-02 11:50:16.000000 cjapy-0.2.1.post1/cjapy/__version__.py
+-rw-rw-rw-   0        0        0   109187 2023-08-02 10:06:13.000000 cjapy-0.2.1.post1/cjapy/cjapy.py
+-rw-rw-rw-   0        0        0      566 2023-06-26 06:55:22.000000 cjapy-0.2.1.post1/cjapy/config.py
+-rw-rw-rw-   0        0        0     7666 2023-06-26 06:48:55.000000 cjapy-0.2.1.post1/cjapy/configs.py
+-rw-rw-rw-   0        0        0    12821 2023-07-05 07:30:15.000000 cjapy-0.2.1.post1/cjapy/connector.py
+-rw-rw-rw-   0        0        0    12007 2021-11-08 18:46:39.000000 cjapy-0.2.1.post1/cjapy/projects.py
+-rw-rw-rw-   0        0        0    17481 2023-08-02 08:44:50.000000 cjapy-0.2.1.post1/cjapy/requestCreator.py
+-rw-rw-rw-   0        0        0     3463 2023-06-26 09:22:08.000000 cjapy-0.2.1.post1/cjapy/token_provider.py
+-rw-rw-rw-   0        0        0     9487 2023-08-02 08:57:05.000000 cjapy-0.2.1.post1/cjapy/workspace.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:57:14.764569 cjapy-0.2.1.post1/cjapy.egg-info/
+-rw-rw-rw-   0        0        0     3571 2023-08-02 11:57:13.000000 cjapy-0.2.1.post1/cjapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-08-02 11:57:14.000000 cjapy-0.2.1.post1/cjapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:57:13.000000 cjapy-0.2.1.post1/cjapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-02 11:57:13.000000 cjapy-0.2.1.post1/cjapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 11:57:13.000000 cjapy-0.2.1.post1/cjapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 11:57:14.910811 cjapy-0.2.1.post1/docs/
+-rw-rw-rw-   0        0        0     1805 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/docs/authenticating_without_config_json.md
+-rw-rw-rw-   0        0        0    27971 2023-05-11 12:56:12.000000 cjapy-0.2.1.post1/docs/cja.md
+-rw-rw-rw-   0        0        0     3664 2023-06-26 06:49:51.000000 cjapy-0.2.1.post1/docs/getting_started.md
+-rw-rw-rw-   0        0        0     3934 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/docs/logging.md
+-rw-rw-rw-   0        0        0     3335 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/docs/main.md
+-rw-rw-rw-   0        0        0     8595 2021-11-08 18:46:39.000000 cjapy-0.2.1.post1/docs/projects.md
+-rw-rw-rw-   0        0        0     1584 2023-08-02 11:51:30.000000 cjapy-0.2.1.post1/docs/releases.md
+-rw-rw-rw-   0        0        0     6465 2023-08-02 11:55:47.000000 cjapy-0.2.1.post1/docs/requestCreator.md
+-rw-rw-rw-   0        0        0     3348 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/docs/workspace.md
+-rw-rw-rw-   0        0        0     1364 2023-06-26 13:49:26.000000 cjapy-0.2.1.post1/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 11:57:14.930740 cjapy-0.2.1.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1871 2021-10-20 19:50:41.000000 cjapy-0.2.1.post1/setup.py
```

### Comparing `cjapy-0.2.1/LICENSE` & `cjapy-0.2.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/PKG-INFO` & `cjapy-0.2.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjapy
-Version: 0.2.1
+Version: 0.2.1.post1
 Summary: Adobe Customer Journey Analytics (CJA) wrapper
 Home-page: https://github.com/pitchmuc/cjapy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/cjapy
 Project-URL: changelog, https://github.com/pitchmuc/cjapy/blob/master/docs/releases.md
```

### Comparing `cjapy-0.2.1/README.md` & `cjapy-0.2.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/cjapy.py` & `cjapy-0.2.1.post1/cjapy/cjapy.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/config.py` & `cjapy-0.2.1.post1/cjapy/config.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/configs.py` & `cjapy-0.2.1.post1/cjapy/configs.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/connector.py` & `cjapy-0.2.1.post1/cjapy/connector.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/projects.py` & `cjapy-0.2.1.post1/cjapy/projects.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/requestCreator.py` & `cjapy-0.2.1.post1/cjapy/requestCreator.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
                     request = json.load(f)
         self.__request = deepcopy(request) or deepcopy(self.template)
         self.__metricCount = len(self.__request["metricContainer"]["metrics"])
         self.__metricFilterCount = len(
             self.__request["metricContainer"].get("metricFilters", [])
         )
         self.__globalFiltersCount = len(self.__request["globalFilters"])
+        self.search = False ## defining if search is being used.
+        if 'search' in self.__request.keys():
+            self.search = True
         ### Preparing some time statement.
         today = datetime.datetime.now()
         today_date_iso = today.isoformat().split("T")[0]
         ## should give '20XX-XX-XX'
         tomorrow_date_iso = (
             (today + datetime.timedelta(days=1)).isoformat().split("T")[0]
         )
@@ -214,20 +217,22 @@
         Set the items ID search in the specified dimension
         Arguments :
             itemIds : REQUIRED : The list of itemId to be searched in the dimension
         """
         if type(itemIds) != list:
             raise TypeError("itemIds should be a list of values")
         self.__request["search"]["itemIds"] = itemIds
+        self.search = True
     
     def removeSearch(self)->None:
         """
         Remove the search capability in the request.
         """
         del self.__request["search"]
+        self.search = False
 
 
     def setRepeatInstance(self, repeat: bool = True) -> None:
         """
         Specify if repeated instances should be counted.
         Arguments:
             repeat : OPTIONAL : True or False (True by default)
```

### Comparing `cjapy-0.2.1/cjapy/token_provider.py` & `cjapy-0.2.1.post1/cjapy/token_provider.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/cjapy/workspace.py` & `cjapy-0.2.1.post1/cjapy/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,16 @@
             row: pd.Series = self.dataframe[self.dataframe.iloc[:, 1] == index]
             itemValue: str = row["itemId"].values[0]
         elif type(index) == int:
             itemValue = self.dataframe.loc[index, "itemId"]
         breakdown = f"{breadown_dimension}:::{itemValue}"
         new_request = RequestCreator(self.dataRequest.to_dict())
         new_request.setDimension(dimension)
+        if new_request.search:
+            new_request.removeSearch()
         metrics = new_request.getMetrics()
         for metric in metrics:
             new_request.addMetricFilter(metricId=metric, filterId=breakdown)
         if n_results < 20000:
             new_request.setLimit(n_results)
             report = self.cjaConnector.getReport(
                 new_request.to_dict(), n_results=n_results
```

### Comparing `cjapy-0.2.1/cjapy.egg-info/PKG-INFO` & `cjapy-0.2.1.post1/cjapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjapy
-Version: 0.2.1
+Version: 0.2.1.post1
 Summary: Adobe Customer Journey Analytics (CJA) wrapper
 Home-page: https://github.com/pitchmuc/cjapy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/cjapy
 Project-URL: changelog, https://github.com/pitchmuc/cjapy/blob/master/docs/releases.md
```

### Comparing `cjapy-0.2.1/cjapy.egg-info/SOURCES.txt` & `cjapy-0.2.1.post1/cjapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/authenticating_without_config_json.md` & `cjapy-0.2.1.post1/docs/authenticating_without_config_json.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/cja.md` & `cjapy-0.2.1.post1/docs/cja.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/getting_started.md` & `cjapy-0.2.1.post1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/logging.md` & `cjapy-0.2.1.post1/docs/logging.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/main.md` & `cjapy-0.2.1.post1/docs/main.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/projects.md` & `cjapy-0.2.1.post1/docs/projects.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/docs/releases.md` & `cjapy-0.2.1.post1/docs/releases.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 The changes have been tracked starting version 0.1.0
 
 ## 0.2.1
 
 * requestCreator can now set `setSearch` and `removeSearch`
 * avoiding modifying initial request from `getReport` 
 * fixing report output decryption from `getReport`
-* adding throwing an `TimeoutError` when API Gateway of CJA is not responding.
+* adding throwing an `TimeoutError` when API Gateway of CJA is not responding.\
+Patch : 
+* Fixing `breakdown` method in `Workspace` class to support when result is coming from search.
 
 ## 0.2.0
 
 * adding support for Oauth Server to Server configuration file
   * adding support for `createConfigFile`
   * adding support for `importConfigFile` and `configure`
 * moving to pyproject.toml release
```

### Comparing `cjapy-0.2.1/docs/requestCreator.md` & `cjapy-0.2.1.post1/docs/requestCreator.md`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,23 @@
   * repeat : OPTIONAL : True or False (True by default)
 
 * `setLimit()`
   Specific the number of element to retrieve. Default is 10.
   Arguments:
   * limit : OPTIONAL : number of elements to return
 
+* `setSearch()`
+  Set a search for specific value in the dimensions.
+  Arguments:
+  * itemIds : REQUIRED : list of value to search for.
+
+* `removeSearch()`
+  Remove the search attribute for the search capabilities.
+  No arguments.
+
 * `addMetricFilter()`
   Add a filter to a metric.
   Arguments:
   * metricId : REQUIRED : metric where the filter is added
   * filterId : REQUIRED : The filter to add.
     When breakdown, use the following format for the value "dimension:::itemId"
   * metricIndex : OPTIONAL : If used, set the filter to the metric located on that index.
@@ -151,7 +160,11 @@
 * last7daysTillToday
 * last7daysTodayIncluded
 
 ### today
 
 `today`attribute is a datetime object, with today timestamp.\
 This can help you derive other dates if needed.
+
+### search
+
+`search` attribute is a boolean defining if search has been set for the dimension.
```

### Comparing `cjapy-0.2.1/docs/workspace.md` & `cjapy-0.2.1.post1/docs/workspace.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/pyproject.toml` & `cjapy-0.2.1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.1/setup.py` & `cjapy-0.2.1.post1/setup.py`

 * *Files identical despite different names*

