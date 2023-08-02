# Comparing `tmp/openedx-filters-1.4.0.tar.gz` & `tmp/openedx-filters-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-filters-1.4.0.tar", last modified: Tue Jul 18 15:46:02 2023, max compression
+gzip compressed data, was "openedx-filters-1.5.0.tar", last modified: Wed Aug  2 16:29:39 2023, max compression
```

## Comparing `openedx-filters-1.4.0.tar` & `openedx-filters-1.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9986 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23553 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters/learning/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19937 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/tests/test_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/openedx_filters/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9986 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-18 15:46:02.000000 openedx-filters-1.4.0/openedx_filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2867 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/tests/test_openedx_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10167 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/openedx_filters/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24267 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/learning/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/openedx_filters/learning/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/learning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20545 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/learning/tests/test_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/openedx_filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/openedx_filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/openedx_filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10167 2023-08-02 16:29:39.000000 openedx-filters-1.5.0/openedx_filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-08-02 16:29:39.000000 openedx-filters-1.5.0/openedx_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:29:39.000000 openedx-filters-1.5.0/openedx_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:29:39.000000 openedx-filters-1.5.0/openedx_filters.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-02 16:29:39.000000 openedx-filters-1.5.0/openedx_filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-08-02 16:29:39.000000 openedx-filters-1.5.0/openedx_filters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2867 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:29:39.765030 openedx-filters-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-08-02 16:29:35.000000 openedx-filters-1.5.0/tests/test_openedx_filters.py
```

### Comparing `openedx-filters-1.4.0/CHANGELOG.rst` & `openedx-filters-1.5.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[1.5.0] - 2023-07-19
+--------------------
+
+Added
+~~~~~
+
+* CourseEnrollmentAPIRenderStarted filter added which can be used to modify the isStarted B2C dashboard rendering process.
+
+
 [1.4.0] - 2023-07-18
 --------------------
 
 Added
 ~~~~~
 
 * InstructorDashboardRenderStarted filter added which can be used to modify the instructor dashboard rendering process.
```

### Comparing `openedx-filters-1.4.0/LICENSE.txt` & `openedx-filters-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/PKG-INFO` & `openedx-filters-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.4.0
+Version: 1.5.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -210,14 +210,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[1.5.0] - 2023-07-19
+--------------------
+
+Added
+~~~~~
+
+* CourseEnrollmentAPIRenderStarted filter added which can be used to modify the isStarted B2C dashboard rendering process.
+
+
 [1.4.0] - 2023-07-18
 --------------------
 
 Added
 ~~~~~
 
 * InstructorDashboardRenderStarted filter added which can be used to modify the instructor dashboard rendering process.
```

### Comparing `openedx-filters-1.4.0/README.rst` & `openedx-filters-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/exceptions.py` & `openedx-filters-1.5.0/openedx_filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/filters.py` & `openedx-filters-1.5.0/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/learning/filters.py` & `openedx-filters-1.5.0/openedx_filters/learning/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -587,14 +587,34 @@
             course_key (CourseKey): The course key for which the home url is being requested.
             course_home_url (String): The url string for the course home
         """
         data = super().run_pipeline(course_key=course_key, course_home_url=course_home_url)
         return data.get("course_key"), data.get("course_home_url")
 
 
+class CourseEnrollmentAPIRenderStarted(OpenEdxPublicFilter):
+    """
+    Custom class used to create filters for enrollment data.
+    """
+
+    filter_type = "org.openedx.learning.home.enrollment.api.rendered.v1"
+
+    @classmethod
+    def run_filter(cls, course_key, serialized_enrollment):
+        """
+        Execute a filter with the specified signature.
+
+        Arguments:
+            course_key (CourseKey): The course key for which isStarted is being modify.
+            serialized_enrollment (dict): enrollment data
+        """
+        data = super().run_pipeline(course_key=course_key, serialized_enrollment=serialized_enrollment)
+        return data.get("course_key"), data.get("serialized_enrollment")
+
+
 class InstructorDashboardRenderStarted(OpenEdxPublicFilter):
     """
     Custom class used to create instructor dashboard filters and its custom methods.
     """
 
     filter_type = "org.openedx.learning.instructor.dashboard.render.started.v1"
```

### Comparing `openedx-filters-1.4.0/openedx_filters/learning/tests/test_filters.py` & `openedx-filters-1.5.0/openedx_filters/learning/tests/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from openedx_filters.learning.filters import (
     AccountSettingsRenderStarted,
     CertificateCreationRequested,
     CertificateRenderStarted,
     CohortAssignmentRequested,
     CohortChangeRequested,
     CourseAboutRenderStarted,
+    CourseEnrollmentAPIRenderStarted,
     CourseEnrollmentQuerysetRequested,
     CourseEnrollmentStarted,
     CourseHomeUrlCreationStarted,
     CourseUnenrollmentStarted,
     DashboardRenderStarted,
     InstructorDashboardRenderStarted,
     StudentLoginRequested,
@@ -600,7 +601,21 @@
             - The filter should return course_key and course_home_url in that order.
         """
         course_key, course_home_url = Mock(), Mock()
 
         result = CourseHomeUrlCreationStarted.run_filter(course_key, course_home_url)
 
         self.assertTupleEqual((course_key, course_home_url,), result)
+
+    def test_course_enrollment_api_render_started(self):
+        """
+        Test CourseEnrollmentAPIRenderStarted filter behavior under normal conditions.
+
+        Expected behavior:
+            - The filter must have the signature specified.
+            - The filter should return course_key and is_started in that order.
+        """
+        course_key, serialized_enrollment = Mock(), Mock()
+
+        result = CourseEnrollmentAPIRenderStarted.run_filter(course_key, serialized_enrollment)
+
+        self.assertTupleEqual((course_key, serialized_enrollment,), result)
```

### Comparing `openedx-filters-1.4.0/openedx_filters/tests/test_exceptions.py` & `openedx-filters-1.5.0/openedx_filters/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/tests/test_filters.py` & `openedx-filters-1.5.0/openedx_filters/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/tests/test_tooling.py` & `openedx-filters-1.5.0/openedx_filters/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/tooling.py` & `openedx-filters-1.5.0/openedx_filters/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters/utils.py` & `openedx-filters-1.5.0/openedx_filters/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/openedx_filters.egg-info/PKG-INFO` & `openedx-filters-1.5.0/openedx_filters.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.4.0
+Version: 1.5.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -210,14 +210,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[1.5.0] - 2023-07-19
+--------------------
+
+Added
+~~~~~
+
+* CourseEnrollmentAPIRenderStarted filter added which can be used to modify the isStarted B2C dashboard rendering process.
+
+
 [1.4.0] - 2023-07-18
 --------------------
 
 Added
 ~~~~~
 
 * InstructorDashboardRenderStarted filter added which can be used to modify the instructor dashboard rendering process.
```

### Comparing `openedx-filters-1.4.0/openedx_filters.egg-info/SOURCES.txt` & `openedx-filters-1.5.0/openedx_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.4.0/setup.py` & `openedx-filters-1.5.0/setup.py`

 * *Files identical despite different names*

