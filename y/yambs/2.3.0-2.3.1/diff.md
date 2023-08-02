# Comparing `tmp/yambs-2.3.0.tar.gz` & `tmp/yambs-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-2.3.0.tar", last modified: Mon Jul 31 05:26:30 2023, max compression
+gzip compressed data, was "yambs-2.3.1.tar", last modified: Wed Aug  2 05:17:06 2023, max compression
```

## Comparing `yambs-2.3.0.tar` & `yambs-2.3.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 05:25:07.000000 yambs-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-31 05:26:30.878316 yambs-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-31 05:25:07.000000 yambs-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-31 05:25:07.000000 yambs-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 05:26:30.878316 yambs-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:25:07.000000 yambs-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.866316 yambs-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-31 05:25:07.000000 yambs-2.3.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 05:25:07.000000 yambs-2.3.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.866316 yambs-2.3.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Dependency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Github.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/yambs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dependency/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dependency/handlers/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/yambs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/yambs/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.366245 yambs-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 05:15:13.000000 yambs-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-02 05:17:06.366245 yambs-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-08-02 05:15:13.000000 yambs-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 05:15:13.000000 yambs-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 05:17:06.366245 yambs-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-02 05:15:13.000000 yambs-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.346245 yambs-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-02 05:15:13.000000 yambs-2.3.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 05:15:13.000000 yambs-2.3.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.350245 yambs-2.3.1/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.350245 yambs-2.3.1/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.354245 yambs-2.3.1/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.354245 yambs-2.3.1/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.354245 yambs-2.3.1/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.354245 yambs-2.3.1/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.358245 yambs-2.3.1/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.362245 yambs-2.3.1/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.362245 yambs-2.3.1/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.362245 yambs-2.3.1/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/handlers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.362245 yambs-2.3.1/yambs/dependency/handlers/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/handlers/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/handlers/yambs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/handlers/yambs/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.362245 yambs-2.3.1/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.362245 yambs-2.3.1/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.366245 yambs-2.3.1/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.366245 yambs-2.3.1/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.366245 yambs-2.3.1/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.366245 yambs-2.3.1/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.366245 yambs-2.3.1/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-08-02 05:15:13.000000 yambs-2.3.1/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:17:06.350245 yambs-2.3.1/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-02 05:17:06.000000 yambs-2.3.1/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-02 05:17:06.000000 yambs-2.3.1/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:17:06.000000 yambs-2.3.1/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 05:17:06.000000 yambs-2.3.1/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-02 05:17:06.000000 yambs-2.3.1/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 05:17:06.000000 yambs-2.3.1/yambs.egg-info/top_level.txt
```

### Comparing `yambs-2.3.0/LICENSE` & `yambs-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/PKG-INFO` & `yambs-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.3.0
+Version: 2.3.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=da0d2fd90a670c981a7628b6eb8a2c87
+    hash=3fc032cf4d97e362f8c12b3c9d721ddc
     =====================================
 -->
 
-# yambs ([2.3.0](https://pypi.org/project/yambs/))
+# yambs ([2.3.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.3.0/README.md` & `yambs-2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=da0d2fd90a670c981a7628b6eb8a2c87
+    hash=3fc032cf4d97e362f8c12b3c9d721ddc
     =====================================
 -->
 
-# yambs ([2.3.0](https://pypi.org/project/yambs/))
+# yambs ([2.3.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.3.0/pyproject.toml` & `yambs-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "2.3.0"
+version = "2.3.1"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-2.3.0/setup.py` & `yambs-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/tests/test_entry.py` & `yambs-2.3.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/aggregation/__init__.py` & `yambs-2.3.1/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/app.py` & `yambs-2.3.1/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/commands/all.py` & `yambs-2.3.1/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/commands/common.py` & `yambs-2.3.1/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/commands/dist.py` & `yambs-2.3.1/yambs/commands/dist.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/commands/gen.py` & `yambs-2.3.1/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/commands/native.py` & `yambs-2.3.1/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/commands/uf2conv.py` & `yambs-2.3.1/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/config/__init__.py` & `yambs-2.3.1/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/config/board.py` & `yambs-2.3.1/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/config/common.py` & `yambs-2.3.1/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/includes/chips.yaml` & `yambs-2.3.1/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/includes/infineon.yaml` & `yambs-2.3.1/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/includes/microchip.yaml` & `yambs-2.3.1/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/native.yaml` & `yambs-2.3.1/yambs/data/native.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 cflag_groups:
   # Compile position-independent to build shared objects.
   pic: [-fPIC]
 
   # Instrument builds for coverage and other analysis.
   debug: [-Og, -g, --coverage]
-  opt: [-O2]
+  opt: [-O2, -s]
   asan: [-fsanitize=address]
   msan: [-fsanitize=memory]
 
 variants:
 
   debug:
     cflag_groups: [asan]
```

### Comparing `yambs-2.3.0/yambs/data/schemas/Chip.yaml` & `yambs-2.3.1/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/schemas/Config.yaml` & `yambs-2.3.1/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/schemas/Native.yaml` & `yambs-2.3.1/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/schemas/config_common.yaml` & `yambs-2.3.1/yambs/data/schemas/config_common.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/templates/native_rules.ninja.j2` & `yambs-2.3.1/yambs/data/templates/native_rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/templates/rules.ninja.j2` & `yambs-2.3.1/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/data/uf2families.json` & `yambs-2.3.1/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/config.py` & `yambs-2.3.1/yambs/dependency/config.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/github.py` & `yambs-2.3.1/yambs/dependency/github.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/handlers/types.py` & `yambs-2.3.1/yambs/dependency/handlers/types.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/handlers/yambs/__init__.py` & `yambs-2.3.1/yambs/dependency/handlers/yambs/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/handlers/yambs/config.py` & `yambs-2.3.1/yambs/dependency/handlers/yambs/config.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/handlers/yambs/github.py` & `yambs-2.3.1/yambs/dependency/handlers/yambs/github.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dependency/manager.py` & `yambs-2.3.1/yambs/dependency/manager.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/dist/__init__.py` & `yambs-2.3.1/yambs/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/entry.py` & `yambs-2.3.1/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/environment/__init__.py` & `yambs-2.3.1/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/environment/native.py` & `yambs-2.3.1/yambs/environment/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/__init__.py` & `yambs-2.3.1/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/architectures.py` & `yambs-2.3.1/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/boards.py` & `yambs-2.3.1/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/chips.py` & `yambs-2.3.1/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/common.py` & `yambs-2.3.1/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/ninja/__init__.py` & `yambs-2.3.1/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/ninja/format.py` & `yambs-2.3.1/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/toolchains.py` & `yambs-2.3.1/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/generate/variants.py` & `yambs-2.3.1/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/github/__init__.py` & `yambs-2.3.1/yambs/github/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/schemas.py` & `yambs-2.3.1/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/translation/__init__.py` & `yambs-2.3.1/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs/uf2/__init__.py` & `yambs-2.3.1/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.0/yambs.egg-info/PKG-INFO` & `yambs-2.3.1/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.3.0
+Version: 2.3.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=da0d2fd90a670c981a7628b6eb8a2c87
+    hash=3fc032cf4d97e362f8c12b3c9d721ddc
     =====================================
 -->
 
-# yambs ([2.3.0](https://pypi.org/project/yambs/))
+# yambs ([2.3.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.3.0/yambs.egg-info/SOURCES.txt` & `yambs-2.3.1/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

