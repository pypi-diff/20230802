# Comparing `tmp/cdk_organizer-1.5.0.tar.gz` & `tmp/cdk_organizer-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_organizer-1.5.0.tar", max compression
+gzip compressed data, was "cdk_organizer-1.6.0b1.tar", max compression
```

## Comparing `cdk_organizer-1.5.0.tar` & `cdk_organizer-1.6.0b1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     6748 2022-10-05 17:16:36.644081 cdk_organizer-1.5.0/README.md
--rw-r--r--   0        0        0      194 2022-09-09 12:39:05.760295 cdk_organizer-1.5.0/cdk_organizer/__init__.py
--rw-r--r--   0        0        0       22 2022-09-09 12:39:05.762815 cdk_organizer-1.5.0/cdk_organizer/aws/__init__.py
--rw-r--r--   0        0        0     1168 2022-09-09 12:39:05.764895 cdk_organizer-1.5.0/cdk_organizer/aws/stack.py
--rw-r--r--   0        0        0      509 2022-09-09 12:39:05.766124 cdk_organizer-1.5.0/cdk_organizer/aws/stack_group.py
--rw-r--r--   0        0        0       27 2022-09-09 12:39:05.766813 cdk_organizer-1.5.0/cdk_organizer/decorators/__init__.py
--rw-r--r--   0        0        0     1129 2022-09-09 12:39:05.768384 cdk_organizer-1.5.0/cdk_organizer/decorators/catch_exceptions.py
--rw-r--r--   0        0        0       22 2022-09-09 12:39:05.769040 cdk_organizer-1.5.0/cdk_organizer/loaders/__init__.py
--rw-r--r--   0        0        0     4058 2022-09-09 12:39:05.770652 cdk_organizer-1.5.0/cdk_organizer/loaders/config_loader.py
--rw-r--r--   0        0        0       28 2022-09-09 12:39:05.771365 cdk_organizer-1.5.0/cdk_organizer/miscellaneous/__init__.py
--rw-r--r--   0        0        0     1652 2022-09-09 12:39:05.772921 cdk_organizer-1.5.0/cdk_organizer/miscellaneous/logging.py
--rw-r--r--   0        0        0       31 2022-09-09 12:39:05.774140 cdk_organizer-1.5.0/cdk_organizer/miscellaneous/yaml_tags/__init__.py
--rw-r--r--   0        0        0     1111 2022-09-09 12:39:05.777863 cdk_organizer-1.5.0/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py
--rw-r--r--   0        0        0     4834 2022-09-09 12:39:05.778749 cdk_organizer-1.5.0/cdk_organizer/stack.py
--rw-r--r--   0        0        0    12127 2023-06-02 22:04:03.712277 cdk_organizer-1.5.0/cdk_organizer/stack_group.py
--rw-r--r--   0        0        0       28 2022-09-09 12:39:05.780694 cdk_organizer-1.5.0/cdk_organizer/terraform/__init__.py
--rw-r--r--   0        0        0     1388 2022-09-13 21:00:59.686116 cdk_organizer-1.5.0/cdk_organizer/terraform/stack.py
--rw-r--r--   0        0        0      519 2022-09-09 12:39:05.784357 cdk_organizer-1.5.0/cdk_organizer/terraform/stack_group.py
--rw-r--r--   0        0        0     1092 2023-06-02 22:07:27.975898 cdk_organizer-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8053 1970-01-01 00:00:00.000000 cdk_organizer-1.5.0/setup.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 cdk_organizer-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     6748 2022-10-05 17:16:36.644081 cdk_organizer-1.6.0b1/README.md
+-rw-r--r--   0        0        0      194 2022-09-09 12:39:05.760295 cdk_organizer-1.6.0b1/cdk_organizer/__init__.py
+-rw-r--r--   0        0        0       22 2022-09-09 12:39:05.762815 cdk_organizer-1.6.0b1/cdk_organizer/aws/__init__.py
+-rw-r--r--   0        0        0     1168 2022-09-09 12:39:05.764895 cdk_organizer-1.6.0b1/cdk_organizer/aws/stack.py
+-rw-r--r--   0        0        0      509 2022-09-09 12:39:05.766124 cdk_organizer-1.6.0b1/cdk_organizer/aws/stack_group.py
+-rw-r--r--   0        0        0       27 2022-09-09 12:39:05.766813 cdk_organizer-1.6.0b1/cdk_organizer/decorators/__init__.py
+-rw-r--r--   0        0        0     1129 2022-09-09 12:39:05.768384 cdk_organizer-1.6.0b1/cdk_organizer/decorators/catch_exceptions.py
+-rw-r--r--   0        0        0       22 2022-09-09 12:39:05.769040 cdk_organizer-1.6.0b1/cdk_organizer/loaders/__init__.py
+-rw-r--r--   0        0        0     4058 2022-09-09 12:39:05.770652 cdk_organizer-1.6.0b1/cdk_organizer/loaders/config_loader.py
+-rw-r--r--   0        0        0       28 2022-09-09 12:39:05.771365 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/__init__.py
+-rw-r--r--   0        0        0     1652 2022-09-09 12:39:05.772921 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/logging.py
+-rw-r--r--   0        0        0       31 2022-09-09 12:39:05.774140 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/yaml_tags/__init__.py
+-rw-r--r--   0        0        0     1111 2022-09-09 12:39:05.777863 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py
+-rw-r--r--   0        0        0     4834 2022-09-09 12:39:05.778749 cdk_organizer-1.6.0b1/cdk_organizer/stack.py
+-rw-r--r--   0        0        0    12127 2023-06-02 22:04:03.712277 cdk_organizer-1.6.0b1/cdk_organizer/stack_group.py
+-rw-r--r--   0        0        0       28 2022-09-09 12:39:05.780694 cdk_organizer-1.6.0b1/cdk_organizer/terraform/__init__.py
+-rw-r--r--   0        0        0     1388 2022-09-13 21:00:59.686116 cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack.py
+-rw-r--r--   0        0        0      519 2022-09-09 12:39:05.784357 cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack_group.py
+-rw-r--r--   0        0        0     1095 2023-08-02 14:12:24.540866 cdk_organizer-1.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0     7482 1970-01-01 00:00:00.000000 cdk_organizer-1.6.0b1/PKG-INFO
```

### Comparing `cdk_organizer-1.5.0/README.md` & `cdk_organizer-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/aws/stack.py` & `cdk_organizer-1.6.0b1/cdk_organizer/aws/stack.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/decorators/catch_exceptions.py` & `cdk_organizer-1.6.0b1/cdk_organizer/decorators/catch_exceptions.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/loaders/config_loader.py` & `cdk_organizer-1.6.0b1/cdk_organizer/loaders/config_loader.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/miscellaneous/logging.py` & `cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py` & `cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/stack.py` & `cdk_organizer-1.6.0b1/cdk_organizer/stack.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/stack_group.py` & `cdk_organizer-1.6.0b1/cdk_organizer/stack_group.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/terraform/stack.py` & `cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/cdk_organizer/terraform/stack_group.py` & `cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack_group.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.5.0/pyproject.toml` & `cdk_organizer-1.6.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 show_missing = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-fail-under=100 --cov-report html:'../../coverage/packages/framework-python/html' --cov-report xml:'../../coverage/packages/framework-python/coverage.xml' --junitxml='../../reports/packages/framework-python/unittests/junit.xml' --html='../../reports/packages/framework-python/unittests/html/index.html'"
 
 [tool.poetry]
 name = "cdk-organizer"
