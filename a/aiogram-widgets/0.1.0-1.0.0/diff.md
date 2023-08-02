# Comparing `tmp/aiogram_widgets-0.1.0.tar.gz` & `tmp/aiogram_widgets-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_widgets-0.1.0.tar", max compression
+gzip compressed data, was "aiogram_widgets-1.0.0.tar", max compression
```

## Comparing `aiogram_widgets-0.1.0.tar` & `aiogram_widgets-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      115 2023-08-02 12:13:04.887957 aiogram_widgets-0.1.0/aiogram_widgets/enums.py
--rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-0.1.0/aiogram_widgets/pagination/__init__.py
--rw-r--r--   0        0        0     4167 2023-08-02 12:07:56.163687 aiogram_widgets-0.1.0/aiogram_widgets/pagination/_base.py
--rw-r--r--   0        0        0     3092 2023-08-02 14:21:23.483546 aiogram_widgets-0.1.0/aiogram_widgets/pagination/keyboard.py
--rw-r--r--   0        0        0     3256 2023-08-02 14:21:32.775046 aiogram_widgets-0.1.0/aiogram_widgets/pagination/text.py
--rw-r--r--   0        0        0      547 2023-08-02 12:13:20.064283 aiogram_widgets-0.1.0/aiogram_widgets/types.py
--rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-0.1.0/LICENSE
--rw-r--r--   0        0        0      649 2023-08-02 14:43:46.312398 aiogram_widgets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4337 2023-08-02 14:29:45.816378 aiogram_widgets-0.1.0/README.md
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 aiogram_widgets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      115 2023-08-02 12:13:04.887957 aiogram_widgets-1.0.0/aiogram_widgets/enums.py
+-rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.0.0/aiogram_widgets/pagination/__init__.py
+-rw-r--r--   0        0        0     4161 2023-08-02 14:50:17.801041 aiogram_widgets-1.0.0/aiogram_widgets/pagination/_base.py
+-rw-r--r--   0        0        0     3092 2023-08-02 14:21:23.483546 aiogram_widgets-1.0.0/aiogram_widgets/pagination/keyboard.py
+-rw-r--r--   0        0        0     3256 2023-08-02 14:21:32.775046 aiogram_widgets-1.0.0/aiogram_widgets/pagination/text.py
+-rw-r--r--   0        0        0      547 2023-08-02 12:13:20.064283 aiogram_widgets-1.0.0/aiogram_widgets/types.py
+-rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.0.0/LICENSE
+-rw-r--r--   0        0        0      649 2023-08-02 14:50:39.357524 aiogram_widgets-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4337 2023-08-02 14:29:45.816378 aiogram_widgets-1.0.0/README.md
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 aiogram_widgets-1.0.0/PKG-INFO
```

### Comparing `aiogram_widgets-0.1.0/aiogram_widgets/pagination/_base.py` & `aiogram_widgets-1.0.0/aiogram_widgets/pagination/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from math import ceil
 from typing import Any, Dict, List
 
 from aiogram import Dispatcher, Router
 from aiogram.types import InlineKeyboardButton, InlineKeyboardMarkup
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 
-from aiogram_widgets.types.types import Additional_buttons_type
+from aiogram_widgets.types import Additional_buttons_type
 
 
 class BasePaginator(ABC):
     def __init__(
         self,
         data: List[Any],
         per_page: int,
```

### Comparing `aiogram_widgets-0.1.0/aiogram_widgets/pagination/keyboard.py` & `aiogram_widgets-1.0.0/aiogram_widgets/pagination/keyboard.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-0.1.0/aiogram_widgets/pagination/text.py` & `aiogram_widgets-1.0.0/aiogram_widgets/pagination/text.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-0.1.0/aiogram_widgets/types.py` & `aiogram_widgets-1.0.0/aiogram_widgets/types.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-0.1.0/LICENSE` & `aiogram_widgets-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-0.1.0/pyproject.toml` & `aiogram_widgets-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiogram-widgets"
-version = "0.1.0"
+version = "1.0.0"
 description = ""
 authors = ["ggindinson"]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `aiogram_widgets-0.1.0/README.md` & `aiogram_widgets-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-0.1.0/PKG-INFO` & `aiogram_widgets-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-widgets
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
 Author: ggindinson
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

