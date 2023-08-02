# Comparing `tmp/django_super_svgs-0.1.0.tar.gz` & `tmp/django_super_svgs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_super_svgs-0.1.0.tar", max compression
+gzip compressed data, was "django_super_svgs-0.1.1.tar", max compression
```

## Comparing `django_super_svgs-0.1.0.tar` & `django_super_svgs-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      867 2023-06-22 13:48:15.291565 django_super_svgs-0.1.0/README.md
--rw-r--r--   0        0        0     3645 2023-06-22 15:32:02.601527 django_super_svgs-0.1.0/django_super_svgs/management/commands/create_snippets.py
--rw-r--r--   0        0        0       43 2023-06-01 19:47:16.341491 django_super_svgs-0.1.0/django_super_svgs/static/django_super_svgs/css/main.css
--rw-r--r--   0        0        0     5469 2023-06-22 15:54:08.334507 django_super_svgs-0.1.0/django_super_svgs/templatetags/base.py
--rw-r--r--   0        0        0      218 2023-06-01 19:39:32.102557 django_super_svgs-0.1.0/django_super_svgs/templatetags/super_svgs.py
--rw-r--r--   0        0        0        0 2023-06-01 19:28:10.075504 django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/__init__.py
--rwxr-xr-x   0        0        0   188194 2023-05-04 01:12:35.545042 django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/dripicons.py
--rwxr-xr-x   0        0        0   126226 2023-06-16 17:16:41.506514 django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/hero_outline.py
--rwxr-xr-x   0        0        0   160707 2023-06-16 17:16:38.843205 django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/hero_solid.py
--rw-r--r--   0        0        0        0 2023-06-21 15:56:18.900262 django_super_svgs-0.1.0/django_super_svgs/tests/__init__.py
--rw-r--r--   0        0        0     3269 2023-06-21 19:12:05.126189 django_super_svgs-0.1.0/django_super_svgs/tests/test_snippets.py
--rw-r--r--   0        0        0     3187 2023-06-21 17:57:06.239714 django_super_svgs-0.1.0/django_super_svgs/tests/test_templates.py
--rw-r--r--   0        0        0     2397 2023-06-21 14:12:47.260071 django_super_svgs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 django_super_svgs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-06-22 13:48:15.291565 django_super_svgs-0.1.1/README.md
+-rw-r--r--   0        0        0     3645 2023-06-22 15:32:02.601527 django_super_svgs-0.1.1/django_super_svgs/management/commands/create_snippets.py
+-rw-r--r--   0        0        0       43 2023-06-01 19:47:16.341491 django_super_svgs-0.1.1/django_super_svgs/static/django_super_svgs/css/main.css
+-rw-r--r--   0        0        0     5482 2023-08-02 15:32:26.430827 django_super_svgs-0.1.1/django_super_svgs/templatetags/base.py
+-rw-r--r--   0        0        0      218 2023-06-01 19:39:32.102557 django_super_svgs-0.1.1/django_super_svgs/templatetags/super_svgs.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:28:10.075504 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/__init__.py
+-rw-r--r--   0        0        0  1096583 2023-08-02 14:04:16.955987 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/bootstrap.py
+-rwxr-xr-x   0        0        0   188194 2023-05-04 01:12:35.545042 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/dripicons.py
+-rwxr-xr-x   0        0        0   126226 2023-06-16 17:16:41.506514 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_outline.py
+-rwxr-xr-x   0        0        0   160707 2023-06-16 17:16:38.843205 django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_solid.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:56:18.900262 django_super_svgs-0.1.1/django_super_svgs/tests/__init__.py
+-rw-r--r--   0        0        0     3306 2023-08-02 14:06:05.675151 django_super_svgs-0.1.1/django_super_svgs/tests/test_snippets.py
+-rw-r--r--   0        0        0     3187 2023-06-21 17:57:06.239714 django_super_svgs-0.1.1/django_super_svgs/tests/test_templates.py
+-rw-r--r--   0        0        0     2464 2023-08-02 14:15:58.167981 django_super_svgs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 django_super_svgs-0.1.1/PKG-INFO
```

### Comparing `django_super_svgs-0.1.0/README.md` & `django_super_svgs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.0/django_super_svgs/management/commands/create_snippets.py` & `django_super_svgs-0.1.1/django_super_svgs/management/commands/create_snippets.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.0/django_super_svgs/templatetags/base.py` & `django_super_svgs-0.1.1/django_super_svgs/templatetags/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from django.utils.regex_helper import _lazy_re_compile
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 
 class BaseTemplateTag(Node):
     kwargs_re = _lazy_re_compile(r"(\w+:)?([a-zA-Z-_]+)=(.+)")
-    SVGS_BASE = ["hero_solid", "hero_outline", "dripicons"]
+    SVGS_BASE = ["hero_solid", "hero_outline", "dripicons", "bootstrap"]
     SVG_CONTAINER_CLASS = "svg-container"
     ERROR_MSG = _(
         'The svg tag requires a svg filename followed by svg name and optionally followed by a list of attributes and values like attr="value"'
     )
 
     def __init__(self, parser, token):
         self.parser = parser
```

### Comparing `django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/dripicons.py` & `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/dripicons.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/hero_outline.py` & `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_outline.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.0/django_super_svgs/templatetags/svgs/hero_solid.py` & `django_super_svgs-0.1.1/django_super_svgs/templatetags/svgs/hero_solid.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.0/django_super_svgs/tests/test_snippets.py` & `django_super_svgs-0.1.1/django_super_svgs/tests/test_snippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         out = StringIO()
         path = pathlib.Path("snipp")
         call_command(
             "create_snippets", builtins=True, output="snipp", stdout=out
         )
 
         files = [
+            path / "bootstrap.json",
             path / "dripicons.json",
             path / "hero_outline.json",
             path / "hero_solid.json",
             path / "mycustomsvg.json",
             path / "package.json",
         ]
```

### Comparing `django_super_svgs-0.1.0/django_super_svgs/tests/test_templates.py` & `django_super_svgs-0.1.1/django_super_svgs/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django_super_svgs-0.1.0/pyproject.toml` & `django_super_svgs-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "django-super-svgs"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool for render svg templates using Django templatetags."
 authors = ["Lucas F. <lucas@lucasf.dev>"]
 readme = "README.md"
 packages = [{include = "django_super_svgs"}]
-license = "BSD 3-Clause"
+license = "BSD-3-Clause"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha" ,
   "Environment :: Web Environment",
   "Framework :: Django",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
@@ -23,15 +23,14 @@
   "Topic :: Internet",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development",
-
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = "^4.2.1"
 
 [tool.poetry.group.doc.dependencies]
@@ -46,17 +45,18 @@
 python-decouple = "^3.8"
 dj-database-url = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[project.urls]
+[tools.poetry.urls]
 Homepage = "https://gitlab.com/lucasf_dev/django-super-svgs"
 Documentation = "https://lucasf_dev.gitlab.io/django-super-svgs/"
+Repository = "https://gitlab.com/lucasf_dev/django-super-svgs"
 
 [tool.isort]
 profile = "black"
 line_length = 79
 multi_line_output = 2
 include_trailing_comma = false
 extend_skip = '''
```

### Comparing `django_super_svgs-0.1.0/PKG-INFO` & `django_super_svgs-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 Metadata-Version: 2.1
 Name: django-super-svgs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for render svg templates using Django templatetags.
-License: BSD 3-Clause
+License: BSD-3-Clause
 Author: Lucas F.
 Author-email: lucas@lucasf.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

