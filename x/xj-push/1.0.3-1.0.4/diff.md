# Comparing `tmp/xj_push-1.0.3.tar.gz` & `tmp/xj_push-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_push-1.0.3.tar", last modified: Wed Aug  2 07:40:51 2023, max compression
+gzip compressed data, was "dist\xj_push-1.0.4.tar", last modified: Wed Aug  2 08:22:49 2023, max compression
```

## Comparing `xj_push-1.0.3.tar` & `xj_push-1.0.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/
--rw-rw-rw-   0        0        0     1084 2023-08-02 07:40:51.000000 xj_push-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      943 2023-07-14 07:14:50.000000 xj_push-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 07:40:51.000000 xj_push-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1902 2023-08-02 07:40:45.000000 xj_push-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push/
--rw-rw-rw-   0        0        0      230 2023-07-19 09:07:24.000000 xj_push-1.0.3/xj_push/__init__.py
--rw-rw-rw-   0        0        0     1945 2023-07-20 02:59:59.000000 xj_push-1.0.3/xj_push/admin.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push/apis/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/apis/__init__.py
--rw-rw-rw-   0        0        0      892 2023-07-20 08:43:52.000000 xj_push-1.0.3/xj_push/apis/push_apis.py
--rw-rw-rw-   0        0        0     1972 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/apis/push_plan_apis.py
--rw-rw-rw-   0        0        0     1951 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/apis/push_push_apis.py
--rw-rw-rw-   0        0        0     1984 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/apis/push_record_apis.py
--rw-rw-rw-   0        0        0     1996 2023-07-20 02:44:18.000000 xj_push-1.0.3/xj_push/apis/push_template_apis.py
--rw-rw-rw-   0        0        0      184 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/apps.py
--rw-rw-rw-   0        0        0     1661 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/common.py
--rw-rw-rw-   0        0        0     4138 2023-07-20 02:44:18.000000 xj_push-1.0.3/xj_push/models.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push/push_pipeline/
--rw-rw-rw-   0        0        0      149 2023-07-20 03:05:22.000000 xj_push-1.0.3/xj_push/push_pipeline/__init__.py
--rw-rw-rw-   0        0        0     4357 2023-08-02 05:55:38.000000 xj_push-1.0.3/xj_push/push_pipeline/bx_custom_pipeline.py
--rw-rw-rw-   0        0        0     2035 2023-07-22 06:48:09.000000 xj_push-1.0.3/xj_push/push_pipeline/bx_visitor_pipeline.py
--rw-rw-rw-   0        0        0     4390 2023-08-02 07:37:27.000000 xj_push-1.0.3/xj_push/push_pipeline/bx_worker_pipeline.py
--rw-rw-rw-   0        0        0     7058 2023-08-01 06:37:27.000000 xj_push-1.0.3/xj_push/push_pipeline/pipline_base.py
--rw-rw-rw-   0        0        0     1212 2023-07-21 07:03:35.000000 xj_push-1.0.3/xj_push/service_register.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push/services/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/services/__init__.py
--rw-rw-rw-   0        0        0     6046 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/services/push_plan_service.py
--rw-rw-rw-   0        0        0     5969 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/services/push_record_service.py
--rw-rw-rw-   0        0        0     6943 2023-07-16 14:35:03.000000 xj_push-1.0.3/xj_push/services/push_service.py
--rw-rw-rw-   0        0        0     4461 2023-08-02 07:33:02.000000 xj_push-1.0.3/xj_push/services/push_template_main_service.py
--rw-rw-rw-   0        0        0     6183 2023-07-20 08:45:42.000000 xj_push-1.0.3/xj_push/services/push_template_service.py
--rw-rw-rw-   0        0        0      260 2023-07-19 09:08:13.000000 xj_push-1.0.3/xj_push/urls.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push/utils/
--rw-rw-rw-   0        0        0        0 2023-07-16 14:35:03.000000 xj_push-1.0.3/xj_push/utils/__init__.py
--rw-rw-rw-   0        0        0     1661 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/utils/common.py
--rw-rw-rw-   0        0        0     4628 2023-07-11 05:41:09.000000 xj_push-1.0.3/xj_push/utils/custom_response.py
--rw-rw-rw-   0        0        0    37715 2023-07-05 03:23:16.000000 xj_push-1.0.3/xj_push/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_push-1.0.3/xj_push/utils/j_dict.py
--rw-rw-rw-   0        0        0     7311 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/utils/model_handle.py
--rw-rw-rw-   0        0        0     5145 2023-06-02 09:15:38.000000 xj_push-1.0.3/xj_push/utils/service_manager.py
--rw-rw-rw-   0        0        0     5668 2023-07-05 05:42:50.000000 xj_push-1.0.3/xj_push/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     7924 2023-07-21 06:22:34.000000 xj_push-1.0.3/xj_push/utils/utility_method.py
--rw-rw-rw-   0        0        0     2460 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/utils/utils.py
--rw-rw-rw-   0        0        0     3385 2023-07-14 07:14:50.000000 xj_push-1.0.3/xj_push/utils/wechat.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push.egg-info/
--rw-rw-rw-   0        0        0     1084 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 07:40:51.000000 xj_push-1.0.3/xj_push.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-08-02 08:22:49.000000 xj_push-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-07-14 07:14:50.000000 xj_push-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:22:49.000000 xj_push-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1902 2023-08-02 08:22:42.000000 xj_push-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push/
+-rw-rw-rw-   0        0        0      230 2023-07-19 09:07:24.000000 xj_push-1.0.4/xj_push/__init__.py
+-rw-rw-rw-   0        0        0     1945 2023-07-20 02:59:59.000000 xj_push-1.0.4/xj_push/admin.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/apis/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-07-20 08:43:52.000000 xj_push-1.0.4/xj_push/apis/push_apis.py
+-rw-rw-rw-   0        0        0     1972 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/apis/push_plan_apis.py
+-rw-rw-rw-   0        0        0     1951 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/apis/push_push_apis.py
+-rw-rw-rw-   0        0        0     1984 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/apis/push_record_apis.py
+-rw-rw-rw-   0        0        0     1996 2023-07-20 02:44:18.000000 xj_push-1.0.4/xj_push/apis/push_template_apis.py
+-rw-rw-rw-   0        0        0      184 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/apps.py
+-rw-rw-rw-   0        0        0     1661 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/common.py
+-rw-rw-rw-   0        0        0     4138 2023-07-20 02:44:18.000000 xj_push-1.0.4/xj_push/models.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push/push_pipeline/
+-rw-rw-rw-   0        0        0      149 2023-07-20 03:05:22.000000 xj_push-1.0.4/xj_push/push_pipeline/__init__.py
+-rw-rw-rw-   0        0        0     4357 2023-08-02 05:55:38.000000 xj_push-1.0.4/xj_push/push_pipeline/bx_custom_pipeline.py
+-rw-rw-rw-   0        0        0     2035 2023-07-22 06:48:09.000000 xj_push-1.0.4/xj_push/push_pipeline/bx_visitor_pipeline.py
+-rw-rw-rw-   0        0        0     4324 2023-08-02 08:21:41.000000 xj_push-1.0.4/xj_push/push_pipeline/bx_worker_pipeline.py
+-rw-rw-rw-   0        0        0     7058 2023-08-01 06:37:27.000000 xj_push-1.0.4/xj_push/push_pipeline/pipline_base.py
+-rw-rw-rw-   0        0        0     1212 2023-07-21 07:03:35.000000 xj_push-1.0.4/xj_push/service_register.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push/services/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/services/__init__.py
+-rw-rw-rw-   0        0        0     6046 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/services/push_plan_service.py
+-rw-rw-rw-   0        0        0     5969 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/services/push_record_service.py
+-rw-rw-rw-   0        0        0     6943 2023-07-16 14:35:03.000000 xj_push-1.0.4/xj_push/services/push_service.py
+-rw-rw-rw-   0        0        0     4548 2023-08-02 08:21:06.000000 xj_push-1.0.4/xj_push/services/push_template_main_service.py
+-rw-rw-rw-   0        0        0     6183 2023-07-20 08:45:42.000000 xj_push-1.0.4/xj_push/services/push_template_service.py
+-rw-rw-rw-   0        0        0      260 2023-07-19 09:08:13.000000 xj_push-1.0.4/xj_push/urls.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-16 14:35:03.000000 xj_push-1.0.4/xj_push/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/utils/common.py
+-rw-rw-rw-   0        0        0     4628 2023-07-11 05:41:09.000000 xj_push-1.0.4/xj_push/utils/custom_response.py
+-rw-rw-rw-   0        0        0    37715 2023-07-05 03:23:16.000000 xj_push-1.0.4/xj_push/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_push-1.0.4/xj_push/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7311 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/utils/model_handle.py
+-rw-rw-rw-   0        0        0     5145 2023-06-02 09:15:38.000000 xj_push-1.0.4/xj_push/utils/service_manager.py
+-rw-rw-rw-   0        0        0     5668 2023-07-05 05:42:50.000000 xj_push-1.0.4/xj_push/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     7924 2023-07-21 06:22:34.000000 xj_push-1.0.4/xj_push/utils/utility_method.py
+-rw-rw-rw-   0        0        0     2460 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/utils/utils.py
+-rw-rw-rw-   0        0        0     3385 2023-07-14 07:14:50.000000 xj_push-1.0.4/xj_push/utils/wechat.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push.egg-info/
+-rw-rw-rw-   0        0        0     1084 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 08:22:49.000000 xj_push-1.0.4/xj_push.egg-info/top_level.txt
```

### Comparing `xj_push-1.0.3/PKG-INFO` & `xj_push-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_push
-Version: 1.0.3
+Version: 1.0.4
 Summary: 推送模块
 License: apache 3.0
 Description-Content-Type: text/markdown
 
 # xj_push
 
 #### 介绍
