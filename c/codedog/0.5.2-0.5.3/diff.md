# Comparing `tmp/codedog-0.5.2.tar.gz` & `tmp/codedog-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedog-0.5.2.tar", max compression
+gzip compressed data, was "codedog-0.5.3.tar", max compression
```

## Comparing `codedog-0.5.2.tar` & `codedog-0.5.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1067 2023-07-29 15:15:38.422410 codedog-0.5.2/LICENSE
--rw-r--r--   0        0        0     1874 2023-07-31 08:08:49.444268 codedog-0.5.2/README.md
--rw-r--r--   0        0        0      328 2023-07-29 14:08:34.763306 codedog-0.5.2/codedog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.763486 codedog-0.5.2/codedog/actors/__init__.py
--rw-r--r--   0        0        0       22 2023-07-29 14:08:34.764323 codedog-0.5.2/codedog/actors/base.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.764498 codedog-0.5.2/codedog/actors/reporters/__init__.py
--rw-r--r--   0        0        0      198 2023-07-29 14:08:34.765314 codedog-0.5.2/codedog/actors/reporters/base.py
--rw-r--r--   0        0        0     1078 2023-07-29 14:08:34.766198 codedog-0.5.2/codedog/actors/reporters/code_review.py
--rw-r--r--   0        0        0     2793 2023-07-29 14:08:34.766867 codedog-0.5.2/codedog/actors/reporters/pr_summary.py
--rw-r--r--   0        0        0     2207 2023-07-29 14:08:34.767415 codedog-0.5.2/codedog/actors/reporters/pull_request.py
--rw-r--r--   0        0        0      167 2023-07-29 14:08:34.768840 codedog-0.5.2/codedog/chains/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 14:08:34.769200 codedog-0.5.2/codedog/chains/code_review/__init__.py
--rw-r--r--   0        0        0     4338 2023-08-02 12:41:46.001586 codedog-0.5.2/codedog/chains/code_review/base.py
--rw-r--r--   0        0        0      231 2023-07-29 14:08:34.771037 codedog-0.5.2/codedog/chains/code_review/prompts.py
--rw-r--r--   0        0        0        0 2023-07-25 09:19:30.869415 codedog-0.5.2/codedog/chains/pr_summary/__init__.py
--rw-r--r--   0        0        0     6524 2023-08-02 12:40:59.303816 codedog-0.5.2/codedog/chains/pr_summary/base.py
--rw-r--r--   0        0        0      579 2023-07-25 09:19:30.871812 codedog-0.5.2/codedog/chains/pr_summary/prompts.py
--rw-r--r--   0        0        0      714 2023-07-29 14:08:34.772749 codedog-0.5.2/codedog/localization.py
--rw-r--r--   0        0        0      738 2023-07-29 14:08:34.773960 codedog-0.5.2/codedog/models/__init__.py
--rw-r--r--   0        0        0      408 2023-07-25 09:19:30.873666 codedog-0.5.2/codedog/models/blob.py
--rw-r--r--   0        0        0     2018 2023-07-29 14:08:34.775025 codedog-0.5.2/codedog/models/change_file.py
--rw-r--r--   0        0        0      192 2023-07-25 09:19:30.874838 codedog-0.5.2/codedog/models/change_summary.py
--rw-r--r--   0        0        0      150 2023-07-29 14:08:34.775873 codedog-0.5.2/codedog/models/code_review.py
--rw-r--r--   0        0        0      800 2023-07-25 09:19:34.757440 codedog-0.5.2/codedog/models/commit.py
--rw-r--r--   0        0        0     1148 2023-07-25 09:19:34.758316 codedog-0.5.2/codedog/models/diff.py
--rw-r--r--   0        0        0      824 2023-07-25 09:19:34.759325 codedog-0.5.2/codedog/models/issue.py
--rw-r--r--   0        0        0      692 2023-07-29 14:08:34.776835 codedog-0.5.2/codedog/models/pr_summary.py
--rw-r--r--   0        0        0     1703 2023-07-29 14:08:34.778019 codedog-0.5.2/codedog/models/pull_request.py
--rw-r--r--   0        0        0      998 2023-07-25 09:19:34.760856 codedog-0.5.2/codedog/models/repository.py
--rw-r--r--   0        0        0      111 2023-07-29 14:08:34.778655 codedog-0.5.2/codedog/processors/__init__.py
--rw-r--r--   0        0        0     3835 2023-07-29 14:08:34.779662 codedog-0.5.2/codedog/processors/pull_request_processor.py
--rw-r--r--   0        0        0      178 2023-07-25 09:19:30.876958 codedog-0.5.2/codedog/retrievers/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-25 09:19:30.877473 codedog-0.5.2/codedog/retrievers/base.py
--rw-r--r--   0        0        0     8663 2023-07-29 14:08:34.780419 codedog-0.5.2/codedog/retrievers/github_retriever.py
--rw-r--r--   0        0        0      126 2023-07-29 14:08:34.781526 codedog-0.5.2/codedog/retrievers/gitlab_retriever.py
--rw-r--r--   0        0        0        0 2023-07-14 03:09:00.196876 codedog-0.5.2/codedog/templates/__init__.py
--rw-r--r--   0        0        0     2910 2023-07-21 05:12:00.256318 codedog-0.5.2/codedog/templates/grimoire_cn.py
--rw-r--r--   0        0        0     4542 2023-07-29 14:08:34.783652 codedog-0.5.2/codedog/templates/grimoire_en.py
--rw-r--r--   0        0        0     1018 2023-07-21 05:12:00.257443 codedog-0.5.2/codedog/templates/template_cn.py
--rw-r--r--   0        0        0     3387 2023-07-29 14:08:34.785033 codedog-0.5.2/codedog/templates/template_en.py
--rw-r--r--   0        0        0        0 2023-08-02 11:24:29.516578 codedog-0.5.2/codedog/utils/__init__.py
--rw-r--r--   0        0        0      486 2023-07-25 09:19:30.882119 codedog-0.5.2/codedog/utils/diff_utils.py
--rw-r--r--   0        0        0      935 2023-07-29 14:08:34.791991 codedog-0.5.2/codedog/utils/langchain_utils.py
--rw-r--r--   0        0        0      118 2023-08-02 12:15:57.996088 codedog-0.5.2/codedog/version.py
--rw-r--r--   0        0        0     1781 2023-08-02 12:42:59.142319 codedog-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      328 2023-07-30 08:13:27.833259 codedog-0.5.3/codedog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/base.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/reporters/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/reporters/base.py
+-rw-r--r--   0        0        0     1078 2023-07-30 08:13:27.835260 codedog-0.5.3/codedog/actors/reporters/code_review.py
+-rw-r--r--   0        0        0     2842 2023-08-02 14:31:22.564488 codedog-0.5.3/codedog/actors/reporters/pr_summary.py
+-rw-r--r--   0        0        0     2207 2023-07-30 08:13:27.835260 codedog-0.5.3/codedog/actors/reporters/pull_request.py
+-rw-r--r--   0        0        0      167 2023-07-30 08:13:27.835260 codedog-0.5.3/codedog/chains/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:13:27.854264 codedog-0.5.3/codedog/chains/code_review/__init__.py
+-rw-r--r--   0        0        0     4143 2023-08-02 14:30:41.484288 codedog-0.5.3/codedog/chains/code_review/base.py
+-rw-r--r--   0        0        0      231 2023-07-30 08:13:27.854264 codedog-0.5.3/codedog/chains/code_review/prompts.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:00:53.472920 codedog-0.5.3/codedog/chains/pr_summary/__init__.py
+-rw-r--r--   0        0        0     6358 2023-08-02 14:30:41.484288 codedog-0.5.3/codedog/chains/pr_summary/base.py
+-rw-r--r--   0        0        0      579 2023-07-25 13:00:53.474921 codedog-0.5.3/codedog/chains/pr_summary/prompts.py
+-rw-r--r--   0        0        0      714 2023-07-30 08:13:27.979292 codedog-0.5.3/codedog/localization.py
+-rw-r--r--   0        0        0      738 2023-07-30 08:13:28.073313 codedog-0.5.3/codedog/models/__init__.py
+-rw-r--r--   0        0        0      408 2023-07-25 13:00:53.493925 codedog-0.5.3/codedog/models/blob.py
+-rw-r--r--   0        0        0     2018 2023-07-30 08:13:28.073313 codedog-0.5.3/codedog/models/change_file.py
+-rw-r--r--   0        0        0      192 2023-07-25 13:00:53.493925 codedog-0.5.3/codedog/models/change_summary.py
+-rw-r--r--   0        0        0      150 2023-07-30 08:13:28.106320 codedog-0.5.3/codedog/models/code_review.py
+-rw-r--r--   0        0        0      800 2023-07-25 13:00:53.494925 codedog-0.5.3/codedog/models/commit.py
+-rw-r--r--   0        0        0     1148 2023-07-25 13:00:53.494925 codedog-0.5.3/codedog/models/diff.py
+-rw-r--r--   0        0        0      824 2023-07-25 13:00:53.494925 codedog-0.5.3/codedog/models/issue.py
+-rw-r--r--   0        0        0      692 2023-07-30 08:13:28.106320 codedog-0.5.3/codedog/models/pr_summary.py
+-rw-r--r--   0        0        0     1703 2023-07-30 08:13:28.107321 codedog-0.5.3/codedog/models/pull_request.py
+-rw-r--r--   0        0        0      998 2023-07-25 13:00:53.495925 codedog-0.5.3/codedog/models/repository.py
+-rw-r--r--   0        0        0      111 2023-07-30 08:13:28.123920 codedog-0.5.3/codedog/processors/__init__.py
+-rw-r--r--   0        0        0     3835 2023-07-30 08:13:28.123920 codedog-0.5.3/codedog/processors/pull_request_processor.py
+-rw-r--r--   0        0        0      178 2023-07-25 13:00:53.496925 codedog-0.5.3/codedog/retrievers/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-25 13:00:53.496925 codedog-0.5.3/codedog/retrievers/base.py
+-rw-r--r--   0        0        0     8661 2023-08-02 14:30:41.485287 codedog-0.5.3/codedog/retrievers/github_retriever.py
+-rw-r--r--   0        0        0      126 2023-07-30 08:13:28.124920 codedog-0.5.3/codedog/retrievers/gitlab_retriever.py
+-rw-r--r--   0        0        0        0 2023-07-15 01:59:22.106348 codedog-0.5.3/codedog/templates/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-22 00:54:46.880133 codedog-0.5.3/codedog/templates/grimoire_cn.py
+-rw-r--r--   0        0        0     4542 2023-07-30 08:13:28.167198 codedog-0.5.3/codedog/templates/grimoire_en.py
+-rw-r--r--   0        0        0     1018 2023-07-22 00:54:46.914141 codedog-0.5.3/codedog/templates/template_cn.py
+-rw-r--r--   0        0        0     3387 2023-07-30 08:13:28.228587 codedog-0.5.3/codedog/templates/template_en.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:57:13.330242 codedog-0.5.3/codedog/utils/__init__.py
+-rw-r--r--   0        0        0      486 2023-07-25 13:00:53.522488 codedog-0.5.3/codedog/utils/diff_utils.py
+-rw-r--r--   0        0        0      935 2023-07-30 08:13:28.243590 codedog-0.5.3/codedog/utils/langchain_utils.py
+-rw-r--r--   0        0        0      118 2023-07-30 08:13:28.244591 codedog-0.5.3/codedog/version.py
+-rw-r--r--   0        0        0     1067 2023-07-30 08:13:27.833259 codedog-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1857 2023-08-02 14:37:21.412244 codedog-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1874 2023-07-30 11:18:08.325034 codedog-0.5.3/README.md
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.3/PKG-INFO
```

### Comparing `codedog-0.5.2/LICENSE` & `codedog-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/README.md` & `codedog-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/actors/reporters/code_review.py` & `codedog-0.5.3/codedog/actors/reporters/code_review.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/actors/reporters/pr_summary.py` & `codedog-0.5.3/codedog/actors/reporters/pr_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,33 +38,34 @@
             overview=self._pr_summary.overview,
         )
 
     def _generate_change_overivew(self) -> str:
         return self.pr_processor.gen_material_change_files(self._pull_request.change_files)
 
     def _generate_file_changes(self) -> str:
