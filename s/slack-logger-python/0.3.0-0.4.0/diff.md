# Comparing `tmp/slack-logger-python-0.3.0.tar.gz` & `tmp/slack-logger-python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-logger-python-0.3.0.tar", last modified: Tue Aug  1 00:57:44 2023, max compression
+gzip compressed data, was "slack-logger-python-0.4.0.tar", last modified: Wed Aug  2 00:51:27 2023, max compression
```

## Comparing `slack-logger-python-0.3.0.tar` & `slack-logger-python-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.github/workflows/tagging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 00:57:34.000000 slack-logger-python-0.3.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/slack_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/slack_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/slack_logger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/slack_logger_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.279563 slack-logger-python-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.github/workflows/tagging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 00:51:19.000000 slack-logger-python-0.4.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/slack_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/slack_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/slack_logger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/slack_logger_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/utils.py
```

### Comparing `slack-logger-python-0.3.0/.github/workflows/deploy.yml` & `slack-logger-python-0.4.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/.github/workflows/format.yml` & `slack-logger-python-0.4.0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/.github/workflows/tagging.yml` & `slack-logger-python-0.4.0/.github/workflows/tagging.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/.gitignore` & `slack-logger-python-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/LICENSE` & `slack-logger-python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/PKG-INFO` & `slack-logger-python-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.3.0
+Version: 0.4.0
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `slack-logger-python-0.3.0/README.md` & `slack-logger-python-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/pyproject.toml` & `slack-logger-python-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/shell.nix` & `slack-logger-python-0.4.0/shell.nix`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.3.0/slack_logger/__init__.py` & `slack-logger-python-0.4.0/slack_logger/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,62 +25,77 @@
     logging.WARN: ":warning:",
     logging.INFO: ":bell:",
     logging.DEBUG: ":microscope:",
     logging.NOTSET: ":mega:",
 }
 
 
+class FilterType(Enum):
+    AnyAllowList = "AnyAllowList"
+    AllAllowList = "AllAllowList"
+    AnyDenyList = "AnyDenyList"
+    AllDenyList = "AllDenyList"
+
+
 @define
-class Configuration:
+class LogConfig:
     service: Optional[str] = None
     environment: Optional[str] = None
     context: List[str] = []
-    emojis: Dict[int, str] = DEFAULT_EMOJIS
     extra_fields: Dict[str, str] = {}
 
 
 @define
+class FormatConfig(LogConfig):
+    emojis: Dict[int, str] = DEFAULT_EMOJIS
+
+
+@define
+class FilterConfig(LogConfig):
+    use_regex: bool = False
+    filter_type: FilterType = FilterType.AnyAllowList
+
+
+@define
 class MessageDesign(ABC):
     @abstractmethod
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         pass
 
-    def get_env(self, config: Configuration, record: LogRecord) -> Optional[str]:
+    def get_env(self, config: LogConfig, record: LogRecord) -> Optional[str]:
         dynamic_env: Optional[str] = getattr(record, "environment", None)
         if dynamic_env is not None:
             return dynamic_env
         if config.environment is not None:
             return config.environment
         return None
 
-    def get_service(self, config: Configuration, record: LogRecord) -> Optional[str]:
+    def get_service(self, config: LogConfig, record: LogRecord) -> Optional[str]:
         dynamic_service: Optional[str] = getattr(record, "service", None)
         if dynamic_service is not None:
             return dynamic_service
         if config.service is not None:
             return config.service
         return None
 
-    def construct_header(
-        self, record: LogRecord, config: Configuration, icon: Optional[str], level: str
-    ) -> HeaderBlock:
+    def construct_header(self, record: LogRecord, config: LogConfig, icon: Optional[str], level: str) -> HeaderBlock:
         service: Optional[str] = self.get_service(config=config, record=record)
         header_msg: str
         if icon is not None:
             header_msg = f"{icon} "
         header_msg += level
         if config.service is not None:
             header_msg += f" | {service}"
         else:
             header_msg += f" | {record.name}"
 
         return HeaderBlock(text=PlainTextObject(text=header_msg))
 
     def construct_context(
-        self, config: Configuration, env: Optional[str], service: Optional[str]
+        self, config: LogConfig, env: Optional[str], service: Optional[str]
     ) -> Optional[ContextBlock]:
         if config.context != []:
             context_msg = ", ".join(config.context)
             return ContextBlock(elements=[MarkdownTextObject(text=context_msg)])
         elif env is not None and service is not None:
             return ContextBlock(elements=[MarkdownTextObject(text=f":point_right: {env}, {service}")])
         elif env is None:
