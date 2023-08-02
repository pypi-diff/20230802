# Comparing `tmp/openhexa.toolbox-0.1.3.tar.gz` & `tmp/openhexa.toolbox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.toolbox-0.1.3.tar", last modified: Tue Aug  1 10:50:16 2023, max compression
+gzip compressed data, was "openhexa.toolbox-0.1.4.tar", last modified: Wed Aug  2 13:02:00 2023, max compression
```

## Comparing `openhexa.toolbox-0.1.3.tar` & `openhexa.toolbox-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.907546 openhexa.toolbox-0.1.4/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29336 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/tests/test_lib.py
```

### Comparing `openhexa.toolbox-0.1.3/LICENSE` & `openhexa.toolbox-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.3/PKG-INFO` & `openhexa.toolbox-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/api.py` & `openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/dhis2.py` & `openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/dhis2.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         connection : openhexa DHIS2Connection
             An initialized openhexa dhis2 connection
         cache_dir : str, optional
             Cache directory. Actual cache data will be stored under a sub-directory
             named after the DHIS2 instance domain.
         """
         self.api = Api(connection)
-        self.cache_dir = self.setup_cache(cache_dir)
+        if cache_dir:
+            self.cache_dir = self.setup_cache(cache_dir)
         self.meta = Metadata(self)
         self.version = self.meta.system_info().get("version")
         self.data_value_sets = DataValueSets(self)
         self.analytics = Analytics(self)
 
     def setup_cache(self, cache_dir: str):
         """Initialize diskcache."""
@@ -123,24 +124,14 @@
                         "level": ou.get("level"),
                         "path": ou.get("path"),
                         "geometry": json.dumps(ou.get("geometry")) if ou.get("geometry") else None,
                     }
                 )
         return org_units
 
-    @staticmethod
-    def add_parent_organisation_units(org_unit_id: str) -> pl.DataFrame:
-        """Add full org unit hierarchy columns.
-
-        Parameters
-        ----------
-
-        """
-        pass
-
     @use_cache("organisation_unit_groups")
     def organisation_unit_groups(self) -> List[dict]:
         """Get organisation unit groups metadata.
 
         Return
         ------
         list of dict
@@ -578,15 +569,15 @@
         if not what:
             raise DHIS2Error("No data dimension provided")
         if not where:
             raise DHIS2Error("No spatial dimension provided")
         if not when:
             raise DHIS2Error("No temporal dimension provided")
 
-        if data_elements and not self.client.version >= 2.39:
+        if data_elements and not self.client.version >= "2.39":
             raise DHIS2Error("Data elements parameter not supported for DHIS2 versions < 2.39")
 
         params = {
             "dataElement": data_elements,
             "dataSet": datasets,
             "dataElementGroup": data_element_groups,
             "period": periods,
@@ -787,15 +778,15 @@
         polars dataframe.
         """
         data_values = []
         for row in response["rows"]:
             data_value = {}
             for i, header in enumerate(response["headers"]):
                 data_value[header["name"]] = row[i]
-                data_values.append(data_value)
+            data_values.append(data_value)
         return data_values
 
     def get(
         self,
         data_elements: List[str] = None,
         data_element_groups: List[str] = None,
         indicators: List[str] = None,
```

### Comparing `openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/periods.py` & `openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/periods.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,32 @@
             dt += self._delta
 
         return prange
 
     def __str__(self):
         return self.period
 
+    def __eq__(self, other):
+        return self.period == other.period
+
+    def __ne__(self, other):
+        return self.period != other.period
+
+    def __gt__(self, other):
+        return self.period > other.period
+
+    def __lt__(self, other):
+        return self.period < other.period
+
+    def __ge__(self, other):
+        return self.period >= other.period
+
+    def __le__(self, other):
+        return self.period <= other.period
+
     def __repr__(self):
         return f'"{self.period}"'
 
 
 class Day(Period):
     """Day.
 
@@ -77,15 +95,16 @@
     @staticmethod
     def check_period(period: str):
         if (len(period) != 6 and len(period) != 7) or period[4] != "W" or period[5] == "0":
             raise ValueError(f'"{period}" is not valid DHIS2 week')
 
     @staticmethod
     def to_datetime(period: str) -> datetime:
-        return datetime.strptime(period, "%YW%W")
+        # a dummy weekday is added so that strptime can be used
+        return datetime.strptime(period + "1", "%YW%W%w")
 
     @staticmethod
     def to_string(dt: datetime) -> str:
         return dt.strftime("%YW%-W")
 
 
 class Month(Period):
@@ -120,15 +139,15 @@
 
     def __init__(self, period: Union[str, datetime]):
         super().__init__(period)
         self._delta = relativedelta(years=1)
 
     @staticmethod
     def check_period(period: str):
-        if len(period) != 6:
+        if len(period) != 4:
             raise ValueError(f'"{period}" is not valid DHIS2 year')
 
     @staticmethod
     def to_datetime(period: str) -> datetime:
         return datetime.strptime(period, "%Y")
 
     @staticmethod
```

### Comparing `openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.3/pyproject.toml` & `openhexa.toolbox-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.1.3"
+version = "0.1.4"
 description = "A set of tools to acquire & process data from various sources"
 authors = [
     { name = "Bluesquare", email = "dev@bluesquarehub.com"}
 ]
 maintainers = [
     { name = "Bluesquare", email = "dev@bluesquarehub.com" }
 ]
```

