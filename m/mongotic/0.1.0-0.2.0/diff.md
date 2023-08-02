# Comparing `tmp/mongotic-0.1.0.tar.gz` & `tmp/mongotic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongotic-0.1.0.tar", max compression
+gzip compressed data, was "mongotic-0.2.0.tar", max compression
```

## Comparing `mongotic-0.1.0.tar` & `mongotic-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-07-31 13:17:50.466286 mongotic-0.1.0/LICENSE
--rw-r--r--   0        0        0     3569 2023-08-01 16:53:40.712419 mongotic-0.1.0/README.md
--rw-r--r--   0        0        0      638 2023-07-31 13:17:50.466572 mongotic-0.1.0/mongotic/__init__.py
--rw-r--r--   0        0        0       36 2023-07-31 13:17:50.466647 mongotic-0.1.0/mongotic/exceptions.py
--rw-r--r--   0        0        0     3665 2023-07-31 13:17:50.466769 mongotic-0.1.0/mongotic/model.py
--rw-r--r--   0        0        0     8018 2023-08-01 15:53:45.661274 mongotic-0.1.0/mongotic/orm.py
--rw-r--r--   0        0        0       18 2023-07-31 13:17:50.466979 mongotic-0.1.0/mongotic/version.py
--rw-r--r--   0        0        0      781 2023-08-01 16:49:17.922789 mongotic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 mongotic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-31 13:17:50.466286 mongotic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3569 2023-08-01 16:53:40.712419 mongotic-0.2.0/README.md
+-rw-r--r--   0        0        0      638 2023-07-31 13:17:50.466572 mongotic-0.2.0/mongotic/__init__.py
+-rw-r--r--   0        0        0       36 2023-07-31 13:17:50.466647 mongotic-0.2.0/mongotic/exceptions.py
+-rw-r--r--   0        0        0     5338 2023-08-02 14:43:56.148820 mongotic-0.2.0/mongotic/model.py
+-rw-r--r--   0        0        0     8282 2023-08-02 14:43:56.149111 mongotic-0.2.0/mongotic/orm.py
+-rw-r--r--   0        0        0       18 2023-07-31 13:17:50.466979 mongotic-0.2.0/mongotic/version.py
+-rw-r--r--   0        0        0      781 2023-08-02 14:44:08.064759 mongotic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 mongotic-0.2.0/PKG-INFO
```

### Comparing `mongotic-0.1.0/LICENSE` & `mongotic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongotic-0.1.0/README.md` & `mongotic-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mongotic-0.1.0/mongotic/__init__.py` & `mongotic-0.2.0/mongotic/__init__.py`

 * *Files identical despite different names*

### Comparing `mongotic-0.1.0/mongotic/orm.py` & `mongotic-0.2.0/mongotic/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,25 @@
     def filter_by(self, **kwargs: Any) -> "QuerySet":
         for k, v in kwargs.items():
             self._filters.append(
                 ModelField(field_name=k, model_class=self.orm_model) == v
             )
         return self
 
-    def limit(self, *args: Any, **kwargs: Any) -> "QuerySet":
-        ...
+    def limit(self, value: int, *args: Any, **kwargs: Any) -> "QuerySet":
+        if value < 0:
+            raise ValueError("Limit value must be positive")
+        self._limit = value
+        return self
 
-    def offset(self, *args: Any, **kwargs: Any) -> "QuerySet":
-        ...
+    def offset(self, value: int, *args: Any, **kwargs: Any) -> "QuerySet":
+        if value < 0:
+            raise ValueError("Offset value must be positive")
+        self._offset = value
+        return self
 
     def first(self, *args: Any, **kwargs: Any) -> "MongoBaseModel":
         collection = self.engine[self._db_name][self._col_name]
 
         filter_body = ModelFieldOperation.to_mongo_filter(filters=self._filters)
         doc_raw = collection.find_one(filter=filter_body)
         if not doc_raw:
```

### Comparing `mongotic-0.1.0/pyproject.toml` & `mongotic-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongotic"
-version = "0.1.0"
+version = "0.2.0"
 description = "The concept of MongoDB, SQLAlchemy and Pydantic."
 authors = ["Allen Chou <f1470891079@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["mongodb", "sqlalchemy", "pydantic"]
 homepage = "https://github.com/dockhardman/mongotic"
 repository = "https://github.com/dockhardman/mongotic"
```

### Comparing `mongotic-0.1.0/PKG-INFO` & `mongotic-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongotic
-Version: 0.1.0
+Version: 0.2.0
 Summary: The concept of MongoDB, SQLAlchemy and Pydantic.
 Home-page: https://github.com/dockhardman/mongotic
 License: MIT
 Keywords: mongodb,sqlalchemy,pydantic
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
```