-version = "1.5.0"
+version = "1.6.0b1"
 description = "CDK Organizer"
 authors = [ ]
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "cdk_organizer"
 
   [tool.poetry.dependencies]
-  python = ">=3.7,<3.10"
+  python = ">=3.7,<=3.10"
   PyYAML = "^6.0"
   dacite = "^1.6.0"
   pyhumps = "^3.7.2"
   constructs = "^10.1.49"
   cdktf = { version = "^0.15.0", optional = true }
   "aws-cdk-lib" = { version = "^2.32.1", optional = true }
```

### Comparing `cdk_organizer-1.5.0/setup.py` & `cdk_organizer-1.6.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,334 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cdk-organizer
+Version: 1.6.0b1
+Summary: CDK Organizer
+Requires-Python: >=3.7,<=3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: aws
+Provides-Extra: terraform
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: aws-cdk-lib (>=2.32.1,<3.0.0) ; extra == "aws"
+Requires-Dist: cdktf (>=0.15.0,<0.16.0) ; extra == "terraform"
+Requires-Dist: constructs (>=10.1.49,<11.0.0)
+Requires-Dist: dacite (>=1.6.0,<2.0.0)
+Requires-Dist: pyhumps (>=3.7.2,<4.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['cdk_organizer',
- 'cdk_organizer.aws',
- 'cdk_organizer.decorators',
- 'cdk_organizer.loaders',
- 'cdk_organizer.miscellaneous',
- 'cdk_organizer.miscellaneous.yaml_tags',
- 'cdk_organizer.terraform']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'constructs>=10.1.49,<11.0.0',
- 'dacite>=1.6.0,<2.0.0',
- 'pyhumps>=3.7.2,<4.0.0']
-
-extras_require = \
-{'aws': ['aws-cdk-lib>=2.32.1,<3.0.0'], 'terraform': ['cdktf>=0.15.0,<0.16.0']}
-
-setup_kwargs = {
-    'name': 'cdk-organizer',
-    'version': '1.5.0',
-    'description': 'CDK Organizer',
-    'long_description': '# CDK Organizer Python Library\n\nThis library contains the core features to handle CDK projects including:\n\n- Logging\n- Configuration Resolver\n- Stack Groups Loader\n- Naming Utils\n\nFull documentation: <https://cdk-organizer.github.io/>\n\n## Installation\n\n```bash\npip install cdk-organizer[terraform,aws]\n```\n\n### Extras\n\n- `terraform`: Include `cdktf` as a dependency.\n- `aws`: Include `aws-cdk-lib` as a dependency.\n\n### CDK Start Script\n\nThe content of the `app.py` file should be as follows:\n\n#### AWS CDK\n\n```python\nimport aws_cdk as cdk\nfrom cdk_organizer.miscellaneous.logging import setup_logging\nfrom cdk_organizer.stack_group import StackGroupLoader\n\napp = cdk.App()\nlogger = setup_logging(__name__, app.node.try_get_context("loglevel") or "INFO")\nloader = StackGroupLoader(app)\n\nloader.synth()\napp.synth()\n```\n\n#### CDK for Terraform\n\n```python\nfrom cdk_organizer.miscellaneous.logging import setup_logging\nfrom cdk_organizer.stack_group import StackGroupLoader\nfrom cdktf import App\n\napp = App()\nlogger = setup_logging(__name__, app.node.try_get_context("loglevel") or "INFO")\nloader = StackGroupLoader(app)\n\nloader.synth()\napp.synth()\n```\n\n## Context Variables\n\nThe following context variables are required to the CDK Organizer to work properly:\n\n- `env`\n- `region`\n\nThe variables can be set in the `cdk.json` file:\n\n```json\n{\n  ...\n  "context": {\n    ...\n    "env": "dev",\n    "region": "us-east-1"\n    ...\n  }\n  ...\n}\n```\n\nOr passed as arguments to the CDK CLI:\n\n```bash\ncdk synth --context env=dev --context region=us-east-1\n```\n\n> In the `cdktf` CLI the context variables cannot be passed as arguments, so they need to be set in the `cdk.json` file. <https://github.com/hashicorp/terraform-cdk/issues/2019>\n> The `env` variable can also be set as an environment variable `CDK_ENV`.\n\n## Project Structure\n\nTo apply the pattern purposed in this library for CDK projects, the following structure is required:\n\n```text\n.\n+-- cdk.json\n+-- app.py\n```\n\n### Stack Structure\n\nthe stack class needs to inherit from class `cdk_organizer.aws.stack.Stack` for AWS CDK and `cdk_organizer.terraform.stack.Stack` for Terraform CDK.\n\n#### AWS CDK\n\n```python\nfrom constructs import Construct\nfrom cdk_organizer.aws.stack import Stack\nfrom cdk_organizer.aws.stack_group import StackGroup\n\n\nclass MyStack(Stack):\n    def __init__(\n        self,\n        scope: Construct,\n        id: str,\n        stack_group: StackGroup,\n        **kwargs\n    ) -> None:\n        super().__init__(scope, id, stack_group, **kwargs)\n```\n\n#### Terraform CDK\n\n```python\nfrom constructs import Construct\nfrom cdk_organizer.terraform.stack import Stack\nfrom cdk_organizer.terraform.stack_group import StackGroup\n\n\nclass MyStack(Stack):\n    def __init__(\n        self,\n        scope: Construct,\n        id: str,\n        stack_group: StackGroup,\n        **kwargs\n    ) -> None:\n        super().__init__(scope, id, stack_group, **kwargs)\n```\n\n#### Using S3 Backend\n\nTo use S3 terraform backend, the following resources are required:\n\n- S3 Bucket\n- DynamoDB Table\n\nAdd the following object to the environment configuration file:\n\n```yaml\ns3_backend:\n  bucket: "<bucket-name>"\n  region: "<aws-region>"\n  dynamodb_table: "<dynamodb-table-name>"\n```\n\n### Stack Group Structure\n\nCreate a `stacks` folder in the root of the project and structure it as follows:\n\n```text\n.\n+-- cdk.json\n+-- app.py\n+-- stacks/\n| +-- <groupName>/\n|   +-- stacks.py\n```\n\nThe stack groups files follow this pattern:\n\n#### AWS CDK\n\n```python\nimport aws_cdk as cdk\nfrom dataclasses import dataclass\nfrom cdk_organizer.aws.stack_group import StackGroup\n\n@dataclass\nclass MyStackGroupConfig:\n    domain: str\n    ipv6: bool = True\n\n\nclass MyStackGroup(StackGroup[MyStackGroupConfig]):\n    def _load_stacks(self) -> None:\n        MyStack(\n            self.app,\n            self.get_stack_name(\'my-stack\'),\n            stack_group=self,\n            parameters=MyStackParameters(\n                domain=self.data.domain,\n                ipv6=self.data.ipv6\n            )\n        )\n```\n\n#### Terraform\n\n```python\nimport cdktf\nfrom dataclasses import dataclass\nfrom cdk_organizer.terraform.stack_group import StackGroup\n\n@dataclass\nclass MyStackGroupConfig:\n    domain: str\n    ipv6: bool = True\n\n\nclass MyStackGroup(StackGroup[MyStackGroupConfig]):\n    def _load_stacks(self) -> None:\n        MyStack(\n            self.app,\n            self.get_stack_name(\'my-stack\'),\n            stack_group=self,\n            parameters=MyStackParameters(\n                domain=self.data.domain,\n                ipv6=self.data.ipv6\n            )\n        )\n```\n\n#### Using Stack Attributes from Other Stack Groups\n\nIn some cases, you may want to use the attributes of another stack group. For example, refer the DNS Hosted Zone created by a shared stack group.\n\nTo resolve the group use the `self.resolve_group` function in the stack group class, like the example below:\n\n```python\nimport aws_cdk as cdk\nfrom dataclasses import dataclass\nfrom cdk_organizer.aws.stack_group import StackGroup\nfrom stacks.dns import DNSStackGroup\n\n@dataclass\nclass MyStackGroupConfig:\n    domain: str\n    ipv6: bool = True\n\n\nclass MyStackGroup(StackGroup[MyStackGroupConfig]):\n    def _load_stacks(self) -> None:\n        MyStack(\n            self.app,\n            self.get_stack_name(\'my-stack\'),\n            stack_group=self,\n            parameters=MyStackParameters(\n                domain=self.data.domain,\n                zone=self.resolve_group(DNSStackGroup).zone\n                ipv6=self.data.ipv6\n            )\n        )\n```\n\nThe function `get_stack_name` generates the stack name based on following pattern.\n\n**Pattern**: `{module_path}-{name}-{region}-{env}`\n\nConsider the following example:\n\n**module_path**: `myproject.myapp.www`\n**name**: `spa`\n**region**: `us-east-1`\n**env**: `dev`\n\nStack name will be:\n\n- `myproject-myapp-www-spa-us-east-1-dev`.\n\n### Config Structure\n\nCreate a `config` folder in the root of the project and structure it as follows:\n\n```text\n.\n+-- cdk.json\n+-- app.py\n+-- config/\n| +-- <env>/\n|   +-- config.yaml\n|   +-- <region>/\n|     +-- config.yaml\n|     +-- <groupName>/\n|         +-- config.yaml\n```\n\nThe first two levels are reserved to the environment name and the region name, the next levels needs to match the stack group structure.\n\nExample:\n\n```text\n.\n+-- cdk.json\n+-- app.py\n+-- config/\n| +-- config.yaml\n| +-- dev/\n|   +-- config.yaml\n|   +-- us-east-1/\n|     +-- config.yaml\n|     +-- app1/\n|       +-- config.yaml\n+-- stacks/\n| +-- app1/\n|   +-- stacks.py\n+-- templates/\n|   +-- stacks/\n```\n\n### Examples\n\n- [AWS CDK](https://github.com/cdk-organizer/cdk-organizer/tree/main/examples/python/aws-cdk)\n- [CDK for Terraform](https://github.com/cdk-organizer/cdk-organizer/tree/main/examples/python/cdktf)\n',
-    'author': 'None',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<3.10',
+# CDK Organizer Python Library
+
+This library contains the core features to handle CDK projects including:
+
+- Logging
+- Configuration Resolver
+- Stack Groups Loader
+- Naming Utils
+
+Full documentation: <https://cdk-organizer.github.io/>
+
+## Installation
+
+```bash
+pip install cdk-organizer[terraform,aws]
+```
+
+### Extras
+
+- `terraform`: Include `cdktf` as a dependency.
+- `aws`: Include `aws-cdk-lib` as a dependency.
+
+### CDK Start Script
+
+The content of the `app.py` file should be as follows:
+
+#### AWS CDK
+
+```python
+import aws_cdk as cdk
+from cdk_organizer.miscellaneous.logging import setup_logging
+from cdk_organizer.stack_group import StackGroupLoader
+
+app = cdk.App()
+logger = setup_logging(__name__, app.node.try_get_context("loglevel") or "INFO")
+loader = StackGroupLoader(app)
+
+loader.synth()
+app.synth()
+```
+
+#### CDK for Terraform
+
+```python
+from cdk_organizer.miscellaneous.logging import setup_logging
+from cdk_organizer.stack_group import StackGroupLoader
+from cdktf import App
+
+app = App()
+logger = setup_logging(__name__, app.node.try_get_context("loglevel") or "INFO")
+loader = StackGroupLoader(app)
+
+loader.synth()
+app.synth()
+```
+
+## Context Variables
+
+The following context variables are required to the CDK Organizer to work properly:
+
+- `env`
+- `region`
+
+The variables can be set in the `cdk.json` file:
+
+```json
+{
+  ...
+  "context": {
+    ...
+    "env": "dev",
+    "region": "us-east-1"
+    ...
+  }
+  ...
 }
+```
+
+Or passed as arguments to the CDK CLI:
+
+```bash
+cdk synth --context env=dev --context region=us-east-1
+```
+
+> In the `cdktf` CLI the context variables cannot be passed as arguments, so they need to be set in the `cdk.json` file. <https://github.com/hashicorp/terraform-cdk/issues/2019>
+> The `env` variable can also be set as an environment variable `CDK_ENV`.
+
+## Project Structure
+
+To apply the pattern purposed in this library for CDK projects, the following structure is required:
+
+```text
+.
++-- cdk.json
++-- app.py
+```
+
+### Stack Structure
+
+the stack class needs to inherit from class `cdk_organizer.aws.stack.Stack` for AWS CDK and `cdk_organizer.terraform.stack.Stack` for Terraform CDK.
+
+#### AWS CDK
+
+```python
+from constructs import Construct
+from cdk_organizer.aws.stack import Stack
+from cdk_organizer.aws.stack_group import StackGroup
+
+
+class MyStack(Stack):
+    def __init__(
+        self,
+        scope: Construct,
+        id: str,
+        stack_group: StackGroup,
+        **kwargs
+    ) -> None:
+        super().__init__(scope, id, stack_group, **kwargs)
+```
+
+#### Terraform CDK
+
+```python
+from constructs import Construct
+from cdk_organizer.terraform.stack import Stack
+from cdk_organizer.terraform.stack_group import StackGroup
+
+
+class MyStack(Stack):
+    def __init__(
+        self,
+        scope: Construct,
+        id: str,
+        stack_group: StackGroup,
+        **kwargs
+    ) -> None:
+        super().__init__(scope, id, stack_group, **kwargs)
+```
+
+#### Using S3 Backend
+
+To use S3 terraform backend, the following resources are required:
+
+- S3 Bucket
+- DynamoDB Table
+
+Add the following object to the environment configuration file:
+
+```yaml
+s3_backend:
+  bucket: "<bucket-name>"
+  region: "<aws-region>"
+  dynamodb_table: "<dynamodb-table-name>"
+```
+
+### Stack Group Structure
+
+Create a `stacks` folder in the root of the project and structure it as follows:
+
+```text
+.
++-- cdk.json
++-- app.py
++-- stacks/
+| +-- <groupName>/
+|   +-- stacks.py
+```
+
+The stack groups files follow this pattern:
+
+#### AWS CDK
+
+```python
+import aws_cdk as cdk
+from dataclasses import dataclass
+from cdk_organizer.aws.stack_group import StackGroup
+
+@dataclass
+class MyStackGroupConfig:
+    domain: str
+    ipv6: bool = True
+
+
+class MyStackGroup(StackGroup[MyStackGroupConfig]):
+    def _load_stacks(self) -> None:
+        MyStack(
+            self.app,
+            self.get_stack_name('my-stack'),
+            stack_group=self,
+            parameters=MyStackParameters(
+                domain=self.data.domain,
+                ipv6=self.data.ipv6
+            )
+        )
+```
+
+#### Terraform
+
+```python
+import cdktf
+from dataclasses import dataclass
+from cdk_organizer.terraform.stack_group import StackGroup
+
+@dataclass
+class MyStackGroupConfig:
+    domain: str
+    ipv6: bool = True
+
+
+class MyStackGroup(StackGroup[MyStackGroupConfig]):
+    def _load_stacks(self) -> None:
+        MyStack(
+            self.app,
+            self.get_stack_name('my-stack'),
+            stack_group=self,
+            parameters=MyStackParameters(
+                domain=self.data.domain,
+                ipv6=self.data.ipv6
+            )
+        )
+```
+
+#### Using Stack Attributes from Other Stack Groups
+
+In some cases, you may want to use the attributes of another stack group. For example, refer the DNS Hosted Zone created by a shared stack group.
+
+To resolve the group use the `self.resolve_group` function in the stack group class, like the example below:
+
+```python
+import aws_cdk as cdk
+from dataclasses import dataclass
+from cdk_organizer.aws.stack_group import StackGroup
+from stacks.dns import DNSStackGroup
+
+@dataclass
+class MyStackGroupConfig:
+    domain: str
+    ipv6: bool = True
+
+
+class MyStackGroup(StackGroup[MyStackGroupConfig]):
+    def _load_stacks(self) -> None:
+        MyStack(
+            self.app,
+            self.get_stack_name('my-stack'),
+            stack_group=self,
+            parameters=MyStackParameters(
+                domain=self.data.domain,
+                zone=self.resolve_group(DNSStackGroup).zone
+                ipv6=self.data.ipv6
+            )
+        )
+```
+
+The function `get_stack_name` generates the stack name based on following pattern.
+
+**Pattern**: `{module_path}-{name}-{region}-{env}`
+
+Consider the following example:
+
+**module_path**: `myproject.myapp.www`
+**name**: `spa`
+**region**: `us-east-1`
+**env**: `dev`
+
+Stack name will be:
+
+- `myproject-myapp-www-spa-us-east-1-dev`.
+
+### Config Structure
+
+Create a `config` folder in the root of the project and structure it as follows:
+
+```text
+.
++-- cdk.json
++-- app.py
++-- config/
+| +-- <env>/
+|   +-- config.yaml
+|   +-- <region>/
+|     +-- config.yaml
+|     +-- <groupName>/
+|         +-- config.yaml
+```
+
+The first two levels are reserved to the environment name and the region name, the next levels needs to match the stack group structure.
+
+Example:
+
+```text
+.
++-- cdk.json
++-- app.py
++-- config/
+| +-- config.yaml
+| +-- dev/
+|   +-- config.yaml
+|   +-- us-east-1/
+|     +-- config.yaml
+|     +-- app1/
+|       +-- config.yaml
++-- stacks/
+| +-- app1/
+|   +-- stacks.py
++-- templates/
+|   +-- stacks/
+```
+
+### Examples
 
+- [AWS CDK](https://github.com/cdk-organizer/cdk-organizer/tree/main/examples/python/aws-cdk)
+- [CDK for Terraform](https://github.com/cdk-organizer/cdk-organizer/tree/main/examples/python/cdktf)
 
-setup(**setup_kwargs)
```

