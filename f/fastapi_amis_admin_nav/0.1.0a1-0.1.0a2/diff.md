# Comparing `tmp/fastapi_amis_admin_nav-0.1.0a1.tar.gz` & `tmp/fastapi_amis_admin_nav-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_nav-0.1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_amis_admin_nav-0.1.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin_nav-0.1.0a1.tar` & `fastapi_amis_admin_nav-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.1.0a1/README.md
--rw-r--r--   0        0        0      382 2023-07-17 10:51:32.245636 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/__init__.py
--rw-r--r--   0        0        0     5445 2023-07-17 03:22:25.604890 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/admin.py
--rw-r--r--   0        0        0     5694 2023-07-17 03:36:39.135513 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/models.py
--rw-r--r--   0        0        0     8701 2023-07-17 02:27:22.952772 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/utils.py
--rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.1.0a2/README.md
+-rw-r--r--   0        0        0      382 2023-08-02 08:03:30.616271 fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/__init__.py
+-rw-r--r--   0        0        0     5445 2023-07-17 03:22:25.604890 fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/admin.py
+-rw-r--r--   0        0        0     5671 2023-08-02 08:00:41.511013 fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/models.py
+-rw-r--r--   0        0        0     8701 2023-07-17 02:27:22.952772 fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/utils.py
+-rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.1.0a2/PKG-INFO
```

### Comparing `fastapi_amis_admin_nav-0.1.0a1/README.md` & `fastapi_amis_admin_nav-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/admin.py` & `fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/admin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/models.py` & `fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         amis_form_item={  # 非自定义页面, 都是只读
             "disabledOn": "!this.is_custom",
         },
     )
     label: str = Field(..., title="页面名称", max_length=20)
     icon: str = Field(
         default="fa fa-flash",
-        max_length=50,
         title="页面图标",
         description="参考: https://fontawesome.com/",
         amis_form_item=amis.Group(
             name="icon",
             body=[
                 amis.InputText(
                     name="icon",
```

### Comparing `fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/utils.py` & `fastapi_amis_admin_nav-0.1.0a2/fastapi_amis_admin_nav/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.1.0a1/pyproject.toml` & `fastapi_amis_admin_nav-0.1.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.1.0a1/PKG-INFO` & `fastapi_amis_admin_nav-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_nav
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: FastAPI-Amis-Admin-Nav是一个基于FastAPI-Amis-Admin并且为FastAPI-Amis-Admin提供可视化导航页面管理的拓展库.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-amis-admin-nav
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

