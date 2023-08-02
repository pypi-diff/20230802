# Comparing `tmp/huggingface_tool-0.0.4.tar.gz` & `tmp/huggingface_tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huggingface_tool-0.0.4.tar", last modified: Wed Jul 26 09:19:27 2023, max compression
+gzip compressed data, was "huggingface_tool-0.0.5.tar", last modified: Wed Aug  2 03:22:24 2023, max compression
```

## Comparing `huggingface_tool-0.0.4.tar` & `huggingface_tool-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:27.001184 huggingface_tool-0.0.4/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-07-05 08:02:03.000000 huggingface_tool-0.0.4/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     3053 2023-07-26 09:19:27.001043 huggingface_tool-0.0.4/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     1956 2023-07-26 09:17:43.000000 huggingface_tool-0.0.4/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.995038 huggingface_tool-0.0.4/huggingface_tool/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1113 2023-07-20 03:29:40.000000 huggingface_tool-0.0.4/huggingface_tool/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.996324 huggingface_tool-0.0.4/huggingface_tool/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 huggingface_tool-0.0.4/huggingface_tool/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4249 2023-07-26 08:28:45.000000 huggingface_tool-0.0.4/huggingface_tool/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.998549 huggingface_tool-0.0.4/huggingface_tool/savers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-05 05:24:38.000000 huggingface_tool-0.0.4/huggingface_tool/savers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      961 2023-07-12 05:17:52.000000 huggingface_tool-0.0.4/huggingface_tool/savers/base_model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1277 2023-07-12 05:19:30.000000 huggingface_tool-0.0.4/huggingface_tool/savers/base_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1025 2023-07-05 07:49:11.000000 huggingface_tool-0.0.4/huggingface_tool/savers/dataset_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      931 2023-07-12 05:17:52.000000 huggingface_tool-0.0.4/huggingface_tool/savers/diffusion_model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1779 2023-07-12 05:23:51.000000 huggingface_tool-0.0.4/huggingface_tool/savers/model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      861 2023-07-12 05:18:18.000000 huggingface_tool-0.0.4/huggingface_tool/savers/tokenizer_saver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:27.000004 huggingface_tool-0.0.4/huggingface_tool/uploaders/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-20 03:03:53.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1320 2023-07-20 03:23:56.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/base_uploader.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1655 2023-07-20 03:23:27.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/dataset_uploader.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1949 2023-07-26 09:16:10.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/model_uploader.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1776 2023-07-26 09:15:26.000000 huggingface_tool-0.0.4/huggingface_tool/uploaders/utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:27.000724 huggingface_tool-0.0.4/huggingface_tool/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 huggingface_tool-0.0.4/huggingface_tool/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1290 2023-07-05 05:32:09.000000 huggingface_tool-0.0.4/huggingface_tool/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1370 2023-07-05 05:21:26.000000 huggingface_tool-0.0.4/huggingface_tool/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-26 09:19:26.995837 huggingface_tool-0.0.4/huggingface_tool.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3053 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      958 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      213 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       17 2023-07-26 09:19:26.000000 huggingface_tool-0.0.4/huggingface_tool.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-26 09:19:27.001226 huggingface_tool-0.0.4/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2978 2023-07-20 02:39:22.000000 huggingface_tool-0.0.4/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.721953 huggingface_tool-0.0.5/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-07-05 08:02:03.000000 huggingface_tool-0.0.5/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3712 2023-08-02 03:22:24.721805 huggingface_tool-0.0.5/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2615 2023-08-02 03:18:39.000000 huggingface_tool-0.0.5/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.715261 huggingface_tool-0.0.5/huggingface_tool/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1113 2023-07-26 09:20:01.000000 huggingface_tool-0.0.5/huggingface_tool/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.716544 huggingface_tool-0.0.5/huggingface_tool/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 huggingface_tool-0.0.5/huggingface_tool/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5252 2023-08-02 03:21:28.000000 huggingface_tool-0.0.5/huggingface_tool/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.719205 huggingface_tool-0.0.5/huggingface_tool/savers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-05 05:24:38.000000 huggingface_tool-0.0.5/huggingface_tool/savers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      871 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/base_api_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      963 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/base_model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1280 2023-08-02 03:21:08.000000 huggingface_tool-0.0.5/huggingface_tool/savers/base_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1027 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/dataset_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      934 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/diffusion_model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1464 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/file_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1832 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1234 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/repo_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      864 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/savers/tokenizer_saver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.720791 huggingface_tool-0.0.5/huggingface_tool/uploaders/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-20 03:03:53.000000 huggingface_tool-0.0.5/huggingface_tool/uploaders/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1323 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/uploaders/base_uploader.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1701 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/uploaders/dataset_uploader.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1948 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/uploaders/model_uploader.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1905 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/uploaders/utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.721520 huggingface_tool-0.0.5/huggingface_tool/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 huggingface_tool-0.0.5/huggingface_tool/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1289 2023-08-02 03:21:26.000000 huggingface_tool-0.0.5/huggingface_tool/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1369 2023-08-02 03:21:25.000000 huggingface_tool-0.0.5/huggingface_tool/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-02 03:22:24.716021 huggingface_tool-0.0.5/huggingface_tool.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3712 2023-08-02 03:22:24.000000 huggingface_tool-0.0.5/huggingface_tool.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1076 2023-08-02 03:22:24.000000 huggingface_tool-0.0.5/huggingface_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-08-02 03:22:24.000000 huggingface_tool-0.0.5/huggingface_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-08-02 03:22:24.000000 huggingface_tool-0.0.5/huggingface_tool.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      213 2023-08-02 03:22:24.000000 huggingface_tool-0.0.5/huggingface_tool.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       17 2023-08-02 03:22:24.000000 huggingface_tool-0.0.5/huggingface_tool.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-08-02 03:22:24.722003 huggingface_tool-0.0.5/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2978 2023-07-20 02:39:22.000000 huggingface_tool-0.0.5/setup.py
```

### Comparing `huggingface_tool-0.0.4/LICENSE` & `huggingface_tool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.4/PKG-INFO` & `huggingface_tool-0.0.5/huggingface_tool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: huggingface_tool
-Version: 0.0.4
+Name: huggingface-tool
+Version: 0.0.5
 Summary: Toolkit for managing huggingface models and datasets
 Home-page: https://github.com/OpenRL-Lab/huggingface_tool
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/huggingface_tool
 Project-URL: Documentation, https://huggingface_tool.readthedocs.io/
 Keywords: huggingface toolkit