```

### Comparing `xj_push-1.0.3/README.md` & `xj_push-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/setup.py` & `xj_push-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_push',  # 模块名称
-    version='1.0.3',  # 模块版本
+    version='1.0.4',  # 模块版本
     description='推送模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_payment'],  # 系指定安装模块
     license="apache 3.0",
```

### Comparing `xj_push-1.0.3/xj_push/admin.py` & `xj_push-1.0.4/xj_push/admin.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/apis/push_apis.py` & `xj_push-1.0.4/xj_push/apis/push_apis.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/apis/push_plan_apis.py` & `xj_push-1.0.4/xj_push/apis/push_plan_apis.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/apis/push_push_apis.py` & `xj_push-1.0.4/xj_push/apis/push_push_apis.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/apis/push_record_apis.py` & `xj_push-1.0.4/xj_push/apis/push_record_apis.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/apis/push_template_apis.py` & `xj_push-1.0.4/xj_push/apis/push_template_apis.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/common.py` & `xj_push-1.0.4/xj_push/common.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/models.py` & `xj_push-1.0.4/xj_push/models.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/push_pipeline/bx_custom_pipeline.py` & `xj_push-1.0.4/xj_push/push_pipeline/bx_custom_pipeline.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/push_pipeline/bx_visitor_pipeline.py` & `xj_push-1.0.4/xj_push/push_pipeline/bx_visitor_pipeline.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/push_pipeline/bx_worker_pipeline.py` & `xj_push-1.0.4/xj_push/push_pipeline/bx_worker_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 record_info = data
 
         return {prefix + k: v for k, v in record_info.items()}, None
 
     @staticmethod
     def process(*args, params: dict = None, **kwargs):
         """流程参数进入管道"""