@@ -101,15 +116,15 @@
 class NoDesign(MessageDesign):
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         return [SectionBlock(text=PlainTextObject(text=record.getMessage()))]
 
 
 @define
 class MinimalDesign(MessageDesign):
-    config: Configuration
+    config: FormatConfig
 
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         level = record.levelname
         message = record.getMessage()
         icon = self.config.emojis.get(record.levelno)
 
         header: HeaderBlock = self.construct_header(record=record, config=self.config, icon=icon, level=level)
@@ -121,15 +136,15 @@
         ]
 
         return default_blocks
 
 
 @define
 class RichDesign(MessageDesign):
-    config: Configuration
+    config: FormatConfig
 
     def format_blocks(self, record: LogRecord) -> Sequence[Optional[Block]]:
         level = record.levelname
         message = record.getMessage()
         icon = self.config.emojis.get(record.levelno)
 
         env: Optional[str] = self.get_env(config=self.config, record=record)
@@ -162,101 +177,124 @@
         ]
 
         return maybe_blocks
 
 
 class SlackFormatter(logging.Formatter):
     design: MessageDesign
-    config: Optional[Configuration]
+    config: Optional[FormatConfig]
 
-    def __init__(self, design: MessageDesign, config: Optional[Configuration] = None):
+    def __init__(self, design: MessageDesign, config: Optional[FormatConfig] = None):
         super(SlackFormatter, self).__init__()
         self.design = design
         self.config = config
 
     @classmethod
-    def plain(cls, config: Optional[Configuration] = None) -> "SlackFormatter":
+    def plain(cls, config: Optional[FormatConfig] = None) -> "SlackFormatter":
         return cls(design=NoDesign(), config=config)
 
     @classmethod
-    def minimal(cls, config: Configuration) -> "SlackFormatter":
+    def minimal(cls, config: FormatConfig) -> "SlackFormatter":
         return cls(design=MinimalDesign(config), config=config)
 
     @classmethod
-    def default(cls, config: Configuration) -> "SlackFormatter":
+    def default(cls, config: FormatConfig) -> "SlackFormatter":
         return cls(design=RichDesign(config), config=config)
 
     def format(self, record: LogRecord) -> str:
         super().format(record)
         return self.design.format(record)
 
 
-class FilterType(Enum):
-    AnyAllowList = "AnyAllowList"
-    AllAllowList = "AllAllowList"
-    AnyDenyList = "AnyDenyList"
-    AllDenyList = "AllDenyList"
-
-
 class SlackFilter(logging.Filter):
-    config: Configuration
-    tpe: FilterType
+    config: FilterConfig
 
-    def __init__(self, config: Configuration, filterType: FilterType = FilterType.AnyAllowList):
+    def __init__(self, config: FilterConfig):
         super(SlackFilter, self).__init__()
         self.config = config
-        self.tpe = filterType
 
     @classmethod
     def filter_by_fields(
-        cls, fields: Dict[str, str], filterType: FilterType = FilterType.AnyAllowList
+        cls, fields: Dict[str, str], filter_type: FilterType = FilterType.AnyAllowList, use_regex: bool = False
     ) -> "SlackFilter":
-        return cls(Configuration(extra_fields=fields), filterType=filterType)
+        return cls(FilterConfig(extra_fields=fields, filter_type=filter_type, use_regex=use_regex))
 
     @classmethod
-    def hide_by_fields(cls, fields: Dict[str, str], filterType: FilterType = FilterType.AnyDenyList) -> "SlackFilter":
-        return cls(Configuration(extra_fields=fields), filterType=filterType)
+    def hide_by_fields(
+        cls, fields: Dict[str, str], filter_type: FilterType = FilterType.AnyDenyList, use_regex: bool = False
+    ) -> "SlackFilter":
+        return cls(FilterConfig(extra_fields=fields, filter_type=filter_type, use_regex=use_regex))
+
+    def match_filter(self, cond_list: List[bool]) -> bool:
+        match self.config.filter_type:
+            case FilterType.AnyAllowList:
+                res = any(cond_list)
+            case FilterType.AllAllowList:
+                res = all(cond_list)
+            case FilterType.AnyDenyList:
+                res = not any(cond_list)
+            case FilterType.AllDenyList:
+                res = not all(cond_list)
+        log.debug(f"final result ({self.config.filter_type}): res({res}) = {cond_list}")
+        return res
+
+    def regexFilterConfig(self, serviceConfig: LogConfig, record: LogRecord) -> bool:
+        import re
 
