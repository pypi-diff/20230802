# Comparing `tmp/actions_security_analyzer-1.2.5.tar.gz` & `tmp/actions_security_analyzer-1.3.5.tar.gz`

## Comparing `actions_security_analyzer-1.2.5.tar` & `actions_security_analyzer-1.3.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/__about__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/colors.py
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/.github/workflows/asa-scan.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-that-creates-or-approves-pr.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/analyzer/__init__.py
--rw-r--r--   0        0        0    12497 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/analyzer/analyzer.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/images/asa-stdout.png
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/LICENSE
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/__about__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/colors.py
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/.github/workflows/asa-scan.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-that-creates-or-approves-pr.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/analyzer/__init__.py
+-rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/analyzer/analyzer.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/images/asa-stdout.png
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/LICENSE
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/PKG-INFO
```

### Comparing `actions_security_analyzer-1.2.5/action.yml` & `actions_security_analyzer-1.3.5/action.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/colors.py` & `actions_security_analyzer-1.3.5/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/main.py` & `actions_security_analyzer-1.3.5/main.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/.github/workflows/asa-scan.yml` & `actions_security_analyzer-1.3.5/.github/workflows/asa-scan.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.3.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/analyzer/analyzer.py` & `actions_security_analyzer-1.3.5/analyzer/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             "_check_for_dangerous_write_permissions": {"level": "FAIL"},
             "_check_for_inline_script": {"level": "WARN"},
             "_check_for_pull_request_target": {"level": "FAIL"},
             "_check_for_script_injection": {"level": "FAIL"},
             "_check_for_self_hosted_runners": {"level": "WARN"},
             "_check_for_aws_configure_credentials_non_oidc": {"level": "WARN"},
             "_check_for_pull_request_create_or_approve": {"level": "FAIL"},
+            "_check_for_remote_script": {"level": "WARN"},
         }
         self.action = {}
 
     def _print_failed_check_msg(self, check: str, level: str):
         c = None
         if level == "FAIL":
             c = Colors.RED
@@ -125,14 +126,31 @@
             if "pull_request_target" in event_triggers:
                 passed = False
         elif type(event_triggers) == str:
             if event_triggers == "pull_request_target":
                 passed = False
         return passed
 
+    def _check_for_remote_script(self) -> bool:
+        passed = True
+        POTENTIAL_REMOTE_SCRIPT = r"((?<=[^a-zA-Z0-9])(?:https?\:\/\/|[a-zA-Z0-9]{1,}\.{1}|\b)(?:\w{1,}\.{1}){1,5}(?:com|org|edu|gov|uk|net|ca|de|jp|fr|au|us|ru|ch|it|nl|se|no|es|mil|iq|io|ac|ly|sm){1}(?:\/[a-zA-Z0-9]{1,})*)"
+        for job in self.jobs.keys():
+            steps = self.jobs[job]["steps"]
+            for step in steps:
+                if "run" in step:
+                    script = step["run"]
+                    variable = search(POTENTIAL_REMOTE_SCRIPT, script)
+                    if variable:
+                        if self.verbose:
+                            print(
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} remote script ('{variable.group()}') being called"
+                            )
+                        passed = False
+        return passed
+
     def _check_for_cache_action_usage(self) -> bool:
         passed = True
         CACHE_ACTION_REGEX = r"actions\/cache@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "uses" in step:
```

### Comparing `actions_security_analyzer-1.2.5/analyzer/analyzer_test.py` & `actions_security_analyzer-1.3.5/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/images/asa-stdout.png` & `actions_security_analyzer-1.3.5/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/.gitignore` & `actions_security_analyzer-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/LICENSE` & `actions_security_analyzer-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/README.md` & `actions_security_analyzer-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/pyproject.toml` & `actions_security_analyzer-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.5/PKG-INFO` & `actions_security_analyzer-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.2.5
+Version: 1.3.5
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