-        major_changes_report = []
-        changes_report = []
+        major_changes = []
+        secondary_changes = []
 
         major_files = set(self._pr_summary.major_files)
         self._pull_request.change_files
         for change_file in self._pull_request.change_files:
             if change_file.full_name not in self._code_summaries:
                 continue
 
             curr_report = self.template.REPORT_CHANGE_OVERVIEW.format(
                 name=change_file.name,
                 url=change_file.diff_url,
                 full_name=change_file.full_name,
                 content=self._code_summaries[change_file.full_name].summary,
             )
 
-            major_changes_report.append(curr_report) if change_file.full_name in major_files else changes_report.append(
-                curr_report
-            )
+            _target_changes = major_changes if change_file.full_name in major_files else secondary_changes
+            _target_changes.append(curr_report)
 
-        report_major = self.template.REPORT_FILE_CHANGES_MAJOR.format(
-            major_changes="\n".join(major_changes_report) if major_changes_report else "",
+        major_change_report = self.template.REPORT_FILE_CHANGES_MAJOR.format(
+            major_changes="\n".join(major_changes) if major_changes else ""
+        )
+        secondary_change_report = self.template.REPORT_FILE_CHANGES.format(
+            changes="\n".join(secondary_changes) if secondary_changes else ""
         )
-        report = self.template.REPORT_FILE_CHANGES.format(changes="\n".join(changes_report) if changes_report else "")
 
-        return f"{report_major}\n{report}\n"
+        return f"{major_change_report}\n{secondary_change_report}\n"
```

### Comparing `codedog-0.5.2/codedog/actors/reporters/pull_request.py` & `codedog-0.5.3/codedog/actors/reporters/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/chains/code_review/base.py` & `codedog-0.5.3/codedog/chains/code_review/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,58 +49,56 @@
     def _call(self, inputs: Dict[str, Any], run_manager: Optional[CallbackManagerForChainRun] = None) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
         code_files: List[ChangeFile] = self.processor.get_diff_code_files(pr)
 
-        code_review_inputs = self._process_code_review_inputs(code_files, _run_manager)
+        code_review_inputs = self._process_code_review_inputs(code_files)
         code_review_outputs = (
             self.chain.apply(code_review_inputs, callbacks=_run_manager.get_child(tag="CodeReview"))
             if code_review_inputs
             else []
         )
 
         return self._process_result(code_files, code_review_outputs)
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
         _run_manager = run_manager or AsyncCallbackManagerForChainRun.get_noop_manager()
-        _run_manager.on_text(inputs["pull_request"].json() + "\n")
+        await _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
         code_files: List[ChangeFile] = self.processor.get_diff_code_files(pr)
 
-        code_review_inputs = self._process_code_review_inputs(code_files, _run_manager)
+        code_review_inputs = self._process_code_review_inputs(code_files)
         code_review_outputs = (
             await self.chain.aapply(code_review_inputs, callbacks=_run_manager.get_child(tag="CodeReview"))
             if code_review_inputs
             else []
         )
 
         return self._process_result(code_files, code_review_outputs)
 
     def _process_code_review_inputs(
         self,
         code_files: List[ChangeFile],
-        run_manager: CallbackManagerForChainRun or AsyncCallbackManagerForChainRun,
     ) -> List[Dict[str, str]]:
         input_data = []
         for code_file in code_files:
             input_item = {
                 "content": code_file.diff_content.content[:4000],  # TODO: handle long diff with summarize chain
                 "name": code_file.full_name,
                 "language": SUFFIX_LANGUAGE_MAPPING.get(code_file.suffix, ""),
             }
             input_data.append(input_item)
 
-        run_manager.on_text(f"Prepare code diff content for {len(input_data)} files.\n")
         return input_data
 
     def _process_result(self, code_files: List[ChangeFile], code_review_outputs: List):
         code_reviews = []
         for i, o in zip_longest(code_files, code_review_outputs):
             code_reviews.append(CodeReview(file=i, review=o["text"]))
         return {"code_reviews": code_reviews}
```

### Comparing `codedog-0.5.2/codedog/chains/pr_summary/base.py` & `codedog-0.5.3/codedog/chains/pr_summary/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def _call(self, inputs: Dict[str, Any], run_manager: Optional[CallbackManagerForChainRun] = None) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
         _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
 
-        code_summary_inputs = self._process_code_summary_inputs(pr, _run_manager)
+        code_summary_inputs = self._process_code_summary_inputs(pr)
         code_summary_outputs = (
             self.code_summary_chain.apply(code_summary_inputs, callbacks=_run_manager.get_child(tag="CodeSummary"))
             if code_summary_inputs
             else []
         )
 
         code_summaries = self.processor.build_change_summaries(code_summary_inputs, code_summary_outputs)
@@ -96,46 +96,43 @@
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
-        _run_manager.on_text(inputs["pull_request"].json() + "\n")
+        await _run_manager.on_text(inputs["pull_request"].json() + "\n")
 
         pr: PullRequest = inputs["pull_request"]
 
-        code_summary_inputs = self._process_code_summary_inputs(pr, _run_manager)
+        code_summary_inputs = self._process_code_summary_inputs(pr)
         code_summary_outputs = (
             await self.code_summary_chain.aapply(code_summary_inputs, callbacks=_run_manager.get_child())
             if code_summary_inputs
             else []
         )
 
         code_summaries = self.processor.build_code_summaries(code_summary_inputs, code_summary_outputs)
 
         pr_summary_input = self._process_pr_summary_input(pr, code_summaries)
         pr_summary_output: PRSummary = await self.pr_summary_chain(pr_summary_input, callbacks=_run_manager.get_child())
 
         return self._process_result(pr_summary_output, code_summaries)
 
-    def _process_code_summary_inputs(
-        self, pr: PullRequest, run_manager: CallbackManagerForChainRun
-    ) -> List[Dict[str, str]]:
+    def _process_code_summary_inputs(self, pr: PullRequest) -> List[Dict[str, str]]:
         input_data = []
         code_files = self.processor.get_diff_code_files(pr)
         for code_file in code_files:
             input_item = {
                 "content": code_file.diff_content.content[:2000],  # TODO: handle long diff
                 "name": code_file.full_name,
                 "language": SUFFIX_LANGUAGE_MAPPING.get(code_file.suffix, ""),
             }
             input_data.append(input_item)
 
-        run_manager.on_text(f"Prepare code diff content for {len(input_data)} files.\n")
         return input_data
 
     def _process_pr_summary_input(self, pr: PullRequest, code_summaries: List[ChangeSummary]) -> Dict[str, str]:
         change_files_material: str = self.processor.gen_material_change_files(pr.change_files)
         code_summaries_material = self.processor.gen_material_code_summaries(code_summaries)
         pr_metadata_material = self.processor.gen_material_pr_metadata(pr)
         return {
```

### Comparing `codedog-0.5.2/codedog/chains/pr_summary/prompts.py` & `codedog-0.5.3/codedog/chains/pr_summary/prompts.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/localization.py` & `codedog-0.5.3/codedog/localization.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/__init__.py` & `codedog-0.5.3/codedog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/change_file.py` & `codedog-0.5.3/codedog/models/change_file.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/commit.py` & `codedog-0.5.3/codedog/models/commit.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/diff.py` & `codedog-0.5.3/codedog/models/diff.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/issue.py` & `codedog-0.5.3/codedog/models/issue.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/pr_summary.py` & `codedog-0.5.3/codedog/models/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/pull_request.py` & `codedog-0.5.3/codedog/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/models/repository.py` & `codedog-0.5.3/codedog/models/repository.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/processors/pull_request_processor.py` & `codedog-0.5.3/codedog/processors/pull_request_processor.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/retrievers/base.py` & `codedog-0.5.3/codedog/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/retrievers/github_retriever.py` & `codedog-0.5.3/codedog/retrievers/github_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,22 +40,22 @@
     }
 
     ISSUE_PATTERN = r"#\d+"
 
     def __init__(
         self,
         client: Github,
-        repository_name_or_id: str or int,
+        repository_name_or_id: str | int,
         pull_request_number: int,
     ):
         """Connect to github remote server and retrieve pull request data.
 
         Args:
             client (github.Github): github client from pyGithub
-            repository_name_or_id (str or int): repository name or id
+            repository_name_or_id (str | int): repository name or id
             pull_request_number (int): pull request number (not global id)
         """
 
         # --- github model ---
         self._git_repository: GHRepo = client.get_repo(repository_name_or_id)
         self._git_pull_request: GHPullRequest = self._git_repository.get_pull(pull_request_number)
```

### Comparing `codedog-0.5.2/codedog/templates/grimoire_cn.py` & `codedog-0.5.3/codedog/templates/grimoire_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/templates/grimoire_en.py` & `codedog-0.5.3/codedog/templates/grimoire_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/templates/template_cn.py` & `codedog-0.5.3/codedog/templates/template_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/templates/template_en.py` & `codedog-0.5.3/codedog/templates/template_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/codedog/utils/langchain_utils.py` & `codedog-0.5.3/codedog/utils/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.2/pyproject.toml` & `codedog-0.5.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-[tool.poetry]
-name = "codedog"
-version = "0.5.2"
-license = "MIT"
-readme = "README.md"
-authors = ["Arcadia <arcadia822@gmail.com>", "Linpp "]
-description = "Codedog reviews your pull request using llm."
-repository = "https://www.github.com/codedog-ai/codedog"
-homepage = "https://www.codedog.ai"
-keywords = ["code review", "langchain", "llm"]
-
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/codedog-ai/codedog/issues"
-"Discord" = "https://discord.gg/8TfqpFC4"
-
-[tool.poetry.dependencies]
-python = "~3.10"
-langchain = "^0.0.247"
-openai = "^0.27.8"
-pydantic = "^1.10.7"
-python-gitlab = "^3.14.0"
-pygithub = "^1.58.2"
-unidiff = "^0.7.5"
-
-
-[tool.poetry.group.dev]
-optional = true
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-flake8 = "^6.0.0"
-isort = "^5.12.0"
-python-semantic-release = "^8.0.4"
-langchain-visualizer = "^0.0.28"
-
-[tool.poetry.group.test]
-optional = true
-
-[tool.poetry.group.test.dependencies]
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
-
-[tool.poetry.group.http]
-optional = true
-
-[tool.poetry.group.http.dependencies]
-fastapi = "^0.100.1"
-uvicorn = "^0.23.1"
-
-[tool.poetry.scripts]
-demoserver = "examples.server:start"
-
-[[tool.poetry.source]]
-name = "PyPI"
-priority = "default"
-
-[[tool.poetry.source]]
-name = "tsinghua"
-url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
-priority = "supplemental"
-
-[tool.semantic_release]
-branch = "master"
-build_command = "poetry build"
-commit_message = 'chore(release): release version v{version}'
-version_variable = ["codedog/version.py:VERSION"]
-version_toml = ["pyproject.toml:tool.poetry.version"]
-
-[tool.semantic_release.remote]
-ignore_token_for_push = true
-
-[tool.semantic_release.publish]
-upload_to_vcs_release = false
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "codedog"
+version = "0.5.3"
+license = "MIT"
+readme = "README.md"
+authors = ["Arcadia <arcadia822@gmail.com>", "Linpp "]
+description = "Codedog reviews your pull request using llm."
+repository = "https://www.github.com/codedog-ai/codedog"
+homepage = "https://www.codedog.ai"
+keywords = ["code review", "langchain", "llm"]
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/codedog-ai/codedog/issues"
+"Discord" = "https://discord.gg/8TfqpFC4"
+
+[tool.poetry.dependencies]
+python = "~3.10"
+langchain = "^0.0.247"
+openai = "^0.27.8"
+pydantic = "^1.10.7"
+python-gitlab = "^3.14.0"
+pygithub = "^1.58.2"
+unidiff = "^0.7.5"
+
+
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+flake8 = "^6.0.0"
+isort = "^5.12.0"
+python-semantic-release = "^8.0.4"
+langchain-visualizer = "^0.0.28"
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest-asyncio = "^0.20.3"
+pytest-cov = "^4.0.0"
+
+[tool.poetry.group.http]
+optional = true
+
+[tool.poetry.group.http.dependencies]
+fastapi = "^0.100.1"
+uvicorn = "^0.23.1"
+
+[tool.poetry.scripts]
+demoserver = "examples.server:start"
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "default"
+
+[[tool.poetry.source]]
+name = "tsinghua"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
+priority = "supplemental"
+
+[tool.semantic_release]
+branch = "master"
+build_command = "poetry build"
+commit_message = 'chore(release): release version v{version}'
+version_variable = ["codedog/version.py:VERSION"]
+version_toml = ["pyproject.toml:tool.poetry.version"]
+
+[tool.semantic_release.remote]
+ignore_token_for_push = true
+
+[tool.semantic_release.publish]
+upload_to_vcs_release = true
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `codedog-0.5.2/PKG-INFO` & `codedog-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedog
-Version: 0.5.2
+Version: 0.5.3
 Summary: Codedog reviews your pull request using llm.
 Home-page: https://www.codedog.ai
 License: MIT
 Keywords: code review,langchain,llm
 Author: Arcadia
 Author-email: arcadia822@gmail.com
 Requires-Python: >=3.10,<3.11
```