@@ -37,14 +37,20 @@
 
 `pip install huggingface-tool`
 
 ## Usage
 
 Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
 
+- Download and save a repo with: `htool save-repo <repo_id> <save_dir> -r <model/dataset>`. `-r` means the repo is a model or dataset repo. By default, it is a model repo.
+  - For example: `htool save-repo OpenRL/tizero ./tizero`
+  - For example: `htool save-repo OpenRL/DeepFakeFace ./DeepFakeFace -r dataset`
+- Download and save a file with: `htool save-file <repo_id>:<remote_filepath> <save_dir> -r <model/dataset>`. `-r` means the repo is a model or dataset repo. By default, it is a model repo.
+  - For example: `htool save-file OpenRL/tizero:actor.pt ./tizero`
+  - For example: `htool save-file OpenRL/DeepFakeFace:README.md ./DeepFakeFace -r dataset`
 - Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
   - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
```

### Comparing `huggingface_tool-0.0.4/README.md` & `huggingface_tool-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 `pip install huggingface-tool`
 
 ## Usage
 
 Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
 
+- Download and save a repo with: `htool save-repo <repo_id> <save_dir> -r <model/dataset>`. `-r` means the repo is a model or dataset repo. By default, it is a model repo.
+  - For example: `htool save-repo OpenRL/tizero ./tizero`
+  - For example: `htool save-repo OpenRL/DeepFakeFace ./DeepFakeFace -r dataset`
+- Download and save a file with: `htool save-file <repo_id>:<remote_filepath> <save_dir> -r <model/dataset>`. `-r` means the repo is a model or dataset repo. By default, it is a model repo.
+  - For example: `htool save-file OpenRL/tizero:actor.pt ./tizero`
+  - For example: `htool save-file OpenRL/DeepFakeFace:README.md ./DeepFakeFace -r dataset`
 - Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
   - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/__init__.py` & `huggingface_tool-0.0.5/huggingface_tool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "huggingface_tool"
