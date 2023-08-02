# Comparing `tmp/codedog-0.5.0.tar.gz` & `tmp/codedog-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedog-0.5.0.tar", max compression
+gzip compressed data, was "codedog-0.5.1.tar", max compression
```

## Comparing `codedog-0.5.0.tar` & `codedog-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,46 @@
--rw-r--r--   0        0        0     1067 2023-07-29 15:15:38.422410 codedog-0.5.0/LICENSE
--rw-r--r--   0        0        0     2409 2023-07-29 15:59:46.295233 codedog-0.5.0/README.md
--rw-r--r--   0        0        0      328 2023-07-29 14:08:34.763306 codedog-0.5.0/codedog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.763486 codedog-0.5.0/codedog/actors/__init__.py
--rw-r--r--   0        0        0       22 2023-07-29 14:08:34.764323 codedog-0.5.0/codedog/actors/base.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.764498 codedog-0.5.0/codedog/actors/reporters/__init__.py
--rw-r--r--   0        0        0      198 2023-07-29 14:08:34.765314 codedog-0.5.0/codedog/actors/reporters/base.py
--rw-r--r--   0        0        0     1078 2023-07-29 14:08:34.766198 codedog-0.5.0/codedog/actors/reporters/code_review.py
--rw-r--r--   0        0        0     2793 2023-07-29 14:08:34.766867 codedog-0.5.0/codedog/actors/reporters/pr_summary.py
--rw-r--r--   0        0        0     2207 2023-07-29 14:08:34.767415 codedog-0.5.0/codedog/actors/reporters/pull_request.py
--rw-r--r--   0        0        0      167 2023-07-29 14:08:34.768840 codedog-0.5.0/codedog/chains/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.769200 codedog-0.5.0/codedog/chains/code_review/__init__.py
--rw-r--r--   0        0        0     4324 2023-07-29 14:08:34.770173 codedog-0.5.0/codedog/chains/code_review/base.py
--rw-r--r--   0        0        0      231 2023-07-29 14:08:34.771037 codedog-0.5.0/codedog/chains/code_review/prompts.py
--rw-r--r--   0        0        0        0 2023-07-25 09:19:30.869415 codedog-0.5.0/codedog/chains/pr_summary/__init__.py
--rw-r--r--   0        0        0     6543 2023-07-29 14:08:34.771959 codedog-0.5.0/codedog/chains/pr_summary/base.py
--rw-r--r--   0        0        0      579 2023-07-25 09:19:30.871812 codedog-0.5.0/codedog/chains/pr_summary/prompts.py
--rw-r--r--   0        0        0      714 2023-07-29 14:08:34.772749 codedog-0.5.0/codedog/localization.py
--rw-r--r--   0        0        0      738 2023-07-29 14:08:34.773960 codedog-0.5.0/codedog/models/__init__.py
--rw-r--r--   0        0        0      408 2023-07-25 09:19:30.873666 codedog-0.5.0/codedog/models/blob.py
--rw-r--r--   0        0        0     2018 2023-07-29 14:08:34.775025 codedog-0.5.0/codedog/models/change_file.py
--rw-r--r--   0        0        0      192 2023-07-25 09:19:30.874838 codedog-0.5.0/codedog/models/change_summary.py
--rw-r--r--   0        0        0      150 2023-07-29 14:08:34.775873 codedog-0.5.0/codedog/models/code_review.py
--rw-r--r--   0        0        0      800 2023-07-25 09:19:34.757440 codedog-0.5.0/codedog/models/commit.py
--rw-r--r--   0        0        0     1148 2023-07-25 09:19:34.758316 codedog-0.5.0/codedog/models/diff.py
--rw-r--r--   0        0        0      824 2023-07-25 09:19:34.759325 codedog-0.5.0/codedog/models/issue.py
--rw-r--r--   0        0        0      692 2023-07-29 14:08:34.776835 codedog-0.5.0/codedog/models/pr_summary.py
--rw-r--r--   0        0        0     1703 2023-07-29 14:08:34.778019 codedog-0.5.0/codedog/models/pull_request.py
--rw-r--r--   0        0        0      998 2023-07-25 09:19:34.760856 codedog-0.5.0/codedog/models/repository.py
--rw-r--r--   0        0        0      111 2023-07-29 14:08:34.778655 codedog-0.5.0/codedog/processors/__init__.py
--rw-r--r--   0        0        0     3835 2023-07-29 14:08:34.779662 codedog-0.5.0/codedog/processors/pull_request_processor.py
--rw-r--r--   0        0        0      178 2023-07-25 09:19:30.876958 codedog-0.5.0/codedog/retrievers/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-25 09:19:30.877473 codedog-0.5.0/codedog/retrievers/base.py
--rw-r--r--   0        0        0     8663 2023-07-29 14:08:34.780419 codedog-0.5.0/codedog/retrievers/github_retriever.py
--rw-r--r--   0        0        0      126 2023-07-29 14:08:34.781526 codedog-0.5.0/codedog/retrievers/gitlab_retriever.py
--rw-r--r--   0        0        0     4855 2023-07-29 15:15:38.423468 codedog-0.5.0/codedog/server.py
--rw-r--r--   0        0        0        0 2023-07-14 03:09:00.196876 codedog-0.5.0/codedog/templates/__init__.py
--rw-r--r--   0        0        0     2910 2023-07-21 05:12:00.256318 codedog-0.5.0/codedog/templates/grimoire_cn.py
--rw-r--r--   0        0        0     4542 2023-07-29 14:08:34.783652 codedog-0.5.0/codedog/templates/grimoire_en.py
--rw-r--r--   0        0        0     1018 2023-07-21 05:12:00.257443 codedog-0.5.0/codedog/templates/template_cn.py
--rw-r--r--   0        0        0     3387 2023-07-29 14:08:34.785033 codedog-0.5.0/codedog/templates/template_en.py
--rw-r--r--   0        0        0      966 2023-07-29 14:08:34.786608 codedog-0.5.0/codedog/utils/__init__.py
--rw-r--r--   0        0        0      486 2023-07-25 09:19:30.882119 codedog-0.5.0/codedog/utils/diff_utils.py
--rw-r--r--   0        0        0      132 2023-07-29 15:15:38.424455 codedog-0.5.0/codedog/utils/github_utils.py
--rw-r--r--   0        0        0      935 2023-07-29 14:08:34.791991 codedog-0.5.0/codedog/utils/langchain_utils.py
--rw-r--r--   0        0        0      118 2023-07-29 14:09:43.784772 codedog-0.5.0/codedog/version.py
--rw-r--r--   0        0        0     1682 2023-07-29 15:58:10.321824 codedog-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 codedog-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-29 15:15:38.422410 codedog-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1874 2023-07-31 08:08:49.444268 codedog-0.5.1/README.md
+-rw-r--r--   0        0        0      328 2023-07-29 14:08:34.763306 codedog-0.5.1/codedog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:08:34.763486 codedog-0.5.1/codedog/actors/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-29 14:08:34.764323 codedog-0.5.1/codedog/actors/base.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:08:34.764498 codedog-0.5.1/codedog/actors/reporters/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-29 14:08:34.765314 codedog-0.5.1/codedog/actors/reporters/base.py
+-rw-r--r--   0        0        0     1078 2023-07-29 14:08:34.766198 codedog-0.5.1/codedog/actors/reporters/code_review.py
+-rw-r--r--   0        0        0     2793 2023-07-29 14:08:34.766867 codedog-0.5.1/codedog/actors/reporters/pr_summary.py
+-rw-r--r--   0        0        0     2207 2023-07-29 14:08:34.767415 codedog-0.5.1/codedog/actors/reporters/pull_request.py
+-rw-r--r--   0        0        0      167 2023-07-29 14:08:34.768840 codedog-0.5.1/codedog/chains/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:08:34.769200 codedog-0.5.1/codedog/chains/code_review/__init__.py
+-rw-r--r--   0        0        0     4326 2023-08-02 11:24:29.515309 codedog-0.5.1/codedog/chains/code_review/base.py
+-rw-r--r--   0        0        0      231 2023-07-29 14:08:34.771037 codedog-0.5.1/codedog/chains/code_review/prompts.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:19:30.869415 codedog-0.5.1/codedog/chains/pr_summary/__init__.py
+-rw-r--r--   0        0        0     6524 2023-08-02 11:24:29.516303 codedog-0.5.1/codedog/chains/pr_summary/base.py
+-rw-r--r--   0        0        0      579 2023-07-25 09:19:30.871812 codedog-0.5.1/codedog/chains/pr_summary/prompts.py
+-rw-r--r--   0        0        0      714 2023-07-29 14:08:34.772749 codedog-0.5.1/codedog/localization.py
+-rw-r--r--   0        0        0      738 2023-07-29 14:08:34.773960 codedog-0.5.1/codedog/models/__init__.py
+-rw-r--r--   0        0        0      408 2023-07-25 09:19:30.873666 codedog-0.5.1/codedog/models/blob.py
+-rw-r--r--   0        0        0     2018 2023-07-29 14:08:34.775025 codedog-0.5.1/codedog/models/change_file.py
+-rw-r--r--   0        0        0      192 2023-07-25 09:19:30.874838 codedog-0.5.1/codedog/models/change_summary.py
+-rw-r--r--   0        0        0      150 2023-07-29 14:08:34.775873 codedog-0.5.1/codedog/models/code_review.py
+-rw-r--r--   0        0        0      800 2023-07-25 09:19:34.757440 codedog-0.5.1/codedog/models/commit.py
+-rw-r--r--   0        0        0     1148 2023-07-25 09:19:34.758316 codedog-0.5.1/codedog/models/diff.py
+-rw-r--r--   0        0        0      824 2023-07-25 09:19:34.759325 codedog-0.5.1/codedog/models/issue.py
+-rw-r--r--   0        0        0      692 2023-07-29 14:08:34.776835 codedog-0.5.1/codedog/models/pr_summary.py
+-rw-r--r--   0        0        0     1703 2023-07-29 14:08:34.778019 codedog-0.5.1/codedog/models/pull_request.py
+-rw-r--r--   0        0        0      998 2023-07-25 09:19:34.760856 codedog-0.5.1/codedog/models/repository.py
+-rw-r--r--   0        0        0      111 2023-07-29 14:08:34.778655 codedog-0.5.1/codedog/processors/__init__.py
+-rw-r--r--   0        0        0     3835 2023-07-29 14:08:34.779662 codedog-0.5.1/codedog/processors/pull_request_processor.py
+-rw-r--r--   0        0        0      178 2023-07-25 09:19:30.876958 codedog-0.5.1/codedog/retrievers/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-25 09:19:30.877473 codedog-0.5.1/codedog/retrievers/base.py
+-rw-r--r--   0        0        0     8663 2023-07-29 14:08:34.780419 codedog-0.5.1/codedog/retrievers/github_retriever.py
+-rw-r--r--   0        0        0      126 2023-07-29 14:08:34.781526 codedog-0.5.1/codedog/retrievers/gitlab_retriever.py
+-rw-r--r--   0        0        0        0 2023-07-14 03:09:00.196876 codedog-0.5.1/codedog/templates/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-21 05:12:00.256318 codedog-0.5.1/codedog/templates/grimoire_cn.py
+-rw-r--r--   0        0        0     4542 2023-07-29 14:08:34.783652 codedog-0.5.1/codedog/templates/grimoire_en.py
+-rw-r--r--   0        0        0     1018 2023-07-21 05:12:00.257443 codedog-0.5.1/codedog/templates/template_cn.py
+-rw-r--r--   0        0        0     3387 2023-07-29 14:08:34.785033 codedog-0.5.1/codedog/templates/template_en.py
+-rw-r--r--   0        0        0        0 2023-08-02 11:24:29.516578 codedog-0.5.1/codedog/utils/__init__.py
+-rw-r--r--   0        0        0      486 2023-07-25 09:19:30.882119 codedog-0.5.1/codedog/utils/diff_utils.py
+-rw-r--r--   0        0        0      935 2023-07-29 14:08:34.791991 codedog-0.5.1/codedog/utils/langchain_utils.py
+-rw-r--r--   0        0        0      118 2023-08-02 12:15:57.996088 codedog-0.5.1/codedog/version.py
+-rw-r--r--   0        0        0     1780 2023-08-02 12:26:24.376828 codedog-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.1/PKG-INFO
```

### Comparing `codedog-0.5.0/LICENSE` & `codedog-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/README.md` & `codedog-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,25 +12,20 @@
 
 Codedog currently load config from environment variables.
 
 settings:
 
 | Config Name                   | Required | Default           | Description                             |
 | ----------------------------- | -------- | ----------------- | --------------------------------------- |
