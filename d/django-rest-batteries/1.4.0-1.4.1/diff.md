# Comparing `tmp/django_rest_batteries-1.4.0.tar.gz` & `tmp/django_rest_batteries-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rest_batteries-1.4.0.tar", max compression
+gzip compressed data, was "django_rest_batteries-1.4.1.tar", max compression
```

## Comparing `django_rest_batteries-1.4.0.tar` & `django_rest_batteries-1.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/LICENSE
--rw-r--r--   0        0        0     4169 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/README.md
--rw-r--r--   0        0        0     1271 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/__init__.py
--rw-r--r--   0        0        0     4628 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/errors_formatter.py
--rw-r--r--   0        0        0      397 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/exception_handlers.py
--rw-r--r--   0        0        0     6572 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/generics.py
--rw-r--r--   0        0        0     4479 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/mixins.py
--rw-r--r--   0        0        0      168 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/views.py
--rw-r--r--   0        0        0     3926 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/viewsets.py
--rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 django_rest_batteries-1.4.0/setup.py
--rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 django_rest_batteries-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/LICENSE
+-rw-r--r--   0        0        0     4169 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/README.md
+-rw-r--r--   0        0        0     1510 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/__init__.py
+-rw-r--r--   0        0        0     4544 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/errors_formatter.py
+-rw-r--r--   0        0        0      397 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/exception_handlers.py
+-rw-r--r--   0        0        0     6574 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/generics.py
+-rw-r--r--   0        0        0     4479 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/mixins.py
+-rw-r--r--   0        0        0      168 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/views.py
+-rw-r--r--   0        0        0     3956 2023-08-02 11:53:46.370035 django_rest_batteries-1.4.1/rest_batteries/viewsets.py
+-rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 django_rest_batteries-1.4.1/setup.py
+-rw-r--r--   0        0        0     5004 1970-01-01 00:00:00.000000 django_rest_batteries-1.4.1/PKG-INFO
```

### Comparing `django_rest_batteries-1.4.0/LICENSE` & `django_rest_batteries-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rest_batteries-1.4.0/README.md` & `django_rest_batteries-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_rest_batteries-1.4.0/pyproject.toml` & `django_rest_batteries-1.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-rest-batteries"
-version = "1.4.0"
+version = "1.4.1"
 description = "Build clean APIs with DRF faster"
 authors = ["Define Impossible <hi@defineimpossible.io>"]
 packages = [
     { include = "rest_batteries" }
 ]
 license = "MIT"
 readme = "README.md"
@@ -15,46 +15,62 @@
     "drf",
     "django",
     "batteries",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-django = "^3.2"
-djangorestframework = "^3.12.2"
+django = ">=3.2"
+djangorestframework = ">=3.12.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+django-debug-toolbar = "^4.1.0"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-django = "^4.5.2"
-django-debug-toolbar = "^4.1.0"
 factory-boy = "^3.2.1"
-isort = "^5.2.2"
-black = "^23.3.0"
+
+[tool.poetry.group.code-quality.dependencies]
+black = "^23.7.0"
+ruff = "^0.0.277"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
-line-length = 88
+line-length = 99
 skip-string-normalization = true
 