-__VERSION__ = "v0.0.4"
+__VERSION__ = "v0.0.5"
 __DESCRIPTION__ = "Toolkit for managing huggingface models and datasets"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/cli/__init__.py` & `huggingface_tool-0.0.5/huggingface_tool/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.4/huggingface_tool/cli/cli.py` & `huggingface_tool-0.0.5/huggingface_tool/cli/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-import os
+
 
 import click
 from click.core import Context, Option
 from termcolor import colored
 
 from huggingface_tool import __AUTHOR__, __EMAIL__, __TITLE__, __VERSION__
 from huggingface_tool.utils.util import get_system_info
 
 
 def red(text: str):
     return colored(text, "red")
 
 
 def print_version(
-        ctx: Context,
-        param: Option,
-        value: bool,
+    ctx: Context,
+    param: Option,
+    value: bool,
 ) -> None:
     if not value or ctx.resilient_parsing:
         return
     click.secho(f"{__TITLE__.upper()} version: {red(__VERSION__)}")
     click.secho(f"Developed by {__AUTHOR__}, Email: {red(__EMAIL__)}")
     ctx.exit()
 
 
 def print_system_info(
-        ctx: Context,
-        param: Option,
-        value: bool,
+    ctx: Context,
+    param: Option,
+    value: bool,
 ) -> None:
     if not value or ctx.resilient_parsing:
         return
     info_dict = get_system_info()
     for key, value in info_dict.items():
         click.secho(f"- {key}: {red(value)}")
     ctx.exit()
@@ -84,71 +84,129 @@
 
 
 @cli.command()
 @click.argument("model_name")
 @click.argument("save_dir")
 def save_dm(model_name, save_dir):
     from huggingface_tool.savers.diffusion_model_saver import DiffusionModelSaver
+
     saver = DiffusionModelSaver(model_name)
     if saver.load():
         saver.save(save_dir)
     else:
         saver.logger.info("Model not found")
 
 
 @cli.command()
+@click.argument("file_name")
+@click.argument("save_dir")
+@click.option(
+    "--repo_type",
+    "-r",
+    type=click.Choice(
+        [
+            "model",
+            "dataset",
+        ]
+    ),
+    default="model",
+    help="repo type",
+)
+def save_file(file_name, save_dir, repo_type):
+    from huggingface_tool.savers.file_saver import FileSaver
+
+    saver = FileSaver(file_name, repo_type)
+    if saver.load():
+        saver.save(save_dir)
+    else:
+        saver.logger.info("File not found")
+
+
+@cli.command()
+@click.argument("repo_name")
+@click.argument("save_dir")
+@click.option(
+    "--repo_type",
+    "-r",
+    type=click.Choice(
+        [
+            "model",
+            "dataset",
+        ]
+    ),
+    default="model",
+    help="repo type",
+)
+def save_repo(repo_name, save_dir, repo_type):
+    from huggingface_tool.savers.repo_saver import RepoSaver
+
+    saver = RepoSaver(repo_name, repo_type)
+    if saver.load():
+        saver.save(save_dir)
+    else:
+        saver.logger.info("Repo not found")
+
+
+@cli.command()
 @click.argument("tokenizer_name")
 @click.argument("save_dir")
 def save_tk(tokenizer_name, save_dir):
     from huggingface_tool.savers.tokenizer_saver import TokenizerSaver
