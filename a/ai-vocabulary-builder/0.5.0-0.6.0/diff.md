# Comparing `tmp/ai_vocabulary_builder-0.5.0.tar.gz` & `tmp/ai_vocabulary_builder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_vocabulary_builder-0.5.0.tar", max compression
+gzip compressed data, was "ai_vocabulary_builder-0.6.0.tar", max compression
```

## Comparing `ai_vocabulary_builder-0.5.0.tar` & `ai_vocabulary_builder-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
--rw-r--r--   0        0        0     1493 2023-03-04 00:47:58.835348 ai_vocabulary_builder-0.5.0/LICENSE
--rw-r--r--   0        0        0    10989 2023-04-01 07:46:46.581402 ai_vocabulary_builder-0.5.0/README.md
--rw-r--r--   0        0        0     1407 2023-04-01 07:46:46.582718 ai_vocabulary_builder-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-01 07:46:46.583289 ai_vocabulary_builder-0.5.0/voc_builder/__init__.py
--rw-r--r--   0        0        0     2627 2023-03-09 13:40:55.254383 ai_vocabulary_builder-0.5.0/voc_builder/builder.py
--rw-r--r--   0        0        0        0 2023-03-08 22:37:55.185350 ai_vocabulary_builder-0.5.0/voc_builder/commands/__init__.py
--rw-r--r--   0        0        0      314 2023-03-26 03:15:36.986387 ai_vocabulary_builder-0.5.0/voc_builder/commands/exceptions.py
--rw-r--r--   0        0        0     3011 2023-04-01 07:18:44.907276 ai_vocabulary_builder-0.5.0/voc_builder/commands/export.py
--rw-r--r--   0        0        0     1492 2023-03-26 03:15:36.986708 ai_vocabulary_builder-0.5.0/voc_builder/commands/parsers.py
--rw-r--r--   0        0        0     1353 2023-03-09 13:40:55.255032 ai_vocabulary_builder-0.5.0/voc_builder/commands/remove.py
--rw-r--r--   0        0        0      371 2023-03-25 23:51:10.501001 ai_vocabulary_builder-0.5.0/voc_builder/config.py
--rw-r--r--   0        0        0      322 2023-03-08 22:37:55.186812 ai_vocabulary_builder-0.5.0/voc_builder/exceptions.py
--rw-r--r--   0        0        0       36 2023-04-01 07:46:46.583649 ai_vocabulary_builder-0.5.0/voc_builder/int_commands/__init__.py
--rw-r--r--   0        0        0     2867 2023-04-01 07:46:46.584044 ai_vocabulary_builder-0.5.0/voc_builder/int_commands/remove.py
--rw-r--r--   0        0        0    23935 2023-04-01 07:46:46.584394 ai_vocabulary_builder-0.5.0/voc_builder/interactive.py
--rw-r--r--   0        0        0     3027 2023-03-26 03:43:50.346557 ai_vocabulary_builder-0.5.0/voc_builder/main.py
--rw-r--r--   0        0        0     3755 2023-03-26 03:55:50.069645 ai_vocabulary_builder-0.5.0/voc_builder/models.py
--rw-r--r--   0        0        0    10532 2023-04-01 07:27:35.414640 ai_vocabulary_builder-0.5.0/voc_builder/openai_svc.py
--rw-r--r--   0        0        0     8962 2023-04-01 07:46:46.584593 ai_vocabulary_builder-0.5.0/voc_builder/store.py
--rw-r--r--   0        0        0     1075 2023-04-01 06:34:24.361479 ai_vocabulary_builder-0.5.0/voc_builder/utils.py
--rw-r--r--   0        0        0     4556 2023-03-12 10:14:56.124104 ai_vocabulary_builder-0.5.0/voc_builder/version.py
--rw-r--r--   0        0        0    11819 1970-01-01 00:00:00.000000 ai_vocabulary_builder-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1493 2023-03-04 00:47:58.835348 ai_vocabulary_builder-0.6.0/LICENSE
+-rw-r--r--   0        0        0    11161 2023-08-02 05:56:00.731521 ai_vocabulary_builder-0.6.0/README.md
+-rw-r--r--   0        0        0     1566 2023-08-02 05:45:00.698962 ai_vocabulary_builder-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-02 05:36:50.519863 ai_vocabulary_builder-0.6.0/voc_builder/__init__.py
+-rw-r--r--   0        0        0     2627 2023-03-09 13:40:55.254383 ai_vocabulary_builder-0.6.0/voc_builder/builder.py
+-rw-r--r--   0        0        0        0 2023-03-08 22:37:55.185350 ai_vocabulary_builder-0.6.0/voc_builder/commands/__init__.py
+-rw-r--r--   0        0        0      314 2023-03-26 03:15:36.986387 ai_vocabulary_builder-0.6.0/voc_builder/commands/exceptions.py
+-rw-r--r--   0        0        0     3011 2023-04-01 07:18:44.907276 ai_vocabulary_builder-0.6.0/voc_builder/commands/export.py
+-rw-r--r--   0        0        0     1492 2023-03-26 03:15:36.986708 ai_vocabulary_builder-0.6.0/voc_builder/commands/parsers.py
+-rw-r--r--   0        0        0     1353 2023-03-09 13:40:55.255032 ai_vocabulary_builder-0.6.0/voc_builder/commands/remove.py
+-rw-r--r--   0        0        0      371 2023-03-25 23:51:10.501001 ai_vocabulary_builder-0.6.0/voc_builder/config.py
+-rw-r--r--   0        0        0      322 2023-03-08 22:37:55.186812 ai_vocabulary_builder-0.6.0/voc_builder/exceptions.py
+-rw-r--r--   0        0        0       36 2023-04-01 07:46:46.583649 ai_vocabulary_builder-0.6.0/voc_builder/int_commands/__init__.py
+-rw-r--r--   0        0        0     2867 2023-04-01 07:46:46.584044 ai_vocabulary_builder-0.6.0/voc_builder/int_commands/remove.py
+-rw-r--r--   0        0        0    23935 2023-04-01 07:46:46.584394 ai_vocabulary_builder-0.6.0/voc_builder/interactive.py
+-rw-r--r--   0        0        0     4674 2023-08-02 05:32:50.746143 ai_vocabulary_builder-0.6.0/voc_builder/main.py
+-rw-r--r--   0        0        0     3755 2023-03-26 03:55:50.069645 ai_vocabulary_builder-0.6.0/voc_builder/models.py
+-rw-r--r--   0        0        0        0 2023-04-30 23:39:50.943742 ai_vocabulary_builder-0.6.0/voc_builder/notepad/__init__.py
+-rw-r--r--   0        0        0    66018 2023-08-02 05:56:38.648406 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/assets/ManageView-42257840.js
+-rw-r--r--   0        0        0       77 2023-08-02 05:56:38.648363 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/assets/ManageView-9e02007a.css
+-rw-r--r--   0        0        0   164360 2023-08-02 05:56:38.648291 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0        0        0   121340 2023-08-02 05:56:38.648531 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0        0        0   277987 2023-08-02 05:56:38.648470 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/assets/index-0d03c8f7.css
+-rw-r--r--   0        0        0   217559 2023-08-02 05:56:38.648333 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/assets/index-0f01e30f.js
+-rw-r--r--   0        0        0      367 2023-08-02 05:56:38.647140 ai_vocabulary_builder-0.6.0/voc_builder/notepad/dist/index.html
+-rw-r--r--   0        0        0     7966 2023-08-02 05:32:50.762199 ai_vocabulary_builder-0.6.0/voc_builder/notepad/server.py
+-rw-r--r--   0        0        0    10532 2023-08-02 05:33:53.491441 ai_vocabulary_builder-0.6.0/voc_builder/openai_svc.py
+-rw-r--r--   0        0        0     8962 2023-07-31 11:10:46.630400 ai_vocabulary_builder-0.6.0/voc_builder/store.py
+-rw-r--r--   0        0        0     1075 2023-04-01 06:34:24.361479 ai_vocabulary_builder-0.6.0/voc_builder/utils.py
+-rw-r--r--   0        0        0     4556 2023-03-12 10:14:56.124104 ai_vocabulary_builder-0.6.0/voc_builder/version.py
+-rw-r--r--   0        0        0    12129 1970-01-01 00:00:00.000000 ai_vocabulary_builder-0.6.0/PKG-INFO
```

### Comparing `ai_vocabulary_builder-0.5.0/LICENSE` & `ai_vocabulary_builder-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/README.md` & `ai_vocabulary_builder-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,28 @@
 安装完成后，请在环境变量中设置你的 [OpenAI API key](https://platform.openai.com/account/api-keys)：
 
 ```console
 # 使用你在 OpenAI 官网上申请到的 key 替换该内容
 export OPENAI_API_KEY='your_api_key'
 ```
 
-之后执行 `aivoc run` 启动工具，进入交互式命令行模式。
+之后执行 `aivoc run` 启动工具，进入交互式命令行模式。或者执行 `aivoc notebook`，在浏览器中打开可交互式 Web App（推荐）。
 
 除环境变量外，你也可以通过 `--api-key` 参数完成设置：
 
 ```console
 aivoc run --api-key "your_api_key"
 ```
 
 ## 使用指南
 
+### 使用 Web App
+
+执行 `aivoc notebook` 命令，使用可交互式 Web App。
+
 ### 交互式命令行
 
 执行 `aivoc run` 命令，会进入交互式命令行模式，在该模式下，你可以快速完成添加生词、阅读故事等操作。
 
 #### 添加生词
 
 默认情况下，命令行处于“添加生词”模式，此时你可以直接粘贴一小段英文：
```

### Comparing `ai_vocabulary_builder-0.5.0/pyproject.toml` & `ai_vocabulary_builder-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [tool.poetry]
 name = "ai-vocabulary-builder"
-version = "0.5.0"
+version = "0.6.0"
 description = "A tool help you build your vocabulary book using AI."
 readme = "README.md"
 authors = ["piglei <piglei2007@gmail.com>"]
 packages = [
     { include = "voc_builder", from="." },
 ]
+include = [
+    { path = "voc_builder/notepad/dist/**/*"},
+]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<4.0"
+python = ">=3.8,<4.0"
 click = "^8.0.0"
 openai = "^0.27.0"
 rich = "^13.0.0"
 tinydb = "^4.7.1"
 questionary = "^1.10.0"
 prompt-toolkit = "^3.0.38"
 packaging = "^23.0"
 pendulum = "^2.1.2"
+fastapi = "^0.95.1"
+uvicorn = {extras = ["standard"], version = "^0.22.0"}
+sse-starlette = "^1.3.4"
 
 [tool.poetry.scripts]
 aivoc = "voc_builder.main:main"
 
 [[tool.poetry.source]]
 default = true
 name = "tencent-mirror"
```

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/builder.py` & `ai_vocabulary_builder-0.6.0/voc_builder/builder.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/commands/export.py` & `ai_vocabulary_builder-0.6.0/voc_builder/commands/export.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/commands/parsers.py` & `ai_vocabulary_builder-0.6.0/voc_builder/commands/parsers.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/commands/remove.py` & `ai_vocabulary_builder-0.6.0/voc_builder/commands/remove.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/int_commands/remove.py` & `ai_vocabulary_builder-0.6.0/voc_builder/int_commands/remove.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/interactive.py` & `ai_vocabulary_builder-0.6.0/voc_builder/interactive.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/models.py` & `ai_vocabulary_builder-0.6.0/voc_builder/models.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/openai_svc.py` & `ai_vocabulary_builder-0.6.0/voc_builder/openai_svc.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/store.py` & `ai_vocabulary_builder-0.6.0/voc_builder/store.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/utils.py` & `ai_vocabulary_builder-0.6.0/voc_builder/utils.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/voc_builder/version.py` & `ai_vocabulary_builder-0.6.0/voc_builder/version.py`

 * *Files identical despite different names*

### Comparing `ai_vocabulary_builder-0.5.0/PKG-INFO` & `ai_vocabulary_builder-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: ai-vocabulary-builder
-Version: 0.5.0
+Version: 0.6.0
 Summary: A tool help you build your vocabulary book using AI.
 Author: piglei
 Author-email: piglei2007@gmail.com
-Requires-Python: >=3.7.1,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
+Requires-Dist: sse-starlette (>=1.3.4,<2.0.0)
 Requires-Dist: tinydb (>=4.7.1,<5.0.0)
+Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 # AI 生词本
 
 AI 生词本（“AI Vocabulary Builder” 简称 aivoc）是一个利用了 AI 技术的智能生词本工具，它能帮你快速构建起自己的生词库，学习起来事半功倍。
 
 核心功能：
@@ -53,24 +56,28 @@
 安装完成后，请在环境变量中设置你的 [OpenAI API key](https://platform.openai.com/account/api-keys)：
 
 ```console
 # 使用你在 OpenAI 官网上申请到的 key 替换该内容
 export OPENAI_API_KEY='your_api_key'
 ```
 
-之后执行 `aivoc run` 启动工具，进入交互式命令行模式。
+之后执行 `aivoc run` 启动工具，进入交互式命令行模式。或者执行 `aivoc notebook`，在浏览器中打开可交互式 Web App（推荐）。
 
 除环境变量外，你也可以通过 `--api-key` 参数完成设置：
 
 ```console
 aivoc run --api-key "your_api_key"
 ```
 
 ## 使用指南
 
+### 使用 Web App
+
+执行 `aivoc notebook` 命令，使用可交互式 Web App。
+
 ### 交互式命令行
 
 执行 `aivoc run` 命令，会进入交互式命令行模式，在该模式下，你可以快速完成添加生词、阅读故事等操作。
 
 #### 添加生词
 
 默认情况下，命令行处于“添加生词”模式，此时你可以直接粘贴一小段英文：
```