-[tool.isort]
-skip = [
+[tool.ruff]
+select = ["E", "F", "I"]
+
+exclude = [
+    ".bzr",
     ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
     ".tox",
     ".venv",
-    "migrations",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "migrations"
 ]
-
-# Vertical hanging indent:
-multi_line_output = 3
-include_trailing_comma = true
-
-line_length = 88
-known_third_party = "rest_batteries"
+line-length = 99
 
 [tool.pytest.ini_options]
 # Django configuration:
 # https://pytest-django.readthedocs.io/en/latest/
 DJANGO_SETTINGS_MODULE = "tests.settings"
```

### Comparing `django_rest_batteries-1.4.0/rest_batteries/errors_formatter.py` & `django_rest_batteries-1.4.1/rest_batteries/errors_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,15 @@
         """
         if errors_dict is None:
             return []
 
         message_value = errors_dict.get(self.MESSAGE, None)
 
         # Note: If 'message' is name of a field we don't want to stop the recursion here!
-        if message_value is not None and (
-            type(message_value) in {str, exceptions.ErrorDetail}
-        ):
+        if message_value is not None and (type(message_value) in {str, exceptions.ErrorDetail}):
             if field_path:
                 errors_dict[self.FIELD] = field_path
             return [errors_dict]
 
         errors_list = []
         for key, value in errors_dict.items():
             new_field_path = (
@@ -122,17 +120,15 @@
                     if self.MESSAGE in field_error:
                         if not key_is_non_field_errors:
                             field_error[self.FIELD] = new_field_path
                         current_level_error_list.append(field_error)
                     else:
                         path = '{0}[{1}]'.format(new_field_path, index)
                         current_level_error_list.extend(
-                            self._get_list_of_errors(
-                                field_path=path, errors_dict=field_error
-                            )
+                            self._get_list_of_errors(field_path=path, errors_dict=field_error)
                         )
             else:
                 path = field_path if key_is_non_field_errors else new_field_path
 
                 current_level_error_list = self._get_list_of_errors(
                     field_path=path, errors_dict=value
                 )
```

### Comparing `django_rest_batteries-1.4.0/rest_batteries/generics.py` & `django_rest_batteries-1.4.1/rest_batteries/generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 
     def get_request_serializer(self, *args, **kwargs) -> BaseSerializer:
         serializer = self.get_request_serializer_or_none(*args, **kwargs)
         if serializer is None:
             self.raise_request_serializer_error()
         return serializer
 
-    def get_request_serializer_or_none(
-        self, *args, **kwargs
-    ) -> Optional[BaseSerializer]:
+    def get_request_serializer_or_none(self, *args, **kwargs) -> Optional[BaseSerializer]:
         serializer_class = self.get_request_serializer_class_or_none()
         if serializer_class is not None:
             kwargs.setdefault('context', self.get_request_serializer_context())
             return serializer_class(*args, **kwargs)
 
     def get_request_serializer_class_or_none(self) -> Optional[Type[BaseSerializer]]:
         if self.request.method == 'DELETE':
@@ -39,40 +37,40 @@
         return self.request_serializer_class
 
     def get_request_serializer_context(self):
         return self.get_serializer_context()
 
     def raise_request_serializer_error(self):
         raise ImproperlyConfigured(
-            f'{self.__class__.__name__} should properly configure `request_serializer_class` attribute'
+            f'{self.__class__.__name__} should properly configure '
+            '`request_serializer_class` attribute'
         )
 
     def get_response_serializer(self, *args, **kwargs) -> BaseSerializer:
         serializer = self.get_response_serializer_or_none(*args, **kwargs)
         if serializer is None:
             self.raise_response_serializer_error()
         return serializer
 
-    def get_response_serializer_or_none(
-        self, *args, **kwargs
-    ) -> Optional[BaseSerializer]:
+    def get_response_serializer_or_none(self, *args, **kwargs) -> Optional[BaseSerializer]:
         serializer_class = self.get_response_serializer_class_or_none()
         if serializer_class is not None:
             kwargs.setdefault('context', self.get_response_serializer_context())
             return serializer_class(*args, **kwargs)
 
     def get_response_serializer_class_or_none(self) -> Optional[Type[BaseSerializer]]:
         return self.response_serializer_class
 
     def get_response_serializer_context(self):
         return self.get_serializer_context()
 
     def raise_response_serializer_error(self):
         raise ImproperlyConfigured(
-            f'{self.__class__.__name__} should properly configure `response_serializer_class` attribute'
+            f'{self.__class__.__name__} should properly configure '
+            '`response_serializer_class` attribute'
         )
 
     def get_serializer_class(self) -> Type[BaseSerializer]:
         response_serializer_class = self.get_response_serializer_class_or_none()
         if response_serializer_class is not None:
             return response_serializer_class
```

### Comparing `django_rest_batteries-1.4.0/rest_batteries/mixins.py` & `django_rest_batteries-1.4.1/rest_batteries/mixins.py`

 * *Files identical despite different names*

### Comparing `django_rest_batteries-1.4.0/rest_batteries/viewsets.py` & `django_rest_batteries-1.4.1/rest_batteries/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         if serializer_class is None:
             return super().get_request_serializer_class_or_none()
 
         return serializer_class
 
     def raise_request_serializer_error(self):
         raise ImproperlyConfigured(
-            f'{self.__class__.__name__} should properly configure `request_action_serializer_classes` attribute'
+            f'{self.__class__.__name__} should properly configure '
+            '`request_action_serializer_classes` attribute'
         )
 
     def get_response_serializer_class_or_none(self) -> Optional[Type[BaseSerializer]]:
         serializer_class = None
 
         if self.response_action_serializer_classes:
             serializer_class = self.response_action_serializer_classes.get(self.action)
@@ -71,15 +72,16 @@
         if serializer_class is None:
             return super().get_response_serializer_class_or_none()
 
         return serializer_class
 
     def raise_response_serializer_error(self):
         raise ImproperlyConfigured(
-            f'{self.__class__.__name__} should properly configure `response_action_serializer_classes` attribute'
+            f'{self.__class__.__name__} should properly configure '
+            '`response_action_serializer_classes` attribute'
         )
 
     def raise_serializer_error(self):
         raise ImproperlyConfigured(
             f'{self.__class__.__name__} should properly configure one of these attributes: '
             f'`response_action_serializer_classes`, `serializer_class`'
         )
```

### Comparing `django_rest_batteries-1.4.0/setup.py` & `django_rest_batteries-1.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['rest_batteries']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['django>=3.2,<4.0', 'djangorestframework>=3.12.2,<4.0.0']
+['django>=3.2', 'djangorestframework>=3.12.2']
 
 setup_kwargs = {
     'name': 'django-rest-batteries',
-    'version': '1.4.0',
+    'version': '1.4.1',
     'description': 'Build clean APIs with DRF faster',
     'long_description': '[![Test](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml/badge.svg)](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml)\n[![Coverage](https://codecov.io/gh/defineimpossible/django-rest-batteries/branch/master/graph/badge.svg)](https://codecov.io/gh/defineimpossible/django-rest-batteries)\n\n# Django REST Framework Batteries\n\nBuild clean APIs with DRF faster.\n\n# Overview\n\nHere\'s a quick overview of what the library has at the moment:\n\n- Action-based serializers for ViewSets\n- Two serializers per request/response cycle for ViewSets and GenericAPIViews\n- Action-based permissions for ViewSets\n- Single format for all errors\n\n# Requirements\n\n- Python ≥ 3.8\n- Django ≥ 3.2\n- Django REST Framework ≥ 3.12\n\n# Installation\n\n```bash\n$ pip install django-rest-batteries\n```\n\n# Usage\n\n## Action-based serializers for ViewSets\n\nEach action can have a separate serializer:\n\n```python\nfrom rest_batteries.mixins import RetrieveModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\n...\n\nclass OrderViewSet(RetrieveModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    response_action_serializer_classes = {\n        \'retrieve\': OrderSerializer,\n        \'list\': OrderListSerializer,\n    }\n```\n\n## Two serializers per request/response cycle\n\nWe found that more often than not we need a separate serializer for handling request payload and a separate serializer for generating response data.\n\nHow to achieve it in ViewSet:\n\n```python\nfrom rest_batteries.mixins import CreateModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\n...\n\nclass OrderViewSet(CreateModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    request_action_serializer_classes = {\n        \'create\': OrderCreateSerializer,\n    }\n    response_action_serializer_classes = {\n        \'create\': OrderResponseSerializer,\n        \'list\': OrderResponseSerializer,\n        \'cancel\': OrderResponseSerializer,\n    }\n```\n\nHow to achieve it in GenericAPIView:\n\n```python\nfrom rest_batteries.generics import CreateAPIView\n...\n\n\nclass OrderCreateView(CreateAPIView):\n    request_serializer_class = OrderCreateSerializer\n    response_serializer_class = OrderResponseSerializer\n```\n\n## Action-based permissions for ViewSets\n\nEach action can have a separate set of permissions:\n\n```python\nfrom rest_batteries.mixins import CreateModelMixin, UpdateModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\nfrom rest_framework.permissions import AllowAny, IsAuthenticated\n...\n\nclass OrderViewSet(CreateModelMixin,\n                   UpdateModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    action_permission_classes = {\n        \'create\': IsAuthenticated,\n        \'update\': [IsAuthenticated, IsOrderOwner],\n        \'list\': AllowAny,\n    }\n```\n\n## Single format for all errors\n\nWe believe that having a single format for all errors is good practice. This will make the process of displaying and handling errors much simpler for clients that use your APIs.\n\nAny error always will be a JSON object with a message, code (identifier of the error), and field if the error is specific to a particular field. How your response could look like:\n\n```python\n{\n    "errors": [\n        {\n            "message": "Delete or cancel all reservations first.",\n            "code": "invalid"\n        },\n        {\n            "message": "Ensure this field has no more than 21 characters.",\n            "code": "max_length",\n            "field": "address.work_phone"\n        },\n        {\n            "message": "This email already exists",\n            "code": "unique",\n            "field": "login_email"\n        }\n    ]\n}\n```\n\nYou will not have a single format out-of-the-box after installation. You need to add an exception handler to your DRF settings:\n\n```python\nREST_FRAMEWORK = {\n    ...\n    \'EXCEPTION_HANDLER\': \'rest_batteries.exception_handlers.errors_formatter_exception_handler\',\n}\n```\n\n# Credits\n\n- [Django-Styleguide by HackSoftware](https://github.com/HackSoftware/Django-Styleguide) - inspiration\n',
     'author': 'Define Impossible',
     'author_email': 'hi@defineimpossible.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/defineimpossible/django-rest-batteries',
```

### Comparing `django_rest_batteries-1.4.0/PKG-INFO` & `django_rest_batteries-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-rest-batteries
-Version: 1.4.0
+Version: 1.4.1
 Summary: Build clean APIs with DRF faster
 Home-page: https://github.com/defineimpossible/django-rest-batteries
 License: MIT
 Keywords: django rest framework,drf,django,batteries
 Author: Define Impossible
 Author-email: hi@defineimpossible.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.2,<4.0)
-Requires-Dist: djangorestframework (>=3.12.2,<4.0.0)
+Requires-Dist: django (>=3.2)
+Requires-Dist: djangorestframework (>=3.12.2)
 Project-URL: Repository, https://github.com/defineimpossible/django-rest-batteries
 Description-Content-Type: text/markdown
 
 [![Test](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml/badge.svg)](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml)
 [![Coverage](https://codecov.io/gh/defineimpossible/django-rest-batteries/branch/master/graph/badge.svg)](https://codecov.io/gh/defineimpossible/django-rest-batteries)
 
 # Django REST Framework Batteries
```