+
     saver = TokenizerSaver(tokenizer_name)
     if saver.load():
         saver.save(save_dir)
     else:
         saver.logger.info("Tokenizer not found")
 
 
 @cli.command()
 @click.argument("dataset_name")
 @click.argument("save_dir")
 def save_data(dataset_name, save_dir):
     from huggingface_tool.savers.dataset_saver import DatasetSaver
+
     saver = DatasetSaver(dataset_name)
     if saver.load():
         saver.save(save_dir)
     else:
         saver.logger.info("Dataset not found")
 
 
 @cli.command()
 @click.argument("model_class")
 @click.argument("model_name")
 @click.argument("save_dir")
 def save_model(model_class, model_name, save_dir):
     from huggingface_tool.savers.model_saver import ModelSaver
+
     saver = ModelSaver(model_class, model_name)
     if saver.load():
         saver.save(save_dir)
     else:
         saver.logger.info("Dataset not found")
 
+
 @cli.command()
 @click.argument("dataset_dir")
 @click.argument("dataset_name")
 def upload_data(dataset_dir, dataset_name):
     from huggingface_tool.uploaders.dataset_uploader import DatasetUploader
+
     uploader = DatasetUploader(dataset_dir, dataset_name)
     if uploader.check():
         uploader.push()
     else:
         uploader.logger.info("Dataset not valid")
 
+
 @cli.command()
 @click.argument("model_dir")
 @click.argument("model_name")
 def upload_model(model_dir, model_name):
     from huggingface_tool.uploaders.model_uploader import ModelUploader
+
     uploader = ModelUploader(model_dir, model_name)
     if uploader.check():
         uploader.push()
     else:
         uploader.logger.info("Dataset not valid")
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/__init__.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/base_model_saver.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/dataset_saver.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from abc import ABC
+import datasets
+
 from huggingface_tool.savers.base_saver import BaseSaver
 
-class BaseModelSaver(BaseSaver,ABC):
+
+class DatasetSaver(BaseSaver):
+    def _load(self, name: str):
+        return datasets.load_dataset(name)
+
     def save(self, save_dir: str):
         if self.loaded_object is None:
-            self.logger.info("No model loaded, cannot save")
+            self.logger.info("No dataset loaded, cannot save")
             return
-        self.loaded_object.save_pretrained(save_dir)
-
+        self.loaded_object.save_to_disk(save_dir)
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/base_saver.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/base_saver.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 
 """"""
 
 from abc import ABC, abstractmethod
 
 from huggingface_tool.utils.logger import Logger
 
+
 class BaseSaver(ABC):
-    def __init__(self, name:str):
+    def __init__(self, name: str):
         self.logger = Logger()
         self.name = name
         self.loaded_object = None
 
-
-
     def load(self) -> bool:
         try:
             self.loaded_object = self._load(self.name)
         except:
             self.logger.info(f"Could not load model from {self.name}")
             return False
         return True
 
     @abstractmethod
-    def _load(self,name:str):
+    def _load(self, name: str):
         raise NotImplementedError
 
     @abstractmethod
-    def save(self,save_dir: str):
+    def save(self, save_dir: str):
         raise NotImplementedError
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/dataset_saver.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/base_model_saver.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,21 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-import datasets
+from abc import ABC
 
 from huggingface_tool.savers.base_saver import BaseSaver
 
-class DatasetSaver(BaseSaver):
-    def _load(self,name:str):
-        return datasets.load_dataset(name)
 
+class BaseModelSaver(BaseSaver, ABC):
     def save(self, save_dir: str):
         if self.loaded_object is None:
-            self.logger.info("No dataset loaded, cannot save")
+            self.logger.info("No model loaded, cannot save")
             return