-        write_to_log(prefix="推送", content="运行到这里")
         params, err = force_transform_type(variable=params, var_type="only_dict", default={})
         kwargs, err = force_transform_type(variable=kwargs, var_type="only_dict", default={})
         params.update(kwargs)
         params["push_current_time"] = time.strftime("%Y-%m-%d %H:%M:%S")
 
         # 获取报名相关的信息
         enroll_id = params.get("enroll_id", None)
```

### Comparing `xj_push-1.0.3/xj_push/push_pipeline/pipline_base.py` & `xj_push-1.0.4/xj_push/push_pipeline/pipline_base.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/service_register.py` & `xj_push-1.0.4/xj_push/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/services/push_plan_service.py` & `xj_push-1.0.4/xj_push/services/push_plan_service.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/services/push_record_service.py` & `xj_push-1.0.4/xj_push/services/push_record_service.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/services/push_service.py` & `xj_push-1.0.4/xj_push/services/push_service.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/services/push_template_main_service.py` & `xj_push-1.0.4/xj_push/services/push_template_main_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,11 +83,12 @@
                     prefix="小程序获取单点登录信息",
                     content="单点登录信息:" + str(user_id) + ";" + str(sub_appid) + "不存在",
                     err_obj=err
                 )
                 return None, err
             new_data['touser'] = sso.get("sso_unicode", "")
             wechat_user_info = applet_subscribe_message(new_data)
+            write_to_log(prefix="微信推送结果日志", content=wechat_user_info)
 
         # TODO 推送成功人数加一
         # print(new_data)
         return None, None
```

### Comparing `xj_push-1.0.3/xj_push/services/push_template_service.py` & `xj_push-1.0.4/xj_push/services/push_template_service.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/common.py` & `xj_push-1.0.4/xj_push/utils/common.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/custom_response.py` & `xj_push-1.0.4/xj_push/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/custom_tool.py` & `xj_push-1.0.4/xj_push/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/j_config.py` & `xj_push-1.0.4/xj_push/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/model_handle.py` & `xj_push-1.0.4/xj_push/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/service_manager.py` & `xj_push-1.0.4/xj_push/utils/service_manager.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/user_wrapper.py` & `xj_push-1.0.4/xj_push/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/utility_method.py` & `xj_push-1.0.4/xj_push/utils/utility_method.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/utils.py` & `xj_push-1.0.4/xj_push/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push/utils/wechat.py` & `xj_push-1.0.4/xj_push/utils/wechat.py`

 * *Files identical despite different names*

### Comparing `xj_push-1.0.3/xj_push.egg-info/PKG-INFO` & `xj_push-1.0.4/xj_push.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-push
-Version: 1.0.3
+Version: 1.0.4
 Summary: 推送模块
 License: apache 3.0
 Description-Content-Type: text/markdown
 
 # xj_push
 
 #### 介绍
```

### Comparing `xj_push-1.0.3/xj_push.egg-info/SOURCES.txt` & `xj_push-1.0.4/xj_push.egg-info/SOURCES.txt`

 * *Files identical despite different names*

