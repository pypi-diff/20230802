# Comparing `tmp/codedog-0.5.1.tar.gz` & `tmp/codedog-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedog-0.5.1.tar", max compression
+gzip compressed data, was "codedog-0.5.2.tar", max compression
```

## Comparing `codedog-0.5.1.tar` & `codedog-0.5.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1067 2023-07-29 15:15:38.422410 codedog-0.5.1/LICENSE
--rw-r--r--   0        0        0     1874 2023-07-31 08:08:49.444268 codedog-0.5.1/README.md
--rw-r--r--   0        0        0      328 2023-07-29 14:08:34.763306 codedog-0.5.1/codedog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.763486 codedog-0.5.1/codedog/actors/__init__.py
--rw-r--r--   0        0        0       22 2023-07-29 14:08:34.764323 codedog-0.5.1/codedog/actors/base.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.764498 codedog-0.5.1/codedog/actors/reporters/__init__.py
--rw-r--r--   0        0        0      198 2023-07-29 14:08:34.765314 codedog-0.5.1/codedog/actors/reporters/base.py
--rw-r--r--   0        0        0     1078 2023-07-29 14:08:34.766198 codedog-0.5.1/codedog/actors/reporters/code_review.py
--rw-r--r--   0        0        0     2793 2023-07-29 14:08:34.766867 codedog-0.5.1/codedog/actors/reporters/pr_summary.py
--rw-r--r--   0        0        0     2207 2023-07-29 14:08:34.767415 codedog-0.5.1/codedog/actors/reporters/pull_request.py
--rw-r--r--   0        0        0      167 2023-07-29 14:08:34.768840 codedog-0.5.1/codedog/chains/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.769200 codedog-0.5.1/codedog/chains/code_review/__init__.py
--rw-r--r--   0        0        0     4326 2023-08-02 11:24:29.515309 codedog-0.5.1/codedog/chains/code_review/base.py
--rw-r--r--   0        0        0      231 2023-07-29 14:08:34.771037 codedog-0.5.1/codedog/chains/code_review/prompts.py
--rw-r--r--   0        0        0        0 2023-07-25 09:19:30.869415 codedog-0.5.1/codedog/chains/pr_summary/__init__.py
--rw-r--r--   0        0        0     6524 2023-08-02 11:24:29.516303 codedog-0.5.1/codedog/chains/pr_summary/base.py
--rw-r--r--   0        0        0      579 2023-07-25 09:19:30.871812 codedog-0.5.1/codedog/chains/pr_summary/prompts.py
--rw-r--r--   0        0        0      714 2023-07-29 14:08:34.772749 codedog-0.5.1/codedog/localization.py
--rw-r--r--   0        0        0      738 2023-07-29 14:08:34.773960 codedog-0.5.1/codedog/models/__init__.py
--rw-r--r--   0        0        0      408 2023-07-25 09:19:30.873666 codedog-0.5.1/codedog/models/blob.py
--rw-r--r--   0        0        0     2018 2023-07-29 14:08:34.775025 codedog-0.5.1/codedog/models/change_file.py
--rw-r--r--   0        0        0      192 2023-07-25 09:19:30.874838 codedog-0.5.1/codedog/models/change_summary.py
--rw-r--r--   0        0        0      150 2023-07-29 14:08:34.775873 codedog-0.5.1/codedog/models/code_review.py
--rw-r--r--   0        0        0      800 2023-07-25 09:19:34.757440 codedog-0.5.1/codedog/models/commit.py
--rw-r--r--   0        0        0     1148 2023-07-25 09:19:34.758316 codedog-0.5.1/codedog/models/diff.py
--rw-r--r--   0        0        0      824 2023-07-25 09:19:34.759325 codedog-0.5.1/codedog/models/issue.py
--rw-r--r--   0        0        0      692 2023-07-29 14:08:34.776835 codedog-0.5.1/codedog/models/pr_summary.py
--rw-r--r--   0        0        0     1703 2023-07-29 14:08:34.778019 codedog-0.5.1/codedog/models/pull_request.py
--rw-r--r--   0        0        0      998 2023-07-25 09:19:34.760856 codedog-0.5.1/codedog/models/repository.py
--rw-r--r--   0        0        0      111 2023-07-29 14:08:34.778655 codedog-0.5.1/codedog/processors/__init__.py
--rw-r--r--   0        0        0     3835 2023-07-29 14:08:34.779662 codedog-0.5.1/codedog/processors/pull_request_processor.py
--rw-r--r--   0        0        0      178 2023-07-25 09:19:30.876958 codedog-0.5.1/codedog/retrievers/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-25 09:19:30.877473 codedog-0.5.1/codedog/retrievers/base.py
--rw-r--r--   0        0        0     8663 2023-07-29 14:08:34.780419 codedog-0.5.1/codedog/retrievers/github_retriever.py
--rw-r--r--   0        0        0      126 2023-07-29 14:08:34.781526 codedog-0.5.1/codedog/retrievers/gitlab_retriever.py
--rw-r--r--   0        0        0        0 2023-07-14 03:09:00.196876 codedog-0.5.1/codedog/templates/__init__.py
--rw-r--r--   0        0        0     2910 2023-07-21 05:12:00.256318 codedog-0.5.1/codedog/templates/grimoire_cn.py
--rw-r--r--   0        0        0     4542 2023-07-29 14:08:34.783652 codedog-0.5.1/codedog/templates/grimoire_en.py
--rw-r--r--   0        0        0     1018 2023-07-21 05:12:00.257443 codedog-0.5.1/codedog/templates/template_cn.py
--rw-r--r--   0        0        0     3387 2023-07-29 14:08:34.785033 codedog-0.5.1/codedog/templates/template_en.py
--rw-r--r--   0        0        0        0 2023-08-02 11:24:29.516578 codedog-0.5.1/codedog/utils/__init__.py
--rw-r--r--   0        0        0      486 2023-07-25 09:19:30.882119 codedog-0.5.1/codedog/utils/diff_utils.py
--rw-r--r--   0        0        0      935 2023-07-29 14:08:34.791991 codedog-0.5.1/codedog/utils/langchain_utils.py
--rw-r--r--   0        0        0      118 2023-08-02 12:15:57.996088 codedog-0.5.1/codedog/version.py
--rw-r--r--   0        0        0     1780 2023-08-02 12:26:24.376828 codedog-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-29 15:15:38.422410 codedog-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1874 2023-07-31 08:08:49.444268 codedog-0.5.2/README.md
+-rw-r--r--   0        0        0      328 2023-07-29 14:08:34.763306 codedog-0.5.2/codedog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:08:34.763486 codedog-0.5.2/codedog/actors/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-29 14:08:34.764323 codedog-0.5.2/codedog/actors/base.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:08:34.764498 codedog-0.5.2/codedog/actors/reporters/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-29 14:08:34.765314 codedog-0.5.2/codedog/actors/reporters/base.py
+-rw-r--r--   0        0        0     1078 2023-07-29 14:08:34.766198 codedog-0.5.2/codedog/actors/reporters/code_review.py
+-rw-r--r--   0        0        0     2793 2023-07-29 14:08:34.766867 codedog-0.5.2/codedog/actors/reporters/pr_summary.py
+-rw-r--r--   0        0        0     2207 2023-07-29 14:08:34.767415 codedog-0.5.2/codedog/actors/reporters/pull_request.py
+-rw-r--r--   0        0        0      167 2023-07-29 14:08:34.768840 codedog-0.5.2/codedog/chains/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:08:34.769200 codedog-0.5.2/codedog/chains/code_review/__init__.py
+-rw-r--r--   0        0        0     4338 2023-08-02 12:41:46.001586 codedog-0.5.2/codedog/chains/code_review/base.py
+-rw-r--r--   0        0        0      231 2023-07-29 14:08:34.771037 codedog-0.5.2/codedog/chains/code_review/prompts.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:19:30.869415 codedog-0.5.2/codedog/chains/pr_summary/__init__.py
+-rw-r--r--   0        0        0     6524 2023-08-02 12:40:59.303816 codedog-0.5.2/codedog/chains/pr_summary/base.py
+-rw-r--r--   0        0        0      579 2023-07-25 09:19:30.871812 codedog-0.5.2/codedog/chains/pr_summary/prompts.py
+-rw-r--r--   0        0        0      714 2023-07-29 14:08:34.772749 codedog-0.5.2/codedog/localization.py
+-rw-r--r--   0        0        0      738 2023-07-29 14:08:34.773960 codedog-0.5.2/codedog/models/__init__.py
+-rw-r--r--   0        0        0      408 2023-07-25 09:19:30.873666 codedog-0.5.2/codedog/models/blob.py
+-rw-r--r--   0        0        0     2018 2023-07-29 14:08:34.775025 codedog-0.5.2/codedog/models/change_file.py
+-rw-r--r--   0        0        0      192 2023-07-25 09:19:30.874838 codedog-0.5.2/codedog/models/change_summary.py
+-rw-r--r--   0        0        0      150 2023-07-29 14:08:34.775873 codedog-0.5.2/codedog/models/code_review.py
+-rw-r--r--   0        0        0      800 2023-07-25 09:19:34.757440 codedog-0.5.2/codedog/models/commit.py
+-rw-r--r--   0        0        0     1148 2023-07-25 09:19:34.758316 codedog-0.5.2/codedog/models/diff.py
+-rw-r--r--   0        0        0      824 2023-07-25 09:19:34.759325 codedog-0.5.2/codedog/models/issue.py
+-rw-r--r--   0        0        0      692 2023-07-29 14:08:34.776835 codedog-0.5.2/codedog/models/pr_summary.py
+-rw-r--r--   0        0        0     1703 2023-07-29 14:08:34.778019 codedog-0.5.2/codedog/models/pull_request.py
+-rw-r--r--   0        0        0      998 2023-07-25 09:19:34.760856 codedog-0.5.2/codedog/models/repository.py
+-rw-r--r--   0        0        0      111 2023-07-29 14:08:34.778655 codedog-0.5.2/codedog/processors/__init__.py
+-rw-r--r--   0        0        0     3835 2023-07-29 14:08:34.779662 codedog-0.5.2/codedog/processors/pull_request_processor.py
+-rw-r--r--   0        0        0      178 2023-07-25 09:19:30.876958 codedog-0.5.2/codedog/retrievers/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-25 09:19:30.877473 codedog-0.5.2/codedog/retrievers/base.py
+-rw-r--r--   0        0        0     8663 2023-07-29 14:08:34.780419 codedog-0.5.2/codedog/retrievers/github_retriever.py
+-rw-r--r--   0        0        0      126 2023-07-29 14:08:34.781526 codedog-0.5.2/codedog/retrievers/gitlab_retriever.py
+-rw-r--r--   0        0        0        0 2023-07-14 03:09:00.196876 codedog-0.5.2/codedog/templates/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-21 05:12:00.256318 codedog-0.5.2/codedog/templates/grimoire_cn.py
+-rw-r--r--   0        0        0     4542 2023-07-29 14:08:34.783652 codedog-0.5.2/codedog/templates/grimoire_en.py
+-rw-r--r--   0        0        0     1018 2023-07-21 05:12:00.257443 codedog-0.5.2/codedog/templates/template_cn.py
+-rw-r--r--   0        0        0     3387 2023-07-29 14:08:34.785033 codedog-0.5.2/codedog/templates/template_en.py
+-rw-r--r--   0        0        0        0 2023-08-02 11:24:29.516578 codedog-0.5.2/codedog/utils/__init__.py
+-rw-r--r--   0        0        0      486 2023-07-25 09:19:30.882119 codedog-0.5.2/codedog/utils/diff_utils.py
+-rw-r--r--   0        0        0      935 2023-07-29 14:08:34.791991 codedog-0.5.2/codedog/utils/langchain_utils.py
+-rw-r--r--   0        0        0      118 2023-08-02 12:15:57.996088 codedog-0.5.2/codedog/version.py
+-rw-r--r--   0        0        0     1781 2023-08-02 12:42:59.142319 codedog-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.2/PKG-INFO
```

### Comparing `codedog-0.5.1/LICENSE` & `codedog-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/README.md` & `codedog-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/actors/reporters/code_review.py` & `codedog-0.5.2/codedog/actors/reporters/code_review.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/actors/reporters/pr_summary.py` & `codedog-0.5.2/codedog/actors/reporters/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/actors/reporters/pull_request.py` & `codedog-0.5.2/codedog/actors/reporters/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/chains/code_review/base.py` & `codedog-0.5.2/codedog/chains/code_review/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
         code_files: List[ChangeFile] = self.processor.get_diff_code_files(pr)
 
         code_review_inputs = self._process_code_review_inputs(code_files, _run_manager)
         code_review_outputs = (
-            self.chain.aapply(code_review_inputs, callbacks=_run_manager.get_child(tag="CodeReview"))
+            await self.chain.aapply(code_review_inputs, callbacks=_run_manager.get_child(tag="CodeReview"))
             if code_review_inputs
             else []
         )
 
         return self._process_result(code_files, code_review_outputs)
 
     def _process_code_review_inputs(
@@ -95,15 +95,15 @@
                 "language": SUFFIX_LANGUAGE_MAPPING.get(code_file.suffix, ""),
             }
             input_data.append(input_item)
 
         run_manager.on_text(f"Prepare code diff content for {len(input_data)} files.\n")
         return input_data
 