-        self.loaded_object.save_to_disk(save_dir)
-
+        self.loaded_object.save_pretrained(save_dir)
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/diffusion_model_saver.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/diffusion_model_saver.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from huggingface_tool.savers.base_model_saver import BaseModelSaver
-
 import torch
 from diffusers import StableDiffusionPipeline
 
+from huggingface_tool.savers.base_model_saver import BaseModelSaver
+
+
 class DiffusionModelSaver(BaseModelSaver):
-    def _load(self, name)->bool:
+    def _load(self, name) -> bool:
         return StableDiffusionPipeline.from_pretrained(name, torch_dtype=torch.float16)
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/model_saver.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/model_saver.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,24 +18,31 @@
 import transformers
 
 from huggingface_tool.savers.base_model_saver import BaseModelSaver
 
 model_class_dict = {
     "AutoModelForSeq2SeqLM": transformers.AutoModelForSeq2SeqLM,
     "AutoModelForCausalLM": transformers.AutoModelForCausalLM,
-    "AutoModelForSequenceClassification": transformers.AutoModelForSequenceClassification,
+    "AutoModelForSequenceClassification": (
+        transformers.AutoModelForSequenceClassification
+    ),
     "AutoModelForQuestionAnswering": transformers.AutoModelForQuestionAnswering,
     "AutoModelForTokenClassification": transformers.AutoModelForTokenClassification,
     "AutoModelForMultipleChoice": transformers.AutoModelForMultipleChoice,
-    "AutoModelForNextSentencePrediction": transformers.AutoModelForNextSentencePrediction,
+    "AutoModelForNextSentencePrediction": (
+        transformers.AutoModelForNextSentencePrediction
+    ),
     "AutoModelForPreTraining": transformers.AutoModelForPreTraining,
     "AutoModelForMaskedLM": transformers.AutoModelForMaskedLM,
-    "AutoModelForTableQuestionAnswering": transformers.AutoModelForTableQuestionAnswering,
+    "AutoModelForTableQuestionAnswering": (
+        transformers.AutoModelForTableQuestionAnswering
+    ),
 }
 
+
 class ModelSaver(BaseModelSaver):
-    def __init__(self, model_class:str, name:str):
+    def __init__(self, model_class: str, name: str):
         super().__init__(name)
         self.model_class = model_class
 
-    def _load(self,name):
-        return model_class_dict[self.model_class].from_pretrained(name)
+    def _load(self, name):
+        return model_class_dict[self.model_class].from_pretrained(name)
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/savers/tokenizer_saver.py` & `huggingface_tool-0.0.5/huggingface_tool/savers/tokenizer_saver.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 # limitations under the License.
 
 """"""
 from transformers import AutoTokenizer
 
 from huggingface_tool.savers.base_model_saver import BaseModelSaver
 
+
 class TokenizerSaver(BaseModelSaver):
-    def _load(self,name):
-        return AutoTokenizer.from_pretrained(name)
+    def _load(self, name):
+        return AutoTokenizer.from_pretrained(name)
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/uploaders/__init__.py` & `huggingface_tool-0.0.5/huggingface_tool/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.4/huggingface_tool/uploaders/base_uploader.py` & `huggingface_tool-0.0.5/huggingface_tool/uploaders/base_uploader.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from abc import ABC, abstractmethod
 
-
 from huggingface_tool.utils.logger import Logger
 
+
 class BaseUploader(ABC):
     def __init__(self, file_or_dir: str, remote_name: str) -> None:
         self.logger = Logger()
         self.file_or_dir = file_or_dir
         self.remote_name = remote_name
 
     @abstractmethod
     def check(self) -> bool:
         raise NotImplementedError
 
-    def push(self)->bool:
+    def push(self) -> bool:
         success = self._push()
         if success:
             self._success_message()
         return success
 
     @abstractmethod
     def _push(self) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def _success_message(self):
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/uploaders/dataset_uploader.py` & `huggingface_tool-0.0.5/huggingface_tool/uploaders/dataset_uploader.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from pathlib import Path
-from huggingface_tool.uploaders.base_uploader import BaseUploader
+
 from datasets import load_from_disk
 