-| CODEDOG_SERVER                | No       | 0.0.0.0           | Server address                          |
-| CODEDOG_PORT                  | No       | 32167             | Server port                             |
-| CODEDOG_WORKER_NUM            | No       | 1                 | Server thread number                    |
-| OPENAI_API_KEY                | Yes      |                   | Api Key for calling openai gpt4 api     |
-| OPENAI_PROXY                  | No       |                   | Openai proxy                            |
+| OPENAI_API_KEY                | Yes      |                   | Api Key for calling openai gpt api      |
 | AZURE_OPENAI                  | No       |                   | Use azure openai gpt 3.5 if not blank   |
 | AZURE_OPENAI_API_KEY          | No       |                   | Azure openai api key                    |
 | AZURE_OPENAI_API_BASE         | No       |                   | Azure openai api base                   |
 | AZURE_OPENAI_DEPLOYMENT_ID    | No       |                   | Azure openai deployment id for gpt 3.5  |
 | AZURE_OPENAI_EMBEDDING_DEP_ID | No       |                   | Azure openai deployment id for embedding|
-| GITHUB_TOKEN                  | No       |                   | Retrieve github pr data and comment     |
 
 ## Usage
 
 ### Github Example with GPT4
 
 check `example/github_review.py`
```

### Comparing `codedog-0.5.0/codedog/actors/reporters/code_review.py` & `codedog-0.5.1/codedog/actors/reporters/code_review.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/actors/reporters/pr_summary.py` & `codedog-0.5.1/codedog/actors/reporters/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/actors/reporters/pull_request.py` & `codedog-0.5.1/codedog/actors/reporters/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/chains/code_review/base.py` & `codedog-0.5.1/codedog/chains/code_review/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def _call(self, inputs: Dict[str, Any], run_manager: Optional[CallbackManagerForChainRun] = None) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
         code_files: List[ChangeFile] = self.processor.get_diff_code_files(pr)
 