-    def filterConfig(self, serviceConfig: Configuration, record: LogRecord) -> bool:
+        res_list = []
+        if self.config.service is not None:
+            regex = self.config.service
+            haystack = serviceConfig.service if serviceConfig.service is not None else ""
+            regex_match = re.search(regex, haystack)
+            res_list.append(regex_match is not None)
+        if self.config.environment is not None:
+            regex = self.config.environment
+            haystack = serviceConfig.environment if serviceConfig.environment is not None else ""
+            regex_match = re.search(regex, haystack)
+            res_list.append(regex_match is not None)
+        for field_key in self.config.extra_fields.keys():
+            filter_element = serviceConfig.extra_fields.get(field_key)
+            if filter_element is None:
+                res_list.append(False)
+            else:
+                regex = self.config.extra_fields[field_key]
+                haystack = filter_element
+                regex_match = re.search(regex, haystack)
+                log.debug(f"regex filter with regex = {regex}, haystack = {filter_element}")
+                res_list.append(regex_match is not None)
+
+        return self.match_filter(res_list)
+
+    def filterConfig(self, serviceConfig: LogConfig, record: LogRecord) -> bool:
         res_list = []
         if self.config.service is not None:
             res_list.append(serviceConfig.service == self.config.service)
         if self.config.environment is not None:
             res_list.append(serviceConfig.environment == self.config.environment)
-        if self.config.extra_fields != {}:
-            for f in self.config.extra_fields.items():
-                res_list.append(f in serviceConfig.extra_fields.items())
-
-        res: bool
-        match self.tpe:
-            case FilterType.AnyAllowList:
-                res = any(res_list)
-            case FilterType.AllAllowList:
-                res = all(res_list)
-            case FilterType.AnyDenyList:
-                res = not all(res_list)
-            case FilterType.AllDenyList:
-                res = not any(res_list)
+        for f in self.config.extra_fields.items():
+            res_list.append(f in serviceConfig.extra_fields.items())
 
-        log.debug(f"final result ({self.tpe}): res({res}) = {res_list}")
-        return res
+        return self.match_filter(res_list)
 
     def filter(self, record: LogRecord) -> bool:
         log_filters = getattr(record, "filter", None)
         if log_filters is None:
             return True
 
         extra_fields = log_filters.get("extra_fields", {})
         log.debug(f"EXTRA FIELDS: {extra_fields}")
-        rconfig: Configuration = Configuration(
+        rconfig: FilterConfig = FilterConfig(
             service=log_filters.get("service", None),
             environment=log_filters.get("environment", None),
             extra_fields=log_filters.get("extra_fields", {}),
         )
-        return self.filterConfig(serviceConfig=rconfig, record=record)
+        if self.config.use_regex is True:
+            return self.regexFilterConfig(serviceConfig=rconfig, record=record)
+        else:
+            return self.filterConfig(serviceConfig=rconfig, record=record)
 
 
 @define
 class DummyClient(AsyncWebhookClient):
     url: str = ""
 
     async def send(
@@ -280,15 +318,15 @@
             for block in blocks:
                 assert isinstance(block, Block)
                 res.append(block.to_dict())
             t = json.dumps({"blocks": res})
         else:
             t = json.dumps({"text": str(text)})
 
-        log.info(t)
+        log.debug(t)
         return WebhookResponse(url="", status_code=200, body="ok", headers={})
 
 
 class SlackHandler(logging.Handler):
     client: AsyncWebhookClient
 
     def __init__(self, client: AsyncWebhookClient):
@@ -328,15 +366,15 @@
 
         except Exception:
             self.handleError(record)
 
     def handle(self, record: LogRecord) -> bool:
         # This pre-filters the messages with the Slack Filters
         if isinstance(self.formatter, SlackFormatter) and self.formatter.config is not None:
-            format_config: Configuration = self.formatter.config
+            format_config: LogConfig = self.formatter.config
             for sf in self.filters:
                 if isinstance(sf, SlackFilter):
                     res = sf.filterConfig(serviceConfig=format_config, record=record)
                     if not res:
                         return False
 
         return super().handle(record)
```

### Comparing `slack-logger-python-0.3.0/slack_logger_python.egg-info/PKG-INFO` & `slack-logger-python-0.4.0/slack_logger_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.3.0
+Version: 0.4.0
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `slack-logger-python-0.3.0/slack_logger_python.egg-info/SOURCES.txt` & `slack-logger-python-0.4.0/slack_logger_python.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 slack_logger/py.typed
 slack_logger_python.egg-info/PKG-INFO
 slack_logger_python.egg-info/SOURCES.txt
 slack_logger_python.egg-info/dependency_links.txt
 slack_logger_python.egg-info/requires.txt
 slack_logger_python.egg-info/top_level.txt
 tests/__init__.py
-tests/test_basic.py
+tests/test_basic.py
+tests/test_filter.py
+tests/test_formatter.py
+tests/utils.py
```