+from huggingface_tool.uploaders.base_uploader import BaseUploader
+
 
 class DatasetUploader(BaseUploader):
     def __init__(self, file_or_dir: str, remote_name: str) -> None:
         super().__init__(file_or_dir, remote_name)
         self.dataset = None
 
     def check(self) -> bool:
-        assert Path(self.file_or_dir).exists(), f"File or directory {self.file_or_dir} does not exist"
+        assert Path(
+            self.file_or_dir
+        ).exists(), f"File or directory {self.file_or_dir} does not exist"
         try:
             self.dataset = load_from_disk(self.file_or_dir)
         except:
             print("Cannot load local dataset")
             return False
         return True
 
@@ -41,8 +45,10 @@
             self.dataset.push_to_hub(self.remote_name)
         except:
             print("Cannot push to hub")
             return False
         return True
 
     def _success_message(self):
-        print(f"Dataset is uploaded to https://huggingface.co/datasets/{self.remote_name}")
+        print(
+            f"Dataset is uploaded to https://huggingface.co/datasets/{self.remote_name}"
+        )
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/uploaders/model_uploader.py` & `huggingface_tool-0.0.5/huggingface_tool/uploaders/model_uploader.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import os
-
 from pathlib import Path
-from huggingface_tool.uploaders.base_uploader import BaseUploader
-from huggingface_hub import HfApi
-from huggingface_hub import ModelCard
 
+from huggingface_hub import HfApi, ModelCard
+
+from huggingface_tool.uploaders.base_uploader import BaseUploader
 from huggingface_tool.uploaders.utils import _huggingface_api_upload_dir
 
+
 class ModelUploader(BaseUploader):
     def __init__(self, file_or_dir: str, remote_name: str) -> None:
         super().__init__(file_or_dir, remote_name)
         self.model = None
 
     def check(self) -> bool:
-        assert Path(self.file_or_dir).exists(), f"File or directory {self.file_or_dir} does not exist"
+        assert Path(
+            self.file_or_dir
+        ).exists(), f"File or directory {self.file_or_dir} does not exist"
         return True
 
-    def push_modelcard(self)->bool:
-        card = ModelCard.load(os.path.join(self.file_or_dir,"README.md"))
+    def push_modelcard(self) -> bool:
+        card = ModelCard.load(os.path.join(self.file_or_dir, "README.md"))
         try:
             card.validate()
             card.push_to_hub(repo_id=self.remote_name)
         except:
             raise ValueError("model card info is invalid. please check.")
         return True
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/uploaders/utils.py` & `huggingface_tool-0.0.5/huggingface_tool/uploaders/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,37 +13,45 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
-
-def _huggingface_api_upload_file(api, path_or_fileobj, path_in_repo, repo_id, retry=5) -> bool:
+def _huggingface_api_upload_file(
+    api, path_or_fileobj, path_in_repo, repo_id, retry=5
+) -> bool:
     for retry_time in range(retry):
         try:
             api.upload_file(
                 path_or_fileobj=path_or_fileobj,
                 path_in_repo=path_in_repo,
                 repo_id=repo_id,
                 repo_type="model",
             )
             return True
         except:
             if retry_time == retry - 1:
-                print(f"Can not upload the {path_or_fileobj} after {retry} times retry, please check your network connection.")
+                print(
+                    f"Can not upload the {path_or_fileobj} after {retry} times retry,"
+                    " please check your network connection."
+                )
                 return False
 
+
 def _huggingface_api_upload_dir(api, folder_path, repo_id, retry=5) -> bool:
     for retry_time in range(retry):
         try:
             api.upload_folder(
                 folder_path=folder_path,
                 repo_id=repo_id,
                 repo_type="model",
                 ignore_patterns="README.md",
             )
             return True
         except:
             if retry_time == retry - 1:
-                print(f"Can not upload the model after {retry} times retry, please check your network connection.")
-                return False
+                print(
+                    f"Can not upload the model after {retry} times retry, please check"
+                    " your network connection."
+                )
+                return False
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/utils/__init__.py` & `huggingface_tool-0.0.5/huggingface_tool/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.4/huggingface_tool/utils/logger.py` & `huggingface_tool-0.0.5/huggingface_tool/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,20 @@
     ) -> None:
         # TODO: change these flags to log_backend
 
         self.log_level = log_level
         self._init()
 
     def _init(self) -> None:
-
         handlers = [RichHandler()]
 
         for handler in logging.root.handlers[:]:
             logging.root.removeHandler(handler)
 
         logging.basicConfig(
             level=self.log_level,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
-
     def info(self, msg: str):
-        logging.info(msg)
+        logging.info(msg)
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool/utils/util.py` & `huggingface_tool-0.0.5/huggingface_tool/utils/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 import platform
 import re
-
 from typing import Dict
 
 import numpy as np
 
 import huggingface_tool
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool.egg-info/PKG-INFO` & `huggingface_tool-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: huggingface-tool
-Version: 0.0.4
+Name: huggingface_tool
+Version: 0.0.5
 Summary: Toolkit for managing huggingface models and datasets
 Home-page: https://github.com/OpenRL-Lab/huggingface_tool
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/huggingface_tool
 Project-URL: Documentation, https://huggingface_tool.readthedocs.io/
 Keywords: huggingface toolkit
@@ -37,14 +37,20 @@
 
 `pip install huggingface-tool`
 
 ## Usage
 
 Firstly, you need to login with `huggingface-cli login` (you can create or find your token at [settings](https://huggingface.co/settings/tokens)).
 
+- Download and save a repo with: `htool save-repo <repo_id> <save_dir> -r <model/dataset>`. `-r` means the repo is a model or dataset repo. By default, it is a model repo.
+  - For example: `htool save-repo OpenRL/tizero ./tizero`
+  - For example: `htool save-repo OpenRL/DeepFakeFace ./DeepFakeFace -r dataset`
+- Download and save a file with: `htool save-file <repo_id>:<remote_filepath> <save_dir> -r <model/dataset>`. `-r` means the repo is a model or dataset repo. By default, it is a model repo.
+  - For example: `htool save-file OpenRL/tizero:actor.pt ./tizero`
+  - For example: `htool save-file OpenRL/DeepFakeFace:README.md ./DeepFakeFace -r dataset`
 - Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
   - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
```

### Comparing `huggingface_tool-0.0.4/huggingface_tool.egg-info/SOURCES.txt` & `huggingface_tool-0.0.5/huggingface_tool.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 huggingface_tool.egg-info/dependency_links.txt
 huggingface_tool.egg-info/entry_points.txt
 huggingface_tool.egg-info/requires.txt
 huggingface_tool.egg-info/top_level.txt
 huggingface_tool/cli/__init__.py
 huggingface_tool/cli/cli.py
 huggingface_tool/savers/__init__.py
+huggingface_tool/savers/base_api_saver.py
 huggingface_tool/savers/base_model_saver.py
 huggingface_tool/savers/base_saver.py
 huggingface_tool/savers/dataset_saver.py
 huggingface_tool/savers/diffusion_model_saver.py
+huggingface_tool/savers/file_saver.py
 huggingface_tool/savers/model_saver.py
+huggingface_tool/savers/repo_saver.py
 huggingface_tool/savers/tokenizer_saver.py
 huggingface_tool/uploaders/__init__.py
 huggingface_tool/uploaders/base_uploader.py
 huggingface_tool/uploaders/dataset_uploader.py
 huggingface_tool/uploaders/model_uploader.py
 huggingface_tool/uploaders/utils.py
 huggingface_tool/utils/__init__.py
```

### Comparing `huggingface_tool-0.0.4/setup.py` & `huggingface_tool-0.0.5/setup.py`

 * *Files identical despite different names*