-    def _process_result(self, code_files: List[ChangeFile], code_review_outputs):
+    def _process_result(self, code_files: List[ChangeFile], code_review_outputs: List):
         code_reviews = []
         for i, o in zip_longest(code_files, code_review_outputs):
             code_reviews.append(CodeReview(file=i, review=o["text"]))
         return {"code_reviews": code_reviews}
 
     @classmethod
     def from_llm(
```

### Comparing `codedog-0.5.1/codedog/chains/pr_summary/base.py` & `codedog-0.5.2/codedog/chains/pr_summary/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/chains/pr_summary/prompts.py` & `codedog-0.5.2/codedog/chains/pr_summary/prompts.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/localization.py` & `codedog-0.5.2/codedog/localization.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/__init__.py` & `codedog-0.5.2/codedog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/change_file.py` & `codedog-0.5.2/codedog/models/change_file.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/commit.py` & `codedog-0.5.2/codedog/models/commit.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/diff.py` & `codedog-0.5.2/codedog/models/diff.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/issue.py` & `codedog-0.5.2/codedog/models/issue.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/pr_summary.py` & `codedog-0.5.2/codedog/models/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/pull_request.py` & `codedog-0.5.2/codedog/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/models/repository.py` & `codedog-0.5.2/codedog/models/repository.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/processors/pull_request_processor.py` & `codedog-0.5.2/codedog/processors/pull_request_processor.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/retrievers/base.py` & `codedog-0.5.2/codedog/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/retrievers/github_retriever.py` & `codedog-0.5.2/codedog/retrievers/github_retriever.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/templates/grimoire_cn.py` & `codedog-0.5.2/codedog/templates/grimoire_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/templates/grimoire_en.py` & `codedog-0.5.2/codedog/templates/grimoire_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/templates/template_cn.py` & `codedog-0.5.2/codedog/templates/template_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/templates/template_en.py` & `codedog-0.5.2/codedog/templates/template_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/codedog/utils/langchain_utils.py` & `codedog-0.5.2/codedog/utils/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.1/pyproject.toml` & `codedog-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codedog"
-version = "0.5.1"
+version = "0.5.2"
 license = "MIT"
 readme = "README.md"
 authors = ["Arcadia <arcadia822@gmail.com>", "Linpp "]
 description = "Codedog reviews your pull request using llm."
 repository = "https://www.github.com/codedog-ai/codedog"
 homepage = "https://www.codedog.ai"
 keywords = ["code review", "langchain", "llm"]
@@ -66,12 +66,12 @@
 version_variable = ["codedog/version.py:VERSION"]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 
 [tool.semantic_release.remote]
 ignore_token_for_push = true
 
 [tool.semantic_release.publish]
-upload_to_vcs_release = true
+upload_to_vcs_release = false
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `codedog-0.5.1/PKG-INFO` & `codedog-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedog
-Version: 0.5.1
+Version: 0.5.2
 Summary: Codedog reviews your pull request using llm.
 Home-page: https://www.codedog.ai
 License: MIT
 Keywords: code review,langchain,llm
 Author: Arcadia
 Author-email: arcadia822@gmail.com
 Requires-Python: >=3.10,<3.11
```