-        code_review_inputs = self._process_code_review_inputs(code_files, run_manager)
+        code_review_inputs = self._process_code_review_inputs(code_files, _run_manager)
         code_review_outputs = (
             self.chain.apply(code_review_inputs, callbacks=_run_manager.get_child(tag="CodeReview"))
             if code_review_inputs
             else []
         )
 
         return self._process_result(code_files, code_review_outputs)
@@ -69,15 +69,15 @@
     ) -> Dict[str, Any]:
         _run_manager = run_manager or AsyncCallbackManagerForChainRun.get_noop_manager()
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
         code_files: List[ChangeFile] = self.processor.get_diff_code_files(pr)
 
-        code_review_inputs = self._process_code_review_inputs(code_files, run_manager)
+        code_review_inputs = self._process_code_review_inputs(code_files, _run_manager)
         code_review_outputs = (
             self.chain.aapply(code_review_inputs, callbacks=_run_manager.get_child(tag="CodeReview"))
             if code_review_inputs
             else []
         )
 
         return self._process_result(code_files, code_review_outputs)
```

### Comparing `codedog-0.5.0/codedog/chains/pr_summary/base.py` & `codedog-0.5.1/codedog/chains/pr_summary/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def _call(self, inputs: Dict[str, Any], run_manager: Optional[CallbackManagerForChainRun] = None) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
 
