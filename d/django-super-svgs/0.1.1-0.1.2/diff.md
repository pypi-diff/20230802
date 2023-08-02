# Comparing `tmp/django_super_svgs-0.1.1.tar.gz` & `tmp/django_super_svgs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_super_svgs-0.1.1.tar", max compression
+gzip compressed data, was "django_super_svgs-0.1.2.tar", max compression
```

## Comparing `django_super_svgs-0.1.1.tar` & `django_super_svgs-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      867 2023-06-22 13:48:15.291565 django_super_svgs-0.1.1/README.md
--rw-r--r--   0        0        0     3645 2023-06-22 15:32:02.601527 django_super_svgs-0.1.1/django_super_svgs/management/commands/create_snippets.py
--rw-r--r--   0        0        0       43 2023-06-01 19:47:16.341491 django_super_svgs-0.1.1/django_super_svgs/static/django_super_svgs/css/main.css
--rw-r--r--   0        0        0     5482 2023-08-02 15:32:26.430827 django_super_svgs-0.1.1/django_super_svgs/templatetags/base.py
--rw-r--r--   0        0        0      218 2023-06-01 19:39:32.102557 django_super_svgs-0.1.1/django_super_svgs/templatetags/super_svgs.py
--rw-r--r--   0        0        0        0 2023-06-01 19:28:10.075504 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/__init__.py
--rw-r--r--   0        0        0  1096583 2023-08-02 14:04:16.955987 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/bootstrap.py
--rwxr-xr-x   0        0        0   188194 2023-05-04 01:12:35.545042 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/dripicons.py
--rwxr-xr-x   0        0        0   126226 2023-06-16 17:16:41.506514 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_outline.py
--rwxr-xr-x   0        0        0   160707 2023-06-16 17:16:38.843205 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_solid.py
--rw-r--r--   0        0        0        0 2023-06-21 15:56:18.900262 django_super_svgs-0.1.1/django_super_svgs/tests/__init__.py
--rw-r--r--   0        0        0     3306 2023-08-02 14:06:05.675151 django_super_svgs-0.1.1/django_super_svgs/tests/test_snippets.py
--rw-r--r--   0        0        0     3187 2023-06-21 17:57:06.239714 django_super_svgs-0.1.1/django_super_svgs/tests/test_templates.py
--rw-r--r--   0        0        0     2464 2023-08-02 14:15:58.167981 django_super_svgs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 django_super_svgs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1514 2023-08-02 21:16:15.762987 django_super_svgs-0.1.2/LICENSE
+-rw-r--r--   0        0        0      925 2023-08-02 21:16:15.762987 django_super_svgs-0.1.2/README.md
+-rw-r--r--   0        0        0     3645 2023-06-22 15:32:02.601527 django_super_svgs-0.1.2/django_super_svgs/management/commands/create_snippets.py
+-rw-r--r--   0        0        0       43 2023-06-01 19:47:16.341491 django_super_svgs-0.1.2/django_super_svgs/static/django_super_svgs/css/main.css
+-rw-r--r--   0        0        0     5482 2023-08-02 15:32:26.430827 django_super_svgs-0.1.2/django_super_svgs/templatetags/base.py
+-rw-r--r--   0        0        0      218 2023-06-01 19:39:32.102557 django_super_svgs-0.1.2/django_super_svgs/templatetags/super_svgs.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:28:10.075504 django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/__init__.py
+-rw-r--r--   0        0        0  1096583 2023-08-02 14:04:16.955987 django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/bootstrap.py
+-rwxr-xr-x   0        0        0   188194 2023-05-04 01:12:35.545042 django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/dripicons.py
+-rwxr-xr-x   0        0        0   126226 2023-06-16 17:16:41.506514 django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/hero_outline.py
+-rwxr-xr-x   0        0        0   160707 2023-06-16 17:16:38.843205 django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/hero_solid.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:56:18.900262 django_super_svgs-0.1.2/django_super_svgs/tests/__init__.py
+-rw-r--r--   0        0        0     3306 2023-08-02 14:06:05.675151 django_super_svgs-0.1.2/django_super_svgs/tests/test_snippets.py
+-rw-r--r--   0        0        0     3187 2023-06-21 17:57:06.239714 django_super_svgs-0.1.2/django_super_svgs/tests/test_templates.py
+-rw-r--r--   0        0        0     2464 2023-08-02 21:18:40.640955 django_super_svgs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 django_super_svgs-0.1.2/PKG-INFO
```

### Comparing `django_super_svgs-0.1.1/README.md` & `django_super_svgs-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 )
 ```
 
 ## Usage
 
 By default `django-super-svgs` provides these svgs:
 
+- [bootstrap](https://icons.getbootstrap.com/)
 - [dripicons](http://demo.amitjakhu.com/dripicons/)
 - [heroicons](https://heroicons.com/)
 
-Load the tag `super_svgs` in your html file, then use `svg` followed by `svg type` [ dripicons, hero_outline, hero_solid ] and `svg name`:
+Load the tag `super_svgs` in your html file, then use `svg` followed by `svg type` [ bootstrap, dripicons, hero_outline, hero_solid ] and `svg name`:
 
 ```htmldjango
 {% load super_svgs %}
 
 {% svg hero_outline check_circle %}
 ```
```

### Comparing `django_super_svgs-0.1.1/django_super_svgs/management/commands/create_snippets.py` & `django_super_svgs-0.1.2/django_super_svgs/management/commands/create_snippets.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/templatetags/base.py` & `django_super_svgs-0.1.2/django_super_svgs/templatetags/base.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/bootstrap.py` & `django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/dripicons.py` & `django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/dripicons.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_outline.py` & `django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/hero_outline.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_solid.py` & `django_super_svgs-0.1.2/django_super_svgs/templatetags/svgs/hero_solid.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/tests/test_snippets.py` & `django_super_svgs-0.1.2/django_super_svgs/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/django_super_svgs/tests/test_templates.py` & `django_super_svgs-0.1.2/django_super_svgs/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.1/pyproject.toml` & `django_super_svgs-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-super-svgs"
-version = "0.1.1"
+version = "0.1.2"
 description = "A tool for render svg templates using Django templatetags."
 authors = ["Lucas F. <lucas@lucasf.dev>"]
 readme = "README.md"
 packages = [{include = "django_super_svgs"}]
 license = "BSD-3-Clause"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha" ,
```

### Comparing `django_super_svgs-0.1.1/PKG-INFO` & `django_super_svgs-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-super-svgs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for render svg templates using Django templatetags.
 License: BSD-3-Clause
 Author: Lucas F.
 Author-email: lucas@lucasf.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
@@ -58,18 +58,19 @@
 )
 ```
 
 ## Usage
 
 By default `django-super-svgs` provides these svgs:
 
+- [bootstrap](https://icons.getbootstrap.com/)
 - [dripicons](http://demo.amitjakhu.com/dripicons/)
 - [heroicons](https://heroicons.com/)
 
-Load the tag `super_svgs` in your html file, then use `svg` followed by `svg type` [ dripicons, hero_outline, hero_solid ] and `svg name`:
+Load the tag `super_svgs` in your html file, then use `svg` followed by `svg type` [ bootstrap, dripicons, hero_outline, hero_solid ] and `svg name`:
 
 ```htmldjango
 {% load super_svgs %}
 
 {% svg hero_outline check_circle %}
 ```
```

