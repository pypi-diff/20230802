# Comparing `tmp/kpops-1.3.2.tar.gz` & `tmp/kpops-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.3.2.tar", max compression
+gzip compressed data, was "kpops-1.4.0.tar", max compression
```

## Comparing `kpops-1.3.2.tar` & `kpops-1.4.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1064 2023-07-13 08:42:25.158994 kpops-1.3.2/LICENSE
--rw-r--r--   0        0        0     2350 2023-07-13 08:42:25.158994 kpops-1.3.2/README.md
--rw-r--r--   0        0        0       22 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/cli/exception.py
--rw-r--r--   0        0        0    11641 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/cli/main.py
--rw-r--r--   0        0        0     4283 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1969 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/dry_run_handler.py
--rw-r--r--   0        0        0       92 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0    10515 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2152 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     5253 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8142 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      235 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5832 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1825 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      999 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6272 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      231 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9358 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6917 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     7711 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     6658 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    15918 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     6941 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0       66 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     3340 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     8915 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2831 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     9067 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3463 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    13179 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     3878 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/dict_ops.py
--rw-r--r--   0        0        0     2597 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1032 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/environment.py
--rw-r--r--   0        0        0     5620 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      552 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     2563 2023-07-13 08:42:25.162994 kpops-1.3.2/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1933 2023-07-13 08:42:25.166994 kpops-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 kpops-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 07:59:00.969198 kpops-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2350 2023-08-02 07:59:00.969198 kpops-1.4.0/README.md
+-rw-r--r--   0        0        0      206 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/cli/exception.py
+-rw-r--r--   0        0        0    12340 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/cli/main.py
+-rw-r--r--   0        0        0     4283 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1969 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1167 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       92 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0    10515 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     5253 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     7932 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      229 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5832 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1825 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      999 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6272 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      225 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9358 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6749 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      616 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     7710 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     6658 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    15918 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     6984 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0       66 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2471 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3340 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     8722 2023-08-02 07:59:00.973198 kpops-1.4.0/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1110 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2831 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9067 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3463 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    13844 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     3878 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2597 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1032 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5620 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      552 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     2563 2023-08-02 07:59:00.977198 kpops-1.4.0/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1951 2023-08-02 07:59:00.977198 kpops-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3884 1970-01-01 00:00:00.000000 kpops-1.4.0/PKG-INFO
```

### Comparing `kpops-1.3.2/LICENSE` & `kpops-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/README.md` & `kpops-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/cli/custom_formatter.py` & `kpops-1.4.0/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/cli/main.py` & `kpops-1.4.0/kpops/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterator, Optional
 
+import dtyper
 import typer
 
 from kpops import __version__
 from kpops.cli.custom_formatter import CustomFormatter
 from kpops.cli.pipeline_config import ENV_PREFIX, PipelineConfig
 from kpops.cli.registry import Registry
 from kpops.component_handlers import ComponentHandlers
@@ -21,15 +22,15 @@
 from kpops.utils.gen_schema import SchemaScope, gen_config_schema, gen_pipeline_schema
 
 if TYPE_CHECKING:
     from kpops.components.base_components import PipelineComponent
 
 LOG_DIVIDER = "#" * 100
 
-app = typer.Typer(pretty_exceptions_enable=False)
+app = dtyper.Typer(pretty_exceptions_enable=False)
 
 BASE_DIR_PATH_OPTION: Path = typer.Option(
     default=Path("."),
     exists=True,
     dir_okay=True,
     file_okay=False,
     envvar=f"{ENV_PREFIX}PIPELINE_BASE_DIR",
@@ -73,20 +74,23 @@
 
 DRY_RUN: bool = typer.Option(
     True,
     "--dry-run/--execute",
     help="Whether to dry run the command or execute it",
 )
 
+VERBOSE_OPTION = typer.Option(False, help="Enable verbose printing")
+
 COMPONENTS_MODULES: str | None = typer.Argument(
     default=None,
     help="Custom Python module containing your project-specific components",
 )
 
 logger = logging.getLogger()
+logging.getLogger("httpx").setLevel(logging.WARNING)
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(CustomFormatter())
 logger.addHandler(stream_handler)
 
 log = logging.getLogger("")
 
 
@@ -155,15 +159,17 @@
     pipeline: Pipeline, steps: str | None
 ) -> list[PipelineComponent]:
     if steps:
         return filter_steps_to_apply(pipeline, steps=parse_steps(steps))
     return list(pipeline)
 
 