-        code_summary_inputs = self._process_code_summary_inputs(pr, run_manager)
+        code_summary_inputs = self._process_code_summary_inputs(pr, _run_manager)
         code_summary_outputs = (
             self.code_summary_chain.apply(code_summary_inputs, callbacks=_run_manager.get_child(tag="CodeSummary"))
             if code_summary_inputs
             else []
         )
 
         code_summaries = self.processor.build_change_summaries(code_summary_inputs, code_summary_outputs)
@@ -100,32 +100,30 @@
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
 
-        code_summary_inputs = self._process_code_summary_inputs(pr)
+        code_summary_inputs = self._process_code_summary_inputs(pr, _run_manager)
         code_summary_outputs = (
             await self.code_summary_chain.aapply(code_summary_inputs, callbacks=_run_manager.get_child())
             if code_summary_inputs
             else []
         )
 
         code_summaries = self.processor.build_code_summaries(code_summary_inputs, code_summary_outputs)
 
         pr_summary_input = self._process_pr_summary_input(pr, code_summaries)
         pr_summary_output: PRSummary = await self.pr_summary_chain(pr_summary_input, callbacks=_run_manager.get_child())
 
         return self._process_result(pr_summary_output, code_summaries)
 
     def _process_code_summary_inputs(
-        self,
-        pr: PullRequest,
-        run_manager: Optional[CallbackManagerForChainRun] = None,
+        self, pr: PullRequest, run_manager: CallbackManagerForChainRun
     ) -> List[Dict[str, str]]:
         input_data = []
         code_files = self.processor.get_diff_code_files(pr)
         for code_file in code_files:
             input_item = {
                 "content": code_file.diff_content.content[:2000],  # TODO: handle long diff
                 "name": code_file.full_name,
```

### Comparing `codedog-0.5.0/codedog/chains/pr_summary/prompts.py` & `codedog-0.5.1/codedog/chains/pr_summary/prompts.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/localization.py` & `codedog-0.5.1/codedog/localization.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/__init__.py` & `codedog-0.5.1/codedog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/change_file.py` & `codedog-0.5.1/codedog/models/change_file.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/commit.py` & `codedog-0.5.1/codedog/models/commit.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/diff.py` & `codedog-0.5.1/codedog/models/diff.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/issue.py` & `codedog-0.5.1/codedog/models/issue.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/pr_summary.py` & `codedog-0.5.1/codedog/models/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/pull_request.py` & `codedog-0.5.1/codedog/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/models/repository.py` & `codedog-0.5.1/codedog/models/repository.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/processors/pull_request_processor.py` & `codedog-0.5.1/codedog/processors/pull_request_processor.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/retrievers/base.py` & `codedog-0.5.1/codedog/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/retrievers/github_retriever.py` & `codedog-0.5.1/codedog/retrievers/github_retriever.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/templates/grimoire_cn.py` & `codedog-0.5.1/codedog/templates/grimoire_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/templates/grimoire_en.py` & `codedog-0.5.1/codedog/templates/grimoire_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/templates/template_cn.py` & `codedog-0.5.1/codedog/templates/template_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/templates/template_en.py` & `codedog-0.5.1/codedog/templates/template_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/codedog/utils/langchain_utils.py` & `codedog-0.5.1/codedog/utils/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.0/pyproject.toml` & `codedog-0.5.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 [tool.poetry]
 name = "codedog"
-version = "0.5.0"
+version = "0.5.1"
 license = "MIT"
 readme = "README.md"
 authors = ["Arcadia <arcadia822@gmail.com>", "Linpp "]
 description = "Codedog reviews your pull request using llm."
 repository = "https://www.github.com/codedog-ai/codedog"
 homepage = "https://www.codedog.ai"
 keywords = ["code review", "langchain", "llm"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/codedog-ai/codedog/issues"
 "Discord" = "https://discord.gg/8TfqpFC4"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "~3.10"
 langchain = "^0.0.247"
 openai = "^0.27.8"
 pydantic = "^1.10.7"
 python-gitlab = "^3.14.0"
 pygithub = "^1.58.2"
 unidiff = "^0.7.5"
 
+
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
-pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
-python-semantic-release = "^7.34.6"
+python-semantic-release = "^8.0.4"
 langchain-visualizer = "^0.0.28"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
-python-dateutil = "^2.8.2"
 
 [tool.poetry.group.http]
 optional = true
 
 [tool.poetry.group.http.dependencies]
 fastapi = "^0.100.1"
 uvicorn = "^0.23.1"
 
 [tool.poetry.scripts]
-demoserver = "codedog.server:start"
+demoserver = "examples.server:start"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "default"
 
+[[tool.poetry.source]]
+name = "tsinghua"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
+priority = "supplemental"
+
 [tool.semantic_release]
-version_variable = ["./codedog/version.py:VERSION", "pyproject.toml:version"]
 branch = "master"
 build_command = "poetry build"
-upload_to_pypi = false
-upload_to_repository = false
-upload_to_release = true
-commit_message = 'chore(release): release version {version}'
+commit_message = 'chore(release): release version v{version}'
+version_variable = ["codedog/version.py:VERSION"]
+version_toml = ["pyproject.toml:tool.poetry.version"]
+
+[tool.semantic_release.remote]
+ignore_token_for_push = true
+
+[tool.semantic_release.publish]
+upload_to_vcs_release = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `codedog-0.5.0/PKG-INFO` & `codedog-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: codedog
-Version: 0.5.0
+Version: 0.5.1
 Summary: Codedog reviews your pull request using llm.
 Home-page: https://www.codedog.ai
 License: MIT
 Keywords: code review,langchain,llm
 Author: Arcadia
 Author-email: arcadia822@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: langchain (>=0.0.247,<0.0.248)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pygithub (>=1.58.2,<2.0.0)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Requires-Dist: unidiff (>=0.7.5,<0.8.0)
 Project-URL: Bug Tracker, https://github.com/codedog-ai/codedog/issues
@@ -37,25 +36,20 @@
 
 Codedog currently load config from environment variables.
 
 settings:
 
 | Config Name                   | Required | Default           | Description                             |
 | ----------------------------- | -------- | ----------------- | --------------------------------------- |
-| CODEDOG_SERVER                | No       | 0.0.0.0           | Server address                          |
-| CODEDOG_PORT                  | No       | 32167             | Server port                             |
-| CODEDOG_WORKER_NUM            | No       | 1                 | Server thread number                    |
-| OPENAI_API_KEY                | Yes      |                   | Api Key for calling openai gpt4 api     |
-| OPENAI_PROXY                  | No       |                   | Openai proxy                            |
+| OPENAI_API_KEY                | Yes      |                   | Api Key for calling openai gpt api      |
 | AZURE_OPENAI                  | No       |                   | Use azure openai gpt 3.5 if not blank   |
 | AZURE_OPENAI_API_KEY          | No       |                   | Azure openai api key                    |
 | AZURE_OPENAI_API_BASE         | No       |                   | Azure openai api base                   |
 | AZURE_OPENAI_DEPLOYMENT_ID    | No       |                   | Azure openai deployment id for gpt 3.5  |
 | AZURE_OPENAI_EMBEDDING_DEP_ID | No       |                   | Azure openai deployment id for embedding|
-| GITHUB_TOKEN                  | No       |                   | Retrieve github pr data and comment     |
 
 ## Usage
 
 ### Github Example with GPT4
 
 check `example/github_review.py`
```

