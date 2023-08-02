# Comparing `tmp/meringue-1.2.0.dev2.tar.gz` & `tmp/meringue-1.2.0.dev3.tar.gz`

## Comparing `meringue-1.2.0.dev2.tar` & `meringue-1.2.0.dev3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/apps.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/routers.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/docs/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/docs/patchers.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/docs/views.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/conf/__init__.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/actions.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/apps.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/constants.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/drf_fields.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/exceptions.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/generators.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/images.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/properties.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/shortcuts.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/storage.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/templatetags/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/templatetags/m_thumbnails.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/LICENSE
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/README.md
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/apps.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/routers.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/conf/__init__.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/actions.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/apps.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/constants.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/drf_fields.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/exceptions.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/generators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/images.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/properties.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/shortcuts.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/storage.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/templatetags/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/templatetags/m_thumbnails.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/LICENSE
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/README.md
+-rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/PKG-INFO
```

### Comparing `meringue-1.2.0.dev2/meringue/api/routers.py` & `meringue-1.2.0.dev3/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/api/utils.py` & `meringue-1.2.0.dev3/meringue/api/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     Raises:
         Exception: Unknown error type.
 
     Returns:
         Rendered errors.
     """
+
     if isinstance(error_detail, list):
         error_list = [render_error_details(e) for e in error_detail]
         return error_list
 
     elif isinstance(error_detail, ErrorDetail):
         return {
             "message": str(error_detail),
```

### Comparing `meringue-1.2.0.dev2/meringue/api/docs/patchers.py` & `meringue-1.2.0.dev3/meringue/api/docs/patchers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/api/docs/views.py` & `meringue-1.2.0.dev3/meringue/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/conf/__init__.py` & `meringue-1.2.0.dev3/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/conf/default_settings.py` & `meringue-1.2.0.dev3/meringue/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/models.py` & `meringue-1.2.0.dev3/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/query.py` & `meringue-1.2.0.dev3/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/translation.py` & `meringue-1.2.0.dev3/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/upload_handlers.py` & `meringue-1.2.0.dev3/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.2.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.2.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/templatetags/meringue_base.py` & `meringue-1.2.0.dev3/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/utils/crypt.py` & `meringue-1.2.0.dev3/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/utils/datetime.py` & `meringue-1.2.0.dev3/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/core/utils/frontend.py` & `meringue-1.2.0.dev3/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/actions.py` & `meringue-1.2.0.dev3/meringue/thumbnail/actions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/constants.py` & `meringue-1.2.0.dev3/meringue/thumbnail/constants.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/drf_fields.py` & `meringue-1.2.0.dev3/meringue/thumbnail/drf_fields.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/exceptions.py` & `meringue-1.2.0.dev3/meringue/thumbnail/exceptions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/generators.py` & `meringue-1.2.0.dev3/meringue/thumbnail/generators.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/images.py` & `meringue-1.2.0.dev3/meringue/thumbnail/images.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/properties.py` & `meringue-1.2.0.dev3/meringue/thumbnail/properties.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/shortcuts.py` & `meringue-1.2.0.dev3/meringue/thumbnail/shortcuts.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/storage.py` & `meringue-1.2.0.dev3/meringue/thumbnail/storage.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/meringue/thumbnail/templatetags/m_thumbnails.py` & `meringue-1.2.0.dev3/meringue/thumbnail/templatetags/m_thumbnails.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/LICENSE` & `meringue-1.2.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev2/README.md` & `meringue-1.2.0.dev3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,24 @@
 		<img src="https://img.shields.io/badge/types-Mypy-blue.svg" alt="types - Mypy" />
 	</a> -->
 	<a href="https://raw.githubusercontent.com/dd/Meringue/master/LICENSE" target="_blank">
 		<img src="https://img.shields.io/pypi/l/meringue?color=008033" alt="License - GNU Lesser General Public License v3.0" />
 	</a>
 </p>
 
-Full documentation for the project is available at [dd.github.io/Meringue](https://dd.github.io/Meringue/).
-
 Package with various functional (such as mixins, form utils, upload handlers and other) for Django Framework.
 
 This library is a set of various functionality that I use from project to project.
 
 The main task of this package is to clean up this functionality, test it, and also organize the documentation so that colleagues can understand how and what works.
 
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
+Read more in the [documentation](https://dd.github.io/Meringue/).
+
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
 * [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed generating form based on response from api).
 * [ ] Authorization backend for authorization by a pair of email and password.
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
                             ****** Meringue ******
  [PyPI_-_Status] [PyPI_-_Version] [PyPI_-_Downloads]  [PyPI_-_Python_Version]
         [Documentation_-_Release] [Tests_-_Running] [Tests_-_Coverage]
  [Hatch_project] [Material_for_MkDocs] [linting_-_Ruff] [code_style_-_black]
               [License_-_GNU_Lesser_General_Public_License_v3.0]
-Full documentation for the project is available at [dd.github.io/Meringue]
-(https://dd.github.io/Meringue/). Package with various functional (such as
-mixins, form utils, upload handlers and other) for Django Framework. This
-library is a set of various functionality that I use from project to project.
-The main task of this package is to clean up this functionality, test it, and
-also organize the documentation so that colleagues can understand how and what
-works. However, if someone decides to use this functionality in their project,
-and even more so to add functionality or change the implementation to a more
-correct, beautiful or understandable one, I will only be happy, do not worry
-and feel free to write to me by [mail](mailto:dd@manin.space), create an
-[issue](https://github.com/dd/Meringue/issues) or [pull request](https://
-github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
-Roadmap Adding new functionality. Can change. * [ ] [drf](https://www.django-
-rest-framework.org/) serializer serializer for automatic form generation on the
-front when working through rest api. (An npm package on [vuejs](https://
-vuejs.org/) will also be developed generating form based on response from api).
-* [ ] Authorization backend for authorization by a pair of email and password.
-* [ ] Functionality for working with images. * [x] Image editor like
-easy_thumbnails. * [x] A field for the drf serializer that returns a set of
-images (for example, a standard image and a double-sized image for a retina
-screen), as well as in different formats (for example, in the original format
-and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs * [ ]
-Functionality similar to that described in the previous paragraph only for
+Package with various functional (such as mixins, form utils, upload handlers
+and other) for Django Framework. This library is a set of various functionality
+that I use from project to project. The main task of this package is to clean
+up this functionality, test it, and also organize the documentation so that
+colleagues can understand how and what works. However, if someone decides to
+use this functionality in their project, and even more so to add functionality
+or change the implementation to a more correct, beautiful or understandable
+one, I will only be happy, do not worry and feel free to write to me by [mail]
+(mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/
+issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github]
+(https://github.com/dd/Meringue). Read more in the [documentation](https://
+dd.github.io/Meringue/). ## Roadmap Adding new functionality. Can change. * [ ]
+[drf](https://www.django-rest-framework.org/) serializer serializer for
+automatic form generation on the front when working through rest api. (An npm
+package on [vuejs](https://vuejs.org/) will also be developed generating form
+based on response from api). * [ ] Authorization backend for authorization by a
+pair of email and password. * [ ] Functionality for working with images. * [x]
+Image editor like easy_thumbnails. * [x] A field for the drf serializer that
+returns a set of images (for example, a standard image and a double-sized image
+for a retina screen), as well as in different formats (for example, in the
+original format and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs *
+[ ] Functionality similar to that described in the previous paragraph only for
 video. * [ ] Functionality for loading private files available through [nginx
 internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal). ##
 Contributing - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-
 flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/
 gitflow-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https:/
 /github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
 github.com/psf/black) - [x] Lint commit with [Gitlint](https://
```

### Comparing `meringue-1.2.0.dev2/pyproject.toml` & `meringue-1.2.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 modeltranslation = ["django-modeltranslation>=0.17,<0.19"]
 drf = ["djangorestframework>=3.13,<4"]
 drf-spectacular = ["drf-spectacular>=0.26.3,<1"]
+cryptodome = ["pycryptodome==3.18.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/dd/Meringue"
 "Documentation" = "https://dd.github.io/Meringue/"
 "Repository" = "https://github.com/dd/Meringue"
 "Changelog" = "https://github.com/dd/Meringue/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/dd/Meringue/issues"
```

### Comparing `meringue-1.2.0.dev2/PKG-INFO` & `meringue-1.2.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.2.0.dev2
+Version: 1.2.0.dev3
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
@@ -43,14 +43,16 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: django>=1.11.17
+Provides-Extra: cryptodome
+Requires-Dist: pycryptodome==3.18.0; extra == 'cryptodome'
 Provides-Extra: drf
 Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
 Provides-Extra: drf-spectacular
 Requires-Dist: drf-spectacular<1,>=0.26.3; extra == 'drf-spectacular'
 Provides-Extra: modeltranslation
 Requires-Dist: django-modeltranslation<0.19,>=0.17; extra == 'modeltranslation'
 Description-Content-Type: text/markdown
@@ -105,24 +107,24 @@
 		<img src="https://img.shields.io/badge/types-Mypy-blue.svg" alt="types - Mypy" />
 	</a> -->
 	<a href="https://raw.githubusercontent.com/dd/Meringue/master/LICENSE" target="_blank">
 		<img src="https://img.shields.io/pypi/l/meringue?color=008033" alt="License - GNU Lesser General Public License v3.0" />
 	</a>
 </p>
 
-Full documentation for the project is available at [dd.github.io/Meringue](https://dd.github.io/Meringue/).
-
 Package with various functional (such as mixins, form utils, upload handlers and other) for Django Framework.
 
 This library is a set of various functionality that I use from project to project.
 
 The main task of this package is to clean up this functionality, test it, and also organize the documentation so that colleagues can understand how and what works.
 
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
+Read more in the [documentation](https://dd.github.io/Meringue/).
+
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
 * [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed generating form based on response from api).
 * [ ] Authorization backend for authorization by a pair of email and password.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.2.0.dev2 Summary: A set of
+Metadata-Version: 2.1 Name: meringue Version: 1.2.0.dev3 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
 dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
 Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
@@ -23,47 +23,47 @@
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet ::
 WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=3.10 Requires-Dist: django>=1.11.17
-Provides-Extra: drf Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
-Provides-Extra: drf-spectacular Requires-Dist: drf-spectacular<1,>=0.26.3;
-extra == 'drf-spectacular' Provides-Extra: modeltranslation Requires-Dist:
-django-modeltranslation<0.19,>=0.17; extra == 'modeltranslation' Description-
-Content-Type: text/markdown
+Provides-Extra: cryptodome Requires-Dist: pycryptodome==3.18.0; extra ==
+'cryptodome' Provides-Extra: drf Requires-Dist: djangorestframework<4,>=3.13;
+extra == 'drf' Provides-Extra: drf-spectacular Requires-Dist: drf-
+spectacular<1,>=0.26.3; extra == 'drf-spectacular' Provides-Extra:
+modeltranslation Requires-Dist: django-modeltranslation<0.19,>=0.17; extra ==
+'modeltranslation' Description-Content-Type: text/markdown
                             ****** Meringue ******
  [PyPI_-_Status] [PyPI_-_Version] [PyPI_-_Downloads]  [PyPI_-_Python_Version]
         [Documentation_-_Release] [Tests_-_Running] [Tests_-_Coverage]
  [Hatch_project] [Material_for_MkDocs] [linting_-_Ruff] [code_style_-_black]
               [License_-_GNU_Lesser_General_Public_License_v3.0]
-Full documentation for the project is available at [dd.github.io/Meringue]
-(https://dd.github.io/Meringue/). Package with various functional (such as
-mixins, form utils, upload handlers and other) for Django Framework. This
-library is a set of various functionality that I use from project to project.
-The main task of this package is to clean up this functionality, test it, and
-also organize the documentation so that colleagues can understand how and what
-works. However, if someone decides to use this functionality in their project,
-and even more so to add functionality or change the implementation to a more
-correct, beautiful or understandable one, I will only be happy, do not worry
-and feel free to write to me by [mail](mailto:dd@manin.space), create an
-[issue](https://github.com/dd/Meringue/issues) or [pull request](https://
-github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
-Roadmap Adding new functionality. Can change. * [ ] [drf](https://www.django-
-rest-framework.org/) serializer serializer for automatic form generation on the
-front when working through rest api. (An npm package on [vuejs](https://
-vuejs.org/) will also be developed generating form based on response from api).
-* [ ] Authorization backend for authorization by a pair of email and password.
-* [ ] Functionality for working with images. * [x] Image editor like
-easy_thumbnails. * [x] A field for the drf serializer that returns a set of
-images (for example, a standard image and a double-sized image for a retina
-screen), as well as in different formats (for example, in the original format
-and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs * [ ]
-Functionality similar to that described in the previous paragraph only for
+Package with various functional (such as mixins, form utils, upload handlers
+and other) for Django Framework. This library is a set of various functionality
+that I use from project to project. The main task of this package is to clean
+up this functionality, test it, and also organize the documentation so that
+colleagues can understand how and what works. However, if someone decides to
+use this functionality in their project, and even more so to add functionality
+or change the implementation to a more correct, beautiful or understandable
+one, I will only be happy, do not worry and feel free to write to me by [mail]
+(mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/
+issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github]
+(https://github.com/dd/Meringue). Read more in the [documentation](https://
+dd.github.io/Meringue/). ## Roadmap Adding new functionality. Can change. * [ ]
+[drf](https://www.django-rest-framework.org/) serializer serializer for
+automatic form generation on the front when working through rest api. (An npm
+package on [vuejs](https://vuejs.org/) will also be developed generating form
+based on response from api). * [ ] Authorization backend for authorization by a
+pair of email and password. * [ ] Functionality for working with images. * [x]
+Image editor like easy_thumbnails. * [x] A field for the drf serializer that
+returns a set of images (for example, a standard image and a double-sized image
+for a retina screen), as well as in different formats (for example, in the
+original format and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs *
+[ ] Functionality similar to that described in the previous paragraph only for
 video. * [ ] Functionality for loading private files available through [nginx
 internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal). ##
 Contributing - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-
 flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/
 gitflow-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https:/
 /github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
 github.com/psf/black) - [x] Lint commit with [Gitlint](https://
```