-def reverse_pipeline_steps(pipeline, steps) -> Iterator[PipelineComponent]:
+def reverse_pipeline_steps(
+    pipeline: Pipeline, steps: str | None
+) -> Iterator[PipelineComponent]:
     return reversed(get_steps_to_apply(pipeline, steps))
 
 
 def log_action(action: str, pipeline_component: PipelineComponent):
     log.info("\n")
     log.info(LOG_DIVIDER)
     log.info(f"{action} {pipeline_component.name}")
@@ -180,15 +186,15 @@
         pipeline_config = PipelineConfig(defaults_path=defaults)
     else:
         pipeline_config = PipelineConfig()
         pipeline_config.defaults_path = config.parent / pipeline_config.defaults_path
     return pipeline_config
 
 
-@app.command(
+@app.command(  # pyright: ignore[reportGeneralTypeIssues] https://github.com/rec/dtyper/issues/8
     help="""
     Generate json schema.
 
     The schemas can be used to enable support for kpops files in a text editor.
     """
 )
 def schema(
@@ -210,36 +216,36 @@
     match scope:
         case SchemaScope.PIPELINE:
             gen_pipeline_schema(components_module, include_stock_components)
         case SchemaScope.CONFIG:
             gen_config_schema()
 
 
-@app.command(
+@app.command(  # pyright: ignore[reportGeneralTypeIssues] https://github.com/rec/dtyper/issues/8
     help="Enriches pipelines steps with defaults. The output is used as input for the deploy/destroy/... commands."
 )
 def generate(
-    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     pipeline_path: Path = PIPELINE_PATH_ARG,
     components_module: Optional[str] = COMPONENTS_MODULES,
+    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     defaults: Optional[Path] = DEFAULT_PATH_OPTION,
     config: Path = CONFIG_PATH_OPTION,
-    verbose: bool = typer.Option(False, help="Enable verbose printing"),
+    verbose: bool = VERBOSE_OPTION,
     template: bool = typer.Option(False, help="Run Helm template"),
     steps: Optional[str] = PIPELINE_STEPS,
     api_version: Optional[str] = typer.Option(
         None, help="Kubernetes API version used for Capabilities.APIVersions"
     ),
     ca_file: Optional[str] = typer.Option(
         None, help="Verify certificates of HTTPS-enabled servers using this CA bundle"
     ),
     cert_file: Optional[str] = typer.Option(
         None, help="Identify HTTPS client using this SSL certificate file"
     ),
-):
+) -> Pipeline:
     pipeline_config = create_pipeline_config(config, defaults, verbose)
     pipeline = setup_pipeline(
         pipeline_base_dir, pipeline_path, components_module, pipeline_config
     )
     pipeline.print_yaml()
 
     if template:
@@ -254,89 +260,97 @@
                 '--api-version'\n \
                 '--steps'"
         )
 
     return pipeline
 
 
-@app.command(help="Deploy pipeline steps")
+@app.command(
+    help="Deploy pipeline steps"
+)  # pyright: ignore[reportGeneralTypeIssues] https://github.com/rec/dtyper/issues/8
 def deploy(
-    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     pipeline_path: Path = PIPELINE_PATH_ARG,
     components_module: Optional[str] = COMPONENTS_MODULES,
+    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     defaults: Optional[Path] = DEFAULT_PATH_OPTION,
     config: Path = CONFIG_PATH_OPTION,
-    verbose: bool = False,
     dry_run: bool = DRY_RUN,
+    verbose: bool = VERBOSE_OPTION,
     steps: Optional[str] = PIPELINE_STEPS,
 ):
     pipeline_config = create_pipeline_config(config, defaults, verbose)
     pipeline = setup_pipeline(
         pipeline_base_dir, pipeline_path, components_module, pipeline_config
     )
 
     steps_to_apply = get_steps_to_apply(pipeline, steps)
     for component in steps_to_apply:
         log_action("Deploy", component)
         component.deploy(dry_run)
 
 
-@app.command(help="Destroy pipeline steps")
+@app.command(
+    help="Destroy pipeline steps"
+)  # pyright: ignore[reportGeneralTypeIssues] https://github.com/rec/dtyper/issues/8
 def destroy(
-    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     pipeline_path: Path = PIPELINE_PATH_ARG,
     components_module: Optional[str] = COMPONENTS_MODULES,
+    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     defaults: Optional[Path] = DEFAULT_PATH_OPTION,
     config: Path = CONFIG_PATH_OPTION,
     steps: Optional[str] = PIPELINE_STEPS,
+    verbose: bool = VERBOSE_OPTION,
     dry_run: bool = DRY_RUN,
-    verbose: bool = False,
 ):
     pipeline_config = create_pipeline_config(config, defaults, verbose)
     pipeline = setup_pipeline(
         pipeline_base_dir, pipeline_path, components_module, pipeline_config
     )
     pipeline_steps = reverse_pipeline_steps(pipeline, steps)
     for component in pipeline_steps:
         log_action("Destroy", component)
         component.destroy(dry_run)
 
 
-@app.command(help="Reset pipeline steps")
+@app.command(
+    help="Reset pipeline steps"
+)  # pyright: ignore[reportGeneralTypeIssues] https://github.com/rec/dtyper/issues/8
 def reset(
-    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     pipeline_path: Path = PIPELINE_PATH_ARG,
     components_module: Optional[str] = COMPONENTS_MODULES,
+    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     defaults: Optional[Path] = DEFAULT_PATH_OPTION,
     config: Path = CONFIG_PATH_OPTION,
     steps: Optional[str] = PIPELINE_STEPS,
     dry_run: bool = DRY_RUN,
-    verbose: bool = False,
+    verbose: bool = VERBOSE_OPTION,
 ):
     pipeline_config = create_pipeline_config(config, defaults, verbose)
     pipeline = setup_pipeline(
         pipeline_base_dir, pipeline_path, components_module, pipeline_config
     )
     pipeline_steps = reverse_pipeline_steps(pipeline, steps)
     for component in pipeline_steps:
         log_action("Reset", component)
         component.destroy(dry_run)
         component.reset(dry_run)
 
 
-@app.command(help="Clean pipeline steps")
+@app.command(
+    help="Clean pipeline steps"
+)  # pyright: ignore[reportGeneralTypeIssues] https://github.com/rec/dtyper/issues/8
 def clean(
-    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     pipeline_path: Path = PIPELINE_PATH_ARG,
     components_module: Optional[str] = COMPONENTS_MODULES,
+    pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     defaults: Optional[Path] = DEFAULT_PATH_OPTION,
     config: Path = CONFIG_PATH_OPTION,
     steps: Optional[str] = PIPELINE_STEPS,
     dry_run: bool = DRY_RUN,
-    verbose: bool = False,
+    verbose: bool = VERBOSE_OPTION,
 ):
     pipeline_config = create_pipeline_config(config, defaults, verbose)
     pipeline = setup_pipeline(
         pipeline_base_dir, pipeline_path, components_module, pipeline_config
     )
     pipeline_steps = reverse_pipeline_steps(pipeline, steps)
     for component in pipeline_steps:
```

### Comparing `kpops-1.3.2/kpops/cli/pipeline_config.py` & `kpops-1.4.0/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/cli/registry.py` & `kpops-1.4.0/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/__init__.py` & `kpops-1.4.0/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/helm_wrapper/dry_run_handler.py` & `kpops-1.4.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.4.0/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.4.0/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.4.0/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.4.0/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.4.0/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import time
 from time import sleep
 from typing import Any
 
-import requests
+import httpx
 
 from kpops.component_handlers.kafka_connect.exception import (
     ConnectorNotFoundException,
     KafkaConnectError,
 )
 from kpops.component_handlers.kafka_connect.model import (
     KafkaConnectConfig,
@@ -46,47 +46,47 @@
         API Reference: https://docs.confluent.io/platform/current/connect/references/restapi.html#post--connectors
         :param connector_name: The name of the connector
         :param kafka_connect_config: The config of the connector
         :return: The current connector info if successful
         """
         config_json = kafka_connect_config.dict(exclude_none=True)
         connect_data = {"name": connector_name, "config": config_json}
-        response = requests.post(
+        response = httpx.post(
             url=f"{self._host}/connectors", headers=HEADERS, json=connect_data
         )
-        if response.status_code == requests.status_codes.codes.created:
+        if response.status_code == httpx.codes.CREATED:
             log.info(f"Connector {connector_name} created.")
             log.debug(response.json())
             return KafkaConnectResponse(**response.json())
-        elif response.status_code == requests.status_codes.codes.conflict:
+        elif response.status_code == httpx.codes.CONFLICT:
             log.warning(
                 "Rebalancing in progress while creating a connector... Retrying..."
             )
             time.sleep(1)
             self.create_connector(connector_name, kafka_connect_config)
         raise KafkaConnectError(response)
 
     def get_connector(self, connector_name: str) -> KafkaConnectResponse:
         """
         Get information about the connector.
         API Reference: https://docs.confluent.io/platform/current/connect/references/restapi.html#get--connectors-(string-name)
         :param connector_name: Nameof the crated connector
         :return: Information about the connector
         """
-        response = requests.get(
+        response = httpx.get(
             url=f"{self._host}/connectors/{connector_name}", headers=HEADERS
         )
-        if response.status_code == requests.status_codes.codes.ok:
+        if response.status_code == httpx.codes.OK:
             log.info(f"Connector {connector_name} exists.")
             log.debug(response.json())
             return KafkaConnectResponse(**response.json())
-        elif response.status_code == requests.status_codes.codes.not_found:
+        elif response.status_code == httpx.codes.NOT_FOUND:
             log.info(f"The named connector {connector_name} does not exists.")
             raise ConnectorNotFoundException()
-        elif response.status_code == requests.status_codes.codes.conflict:
+        elif response.status_code == httpx.codes.CONFLICT:
             log.warning(
                 "Rebalancing in progress while getting a connector... Retrying..."
             )
             sleep(1)
             self.get_connector(connector_name)
         raise KafkaConnectError(response)
 
@@ -96,29 +96,29 @@
         """
         Create a new connector using the given configuration, or update the configuration for an existing connector.
         :param connector_name: Name of the created connector
         :param kafka_connect_config: Configuration parameters for the connector.
         :return: Information about the connector after the change has been made.
         """
         config_json = kafka_connect_config.dict(exclude_none=True)
-        response = requests.put(
+        response = httpx.put(
             url=f"{self._host}/connectors/{connector_name}/config",
             headers=HEADERS,
             json=config_json,
         )
         data: dict = response.json()
-        if response.status_code == requests.status_codes.codes.ok:
+        if response.status_code == httpx.codes.OK:
             log.info(f"Config for connector {connector_name} updated.")
             log.debug(data)
             return KafkaConnectResponse(**data)
-        if response.status_code == requests.status_codes.codes.created:
+        if response.status_code == httpx.codes.CREATED:
             log.info(f"Connector {connector_name} created.")
             log.debug(data)
             return KafkaConnectResponse(**data)
-        elif response.status_code == requests.status_codes.codes.conflict:
+        elif response.status_code == httpx.codes.CONFLICT:
             log.warning(
                 "Rebalancing in progress while updating a connector... Retrying..."
             )
             sleep(1)
             self.update_connector_config(connector_name, kafka_connect_config)
         raise KafkaConnectError(response)
 
@@ -141,21 +141,21 @@
         :param kafka_connect_config: Configuration parameters for the connector.
         :return:
         """
 
         config_json = self.get_connector_config(connector_name, kafka_connect_config)
         connector_class = ConnectWrapper.get_connector_class_name(config_json)
 
-        response = requests.put(
+        response = httpx.put(
             url=f"{self._host}/connector-plugins/{connector_class}/config/validate",
             headers=HEADERS,
             json=config_json,
         )
 
-        if response.status_code == requests.status_codes.codes.ok:
+        if response.status_code == httpx.codes.OK:
             kafka_connect_error_response = KafkaConnectConfigErrorResponse(
                 **response.json()
             )
 
             errors = []
             if kafka_connect_error_response.error_count > 0:
                 for config in kafka_connect_error_response.configs:
@@ -168,24 +168,24 @@
         raise KafkaConnectError(response)
 
     def delete_connector(self, connector_name: str) -> None:
         """
         Deletes a connector, halting all tasks and deleting its configuration.
         API Reference:https://docs.confluent.io/platform/current/connect/references/restapi.html#delete--connectors-(string-name)-
         """
-        response = requests.delete(
+        response = httpx.delete(
             url=f"{self._host}/connectors/{connector_name}", headers=HEADERS
         )
-        if response.status_code == requests.status_codes.codes.no_content:
+        if response.status_code == httpx.codes.NO_CONTENT:
             log.info(f"Connector {connector_name} deleted.")
             return
-        elif response.status_code == requests.status_codes.codes.not_found:
+        elif response.status_code == httpx.codes.NOT_FOUND:
             log.info(f"The named connector {connector_name} does not exists.")
             raise ConnectorNotFoundException()
-        elif response.status_code == requests.status_codes.codes.conflict:
+        elif response.status_code == httpx.codes.CONFLICT:
             log.warning(
                 "Rebalancing in progress while deleting a connector... Retrying..."
             )
             sleep(1)
             self.delete_connector(connector_name)
         raise KafkaConnectError(response)
```

### Comparing `kpops-1.3.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.4.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.4.0/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.4.0/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.4.0/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/topic/handler.py` & `kpops-1.4.0/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/topic/model.py` & `kpops-1.4.0/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.4.0/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from functools import cached_property
 
-import requests
+import httpx
 
 from kpops.cli.pipeline_config import PipelineConfig
 from kpops.component_handlers.topic.exception import (
     KafkaRestProxyError,
     TopicNotFoundException,
 )
 from kpops.component_handlers.topic.model import (
@@ -40,16 +40,16 @@
         More information about the cluster ID can be found here:
         https://docs.confluent.io/platform/current/kafka-rest/api.html#cluster-v3
 
         Currently both Kafka and Kafka REST Proxy are only aware of the Kafka cluster pointed at by the
         bootstrap.servers configuration. Therefore, only one Kafka cluster will be returned.
         :return: The Kafka cluster ID.
         """
-        response = requests.get(url=f"{self._host}/v3/clusters")
-        if response.status_code == requests.status_codes.codes.ok:
+        response = httpx.get(url=f"{self._host}/v3/clusters")
+        if response.status_code == httpx.codes.OK:
             cluster_information = response.json()
             return cluster_information["data"][0]["cluster_id"]
 
         raise KafkaRestProxyError(response)
 
     @property
     def host(self) -> str:
@@ -57,60 +57,60 @@
 
     def create_topic(self, topic_spec: TopicSpec) -> None:
         """
         Creates a topic.
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#post--clusters-cluster_id-topics
         :param topic_spec: The topic specification.
         """
-        response = requests.post(
+        response = httpx.post(
             url=f"{self._host}/v3/clusters/{self.cluster_id}/topics",
             headers=HEADERS,
             json=topic_spec.dict(exclude_none=True),
         )
-        if response.status_code == requests.status_codes.codes.created:
+        if response.status_code == httpx.codes.CREATED:
             log.info(f"Topic {topic_spec.topic_name} created.")
             log.debug(response.json())
             return
 
         raise KafkaRestProxyError(response)
 
     def delete_topic(self, topic_name: str) -> None:
         """
         Deletes a topic
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#delete--clusters-cluster_id-topics-topic_name
         :param topic_name: Name of the topic
         """
-        response = requests.delete(
+        response = httpx.delete(
             url=f"{self.host}/v3/clusters/{self.cluster_id}/topics/{topic_name}",
             headers=HEADERS,
         )
-        if response.status_code == requests.status_codes.codes.no_content:
+        if response.status_code == httpx.codes.NO_CONTENT:
             log.info(f"Topic {topic_name} deleted.")
             return
 
         raise KafkaRestProxyError(response)
 
     def get_topic(self, topic_name: str) -> TopicResponse:
         """
         Returns the topic with the given topic_name.
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#get--clusters-cluster_id-topics-topic_name
         :param topic_name: The topic name.
         :return: Response of the get topic API
         """
-        response = requests.get(
+        response = httpx.get(
             url=f"{self.host}/v3/clusters/{self.cluster_id}/topics/{topic_name}",
             headers=HEADERS,
         )
-        if response.status_code == requests.status_codes.codes.ok:
+        if response.status_code == httpx.codes.OK:
             log.debug(f"Topic {topic_name} found.")
             log.debug(response.json())
             return TopicResponse(**response.json())
 
         elif (
-            response.status_code == requests.status_codes.codes.not_found
+            response.status_code == httpx.codes.NOT_FOUND
             and response.json()["error_code"] == 40403
         ):
             log.debug(f"Topic {topic_name} not found.")
             log.debug(response.json())
             raise TopicNotFoundException()
 
         raise KafkaRestProxyError(response)
@@ -118,26 +118,26 @@
     def get_topic_config(self, topic_name: str) -> TopicConfigResponse:
         """
         Return the config with the given topic_name.
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#acl-v3
         :param topic_name: The topic name.
         :return: The topic configuration.
         """
-        response = requests.get(
+        response = httpx.get(
             url=f"{self.host}/v3/clusters/{self.cluster_id}/topics/{topic_name}/configs",
             headers=HEADERS,
         )
 
-        if response.status_code == requests.status_codes.codes.ok:
+        if response.status_code == httpx.codes.OK:
             log.debug(f"Configs for {topic_name} found.")
             log.debug(response.json())
             return TopicConfigResponse(**response.json())
 
         elif (
-            response.status_code == requests.status_codes.codes.not_found
+            response.status_code == httpx.codes.NOT_FOUND
             and response.json()["error_code"] == 40403
         ):
             log.debug(f"Configs for {topic_name} not found.")
             log.debug(response.json())
             raise TopicNotFoundException()
 
         raise KafkaRestProxyError(response)
@@ -145,35 +145,35 @@
     def batch_alter_topic_config(self, topic_name: str, json_body: list[dict]) -> None:
         """
         Reset config of given config_name param to the default value on the kafka server.
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#post--clusters-cluster_id-topics-topic_name-configs-alter
         :param topic_name: The topic name.
         :param config_name: The configuration parameter name.
         """
-        response = requests.post(
+        response = httpx.post(
             url=f"{self.host}/v3/clusters/{self.cluster_id}/topics/{topic_name}/configs:alter",
             headers=HEADERS,
             json={"data": json_body},
         )
-        if response.status_code == requests.status_codes.codes.no_content:
+        if response.status_code == httpx.codes.NO_CONTENT:
             log.info(f"Config of topic {topic_name} was altered.")
             return
 
         raise KafkaRestProxyError(response)
 
     def get_broker_config(self) -> BrokerConfigResponse:
         """
         Return the list of configuration parameters for all the brokers in the given Kafka cluster.
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#get--clusters-cluster_id-brokers---configs
         :return: The broker configuration.
         """
-        response = requests.get(
+        response = httpx.get(
             url=f"{self.host}/v3/clusters/{self.cluster_id}/brokers/-/configs",
             headers=HEADERS,
         )
 
-        if response.status_code == requests.status_codes.codes.ok:
+        if response.status_code == httpx.codes.OK:
             log.debug("Broker configs found.")
             log.debug(response.json())
             return BrokerConfigResponse(**response.json())
 
         raise KafkaRestProxyError(response)
```

### Comparing `kpops-1.3.2/kpops/component_handlers/topic/utils.py` & `kpops-1.4.0/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/component_handlers/utils/exception.py` & `kpops-1.4.0/kpops/component_handlers/utils/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 
-import requests
+import httpx
 
-log = logging.getLogger("RequestException")
+log = logging.getLogger("HttpxException")
 
 
-class RequestsException(Exception):
-    def __init__(self, response: requests.Response) -> None:
+class HttpxException(Exception):
+    def __init__(self, response: httpx.Response) -> None:
         self.error_code = response.status_code
         self.error_msg = "Something went wrong!"
         try:
             log.error(
                 f"The request responded with the code {self.error_code}. Error body: {response.json()}"
             )
             response.raise_for_status()
-        except requests.HTTPError as e:
+        except httpx.HTTPError as e:
             self.error_msg = str(e)
             log.error(f"More information: {self.error_msg}")
         super().__init__()
```

### Comparing `kpops-1.3.2/kpops/components/base_components/base_defaults_component.py` & `kpops-1.4.0/kpops/components/base_components/base_defaults_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     :param validate: Whether to run custom validation on the component, defaults to True
     :type validate: bool, optional
     """
 
     type: str = Field(
         default=..., description=describe_attr("type", __doc__), const=True
     )
-
     enrich: bool = Field(
         default=False,
         description=describe_attr("enrich", __doc__),
         exclude=True,
         hidden_from_schema=True,
     )
     config: PipelineConfig = Field(
```

### Comparing `kpops-1.3.2/kpops/components/base_components/kafka_app.py` & `kpops-1.4.0/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/base_components/kafka_connector.py` & `kpops-1.4.0/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/base_components/kubernetes_app.py` & `kpops-1.4.0/kpops/components/base_components/kubernetes_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     @property
     def helm_release_name(self) -> str:
         """The name for the Helm release. Can be overridden."""
         return self.name
 
     @override
     def _validate_custom(self, **kwargs) -> None:
+        super()._validate_custom(**kwargs)
         self.validate_kubernetes_name(self.name)
 
     @override
     def template(
         self, api_version: str | None, ca_file: str | None, cert_file: str | None
     ) -> None:
         flags = HelmTemplateFlags(api_version, ca_file, cert_file, self.version)
```

### Comparing `kpops-1.3.2/kpops/components/base_components/models/from_section.py` & `kpops-1.4.0/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/base_components/models/to_section.py` & `kpops-1.4.0/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/base_components/pipeline_component.py` & `kpops-1.4.0/kpops/components/base_components/pipeline_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,58 +23,52 @@
 
 
 class PipelineComponent(BaseDefaultsComponent):
     """Base class for all components
 
     :param name: Component name
     :type name: str
+    :param prefix: Pipeline prefix that will prefix every component name.
+        If you wish to not have any prefix you can specify an empty string.,
+        defaults to "${pipeline_name}-"
+    :type prefix: str, optional
     :param from_: Topic(s) and/or components from which the component will read
         input, defaults to None
     :type from_: FromSection, optional
-    :param app: Application-specific settings, defaults to None
-    :type app: object, optional
     :param to: Topic(s) into which the component will write output,
         defaults to None
     :type to: ToSection, optional
-    :param prefix: Pipeline prefix that will prefix every component name.
-        If you wish to not have any prefix you can specify an empty string.,
-        defaults to "${pipeline_name}-"
-    :type prefix: str, optional
     """
 
     type: str = Field(
         default="pipeline-component",
         description=describe_attr("type", __doc__),
         const=True,
     )
     schema_type: Literal["pipeline-component"] = Field(
         default="pipeline-component",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
-    name: str = Field(default=..., description="Component name")
+    name: str = Field(default=..., description=describe_attr("name", __doc__))
+    prefix: str = Field(
+        default="${pipeline_name}-",
+        description=describe_attr("prefix", __doc__),
+    )
     from_: FromSection | None = Field(
         default=None,
         alias="from",
         title="From",
         description=describe_attr("from_", __doc__),
     )
-    app: object | None = Field(
-        default=None,
-        description=describe_attr("app", __doc__),
-    )
     to: ToSection | None = Field(
         default=None,
         description=describe_attr("to", __doc__),
     )
-    prefix: str = Field(
-        default="${pipeline_name}-",
-        description=describe_attr("prefix", __doc__),
-    )
 
     class Config(CamelCaseConfig, DescConfig):
         extra = Extra.allow
         keep_untouched = (cached_property,)
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
```

### Comparing `kpops-1.3.2/kpops/components/streams_bootstrap/producer/model.py` & `kpops-1.4.0/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.4.0/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.4.0/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.4.0/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/pipeline_generator/pipeline.py` & `kpops-1.4.0/kpops/pipeline_generator/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import logging
+from collections import Counter
 from collections.abc import Iterator
 from contextlib import suppress
 from pathlib import Path
 
 import yaml
 from pydantic import BaseModel
 from rich.console import Console
@@ -22,14 +23,18 @@
 log = logging.getLogger("PipelineGenerator")
 
 
 class ParsingException(Exception):
     pass
 
 
+class ValidationError(Exception):
+    pass
+
+
 class PipelineComponents(BaseModel):
     """Stores the pipeline components"""
 
     components: list[PipelineComponent] = []
 
     @property
     def last(self) -> PipelineComponent:
@@ -47,22 +52,33 @@
 
     def __bool__(self) -> bool:
         return bool(self.components)
 
     def __iter__(self) -> Iterator[PipelineComponent]:
         return iter(self.components)
 
+    def __len__(self) -> int:
+        return len(self.components)
+
+    def validate_unique_names(self) -> None:
+        step_names = [component.name for component in self.components]
+        duplicates = [name for name, count in Counter(step_names).items() if count > 1]
+        if duplicates:
+            raise ValidationError(
+                f"step names should be unique. duplicate step names: {', '.join(duplicates)}"
+            )
+
     @staticmethod
     def _populate_component_name(component: PipelineComponent) -> None:
         component.name = component.prefix + component.name
         with suppress(
             AttributeError  # Some components like Kafka Connect do not have a name_override attribute
         ):
-            if component.app and getattr(component.app, "name_override") is None:
-                setattr(component.app, "name_override", component.name)
+            if (app := getattr(component, "app")) and app.name_override is None:
+                app.name_override = component.name
 
 
 def create_env_components_index(
     environment_components: list[dict],
 ) -> dict[str, dict]:
     """Create an index for all registered components in the project
 
@@ -92,14 +108,15 @@
     ) -> None:
         self.components: PipelineComponents = PipelineComponents()
         self.handlers = handlers
         self.config = config
         self.registry = registry
         self.env_components_index = create_env_components_index(environment_components)
         self.parse_components(component_list)
+        self.validate()
 
     @classmethod
     def load_from_yaml(
         cls,
         base_dir: Path,
         path: Path,
         registry: Registry,
@@ -269,14 +286,17 @@
     def __str__(self) -> str:
         return yaml.dump(
             json.loads(  # HACK: serialize types on Pydantic model export, which are not serialized by .dict(); e.g. pathlib.Path
                 self.components.json(exclude_none=True, by_alias=True)
             )
         )
 
+    def __len__(self) -> int:
+        return len(self.components)
+
     def substitute_in_component(self, component_as_dict: dict) -> dict:
         """Substitute all $-placeholders in a component in dict representation
 
         :param component_as_dict: Component represented as dict
         :type component_as_dict: dict
         :return: Updated component
         :rtype: dict
@@ -301,14 +321,17 @@
         return json.loads(
             substitute_nested(
                 json.dumps(component_as_dict),
                 **update_nested_pair(substitution, ENV),
             )
         )
 
+    def validate(self) -> None:
+        self.components.validate_unique_names()
+
     @staticmethod
     def pipeline_filename_environment(path: Path, config: PipelineConfig) -> Path:
         """Add the environment name from the PipelineConfig to the pipeline.yaml path
 
         :param path: Path to pipeline.yaml file
         :param config: The PipelineConfig
         :returns: An absolute path to the pipeline_<environment>.yaml
```

### Comparing `kpops-1.3.2/kpops/utils/dict_differ.py` & `kpops-1.4.0/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/utils/dict_ops.py` & `kpops-1.4.0/kpops/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/utils/docstring.py` & `kpops-1.4.0/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/utils/environment.py` & `kpops-1.4.0/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/utils/gen_schema.py` & `kpops-1.4.0/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/utils/pydantic.py` & `kpops-1.4.0/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/kpops/utils/yaml_loading.py` & `kpops-1.4.0/kpops/utils/yaml_loading.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.2/pyproject.toml` & `kpops-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.3.2"
+version = "1.4.0"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
@@ -27,34 +27,35 @@
 kpops = "kpops.cli.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = { extras = ["dotenv"], version = "^1.10.8" }
 rich = "^12.4.4"
 PyYAML = "^6.0"
-requests = "^2.28.0"
 typer = { extras = ["all"], version = "^0.6.1" }
+dtyper = "^2.1.0"
 pyhumps = "^3.7.3"
 cachetools = "^5.2.0"
 dictdiffer = "^0.9.0"
 python-schema-registry-client = "^2.4.1"
+httpx = "^0.24.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
 pytest-timeout = "^2.1.0"
 snapshottest = "^0.6.0"
-responses = "^0.22.0"
 pre-commit = "^2.19.0"
 flake8 = "^4.0.1"
-black = "^22.3.0"
+black = "^23.7.0"
 isort = "^5.12.0"
 typer-cli = "^0.0.13"
 pyright = "^1.1.314"
 pytest-rerunfailures = "^11.1.2"
+pytest-httpx = "^0.22.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-macros-plugin = "^0.7.0"
 mkdocs-material = "^9.0.0"
```

### Comparing `kpops-1.3.2/PKG-INFO` & `kpops-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.3.2
+Version: 1.4.0
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
@@ -20,18 +20,19 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
+Requires-Dist: dtyper (>=2.1.0,<3.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.8,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.3,<4.0.0)
 Requires-Dist: python-schema-registry-client (>=2.4.1,<3.0.0)
-Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
 Project-URL: Documentation, https://bakdata.github.io/kpops/latest
 Project-URL: Repository, https://github.com/bakdata/kpops
 Description-Content-Type: text/markdown
 
 # KPOps
```

