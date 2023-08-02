# Comparing `tmp/aiogram_widgets-1.0.0.tar.gz` & `tmp/aiogram_widgets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_widgets-1.0.0.tar", max compression
+gzip compressed data, was "aiogram_widgets-1.0.1.tar", max compression
```

## Comparing `aiogram_widgets-1.0.0.tar` & `aiogram_widgets-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      115 2023-08-02 12:13:04.887957 aiogram_widgets-1.0.0/aiogram_widgets/enums.py
--rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.0.0/aiogram_widgets/pagination/__init__.py
--rw-r--r--   0        0        0     4161 2023-08-02 14:50:17.801041 aiogram_widgets-1.0.0/aiogram_widgets/pagination/_base.py
--rw-r--r--   0        0        0     3092 2023-08-02 14:21:23.483546 aiogram_widgets-1.0.0/aiogram_widgets/pagination/keyboard.py
--rw-r--r--   0        0        0     3256 2023-08-02 14:21:32.775046 aiogram_widgets-1.0.0/aiogram_widgets/pagination/text.py
--rw-r--r--   0        0        0      547 2023-08-02 12:13:20.064283 aiogram_widgets-1.0.0/aiogram_widgets/types.py
--rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.0.0/LICENSE
--rw-r--r--   0        0        0      649 2023-08-02 14:50:39.357524 aiogram_widgets-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4337 2023-08-02 14:29:45.816378 aiogram_widgets-1.0.0/README.md
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 aiogram_widgets-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      115 2023-08-02 12:13:04.887957 aiogram_widgets-1.0.1/aiogram_widgets/enums.py
+-rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.0.1/aiogram_widgets/pagination/__init__.py
+-rw-r--r--   0        0        0     4161 2023-08-02 14:50:17.801041 aiogram_widgets-1.0.1/aiogram_widgets/pagination/_base.py
+-rw-r--r--   0        0        0     3091 2023-08-02 15:03:15.234777 aiogram_widgets-1.0.1/aiogram_widgets/pagination/keyboard.py
+-rw-r--r--   0        0        0     3255 2023-08-02 15:03:21.200356 aiogram_widgets-1.0.1/aiogram_widgets/pagination/text.py
+-rw-r--r--   0        0        0      547 2023-08-02 12:13:20.064283 aiogram_widgets-1.0.1/aiogram_widgets/types.py
+-rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.0.1/LICENSE
+-rw-r--r--   0        0        0      622 2023-08-02 15:03:53.057697 aiogram_widgets-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4337 2023-08-02 14:29:45.816378 aiogram_widgets-1.0.1/README.md
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 aiogram_widgets-1.0.1/PKG-INFO
```

### Comparing `aiogram_widgets-1.0.0/aiogram_widgets/pagination/_base.py` & `aiogram_widgets-1.0.1/aiogram_widgets/pagination/_base.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.0.0/aiogram_widgets/pagination/keyboard.py` & `aiogram_widgets-1.0.1/aiogram_widgets/pagination/keyboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class KeyboardPaginator(BasePaginator):
     """Allows to create a new markup with keyboard pagination"""
 
     @validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
-        data: Annotated[List[Button_type], Field(min_length=1)],
+        data: Annotated[List[Button_type], Field(min_items=1)],
         router: Dispatcher | Router,
         additional_buttons: Additional_buttons_type | None = None,
         pagination_key: Pagination_key = "keyboard_paginated",
         per_row: Per_row_type = 2,
         per_page: Per_page_type = 10,
     ):
         """
```

### Comparing `aiogram_widgets-1.0.0/aiogram_widgets/pagination/text.py` & `aiogram_widgets-1.0.1/aiogram_widgets/pagination/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class TextPaginator(BasePaginator):
     """Allows to create a new markup with text pagination"""
 
     @validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
-        data: Annotated[List[str], Field(min_length=1)],
+        data: Annotated[List[str], Field(min_items=1)],
         router: Dispatcher | Router,
         data_joiner: str = "\n",
         additional_buttons: Additional_buttons_type | None = None,
         pagination_key: Pagination_key = "text_paginated",
         per_page: PositiveInt = 10,
     ):
         """
```

### Comparing `aiogram_widgets-1.0.0/aiogram_widgets/types.py` & `aiogram_widgets-1.0.1/aiogram_widgets/types.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.0.0/LICENSE` & `aiogram_widgets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.0.0/README.md` & `aiogram_widgets-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.0.0/PKG-INFO` & `aiogram_widgets-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-widgets
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: ggindinson
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

