# Comparing `tmp/seqslab-cli-3.2.2.tar.gz` & `tmp/seqslab-cli-3.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-cli-3.2.2.tar", last modified: Wed Aug  2 11:15:01 2023, max compression
+gzip compressed data, was "seqslab-cli-3.2.2a0.tar", last modified: Tue Jul 18 06:57:32 2023, max compression
```

## Comparing `seqslab-cli-3.2.2.tar` & `seqslab-cli-3.2.2a0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.892976 seqslab-cli-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-08-02 11:15:01.892976 seqslab-cli-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.876975 seqslab-cli-3.2.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/auth/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/drs/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/drs/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/api/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/api/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/drs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/drs/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/drs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/organization/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/organization/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/organization/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/role/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/role/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/role/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.884976 seqslab-cli-3.2.2/python/seqslab/runsheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/runsheet/runsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/session_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/statusbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/trs/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/trs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/trs/register/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/register/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/register/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/register/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/trs/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/trs/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/trs/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/usage_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/user/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/user/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/wes/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/wes/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/wes/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/wes/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/wes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.888976 seqslab-cli-3.2.2/python/seqslab/workspace/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.892976 seqslab-cli-3.2.2/python/seqslab/workspace/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:15:01.892976 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:15:01.000000 seqslab-cli-3.2.2/python/seqslab_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-02 11:15:01.892976 seqslab-cli-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-02 11:14:47.000000 seqslab-cli-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.270305 seqslab-cli-3.2.2a0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.274305 seqslab-cli-3.2.2a0/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.274305 seqslab-cli-3.2.2a0/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/runsheet/runsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-18 06:57:32.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/setup.py
```

### Comparing `seqslab-cli-3.2.2/LICENSE` & `seqslab-cli-3.2.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/PKG-INFO` & `seqslab-cli-3.2.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.2.2
+Version: 3.2.2a0
 Summary: Atgenomix SeqsLab Command Line Tool
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.2 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.2a0 Summary: Atgenomix
 SeqsLab Command Line Tool Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang Author-email: allen.chang@atgenomix.com License: Apache
 License, Version 2.0 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli Description:
 This package provides a unified command line interface to Atgenomix SeqsLab, a
 cloud-native biomedical informatics (BioMed IT) platform.   Table of Contents
    1. Getting_Started
```

### Comparing `seqslab-cli-3.2.2/README.md` & `seqslab-cli-3.2.2a0/README.md`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/__init__.py` & `seqslab-cli-3.2.2a0/python/seqslab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 name = "seqslab"
 
 __all__ = [
 
 ]
 
 
-__version__ = "3.2.2"
+__version__ = "3.2.2a0"
 
 LOGGING = {
     "DIR_PATH": "/var/log/seqslab"
 }
```

### Comparing `seqslab-cli-3.2.2/python/seqslab/auth/azuread.py` & `seqslab-cli-3.2.2a0/python/seqslab/auth/azuread.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/auth/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/auth/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/cli.py` & `seqslab-cli-3.2.2a0/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/context.py` & `seqslab-cli-3.2.2a0/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/api/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/api/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,23 +211,20 @@
 
     def folder_blob(self, stdin: List[dict], **kwargs) -> List[dict]:
         checksums = []
         sizes = []
         dsts_list = []
         access_method_infos = []
         created_times = []
-        is_integrity = True
 
         for i, v in enumerate(stdin):
-            if is_integrity:
-                if 'checksums' in v.keys() and len(v.get('checksums')) > 0:
-                    checksums.append(v.get('checksums')[0].get('checksum'))
-                else:
-                    print(f"WARNING: Index {i}, has no checksums.")
-                    is_integrity = False
+            if 'checksums' in v.keys():
+                checksums.append(v.get('checksums')[0].get('checksum'))
+            else:
+                raise ValueError(f'Index {i}, has no checksums.')
             sizes.append(v.get('size'))
             if 'access_methods' in v.keys():
                 # initialize
                 if len(dsts_list) == 0:
                     for access_method in v['access_methods']:
                         if "access_url" in access_method.keys():
                             if 'url' in access_method['access_url']:
@@ -240,19 +237,16 @@
                     dsts_list=dsts_list, access_methods=v.get('access_methods'),
                     access_method_infos=access_method_infos, index=i)
             else:
                 raise ValueError(f'Index {i}, has no access_methods.')
             created_times.append(v.get('created_time'))
 
         folder_stdin = stdin[0].copy()
-        if is_integrity:
-            folder_stdin['checksums'][0]['checksum_type'] = kwargs.get('checksum_type', "sha256")
-            folder_stdin['checksums'][0]['checksum'] = kwargs.get('checksum', self.concat_checksum(checksums=checksums))
-        else:
-            folder_stdin['checksums'] = []
+        folder_stdin['checksums'][0]['checksum_type'] = kwargs.get('checksum_type', "sha256")
+        folder_stdin['checksums'][0]['checksum'] = kwargs.get('checksum', self.concat_checksum(checksums=checksums))
         folder_stdin['size'] = kwargs.get('size', self.sum_fsize(sizes=sizes))
         folder_stdin['created_time'] = kwargs.get('created_time', self.min_time(times=created_times))
         folder_stdin['mime_type'] = kwargs.get('mime_type', "directory")
         folder_stdin['file_type'] = kwargs.get('file_type', "directory")
         folder_stdin['description'] = kwargs.get('description', folder_stdin['description'])
         folder_stdin['aliases'] = kwargs.get('aliases', folder_stdin['aliases'])
         folder_stdin['metadata'] = json.loads(kwargs.get('metadata')) if "metadata" in kwargs else folder_stdin['metadata']
```

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/api/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/api/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
                 raise ValueError(f'{name}: Make sure the size can not be smaller than 0')
             common["created_time"] = self.time(created_time)
             if not common["created_time"]:
                 raise ValueError(f'{name}: Make sure the time is exist and the format must in RFC3339')
             if kwargs.get("updated_time"):
                 common["updated_time"] = self.time(kwargs.get("updated_time"))
             common["checksums"] = self.checksums(checksums=checksums)
+            if not common["checksums"]:
+                raise ValueError(f'{name}: Make sure the checksum format is correct.')
         return common
 
     @staticmethod
     def contents(contents: list) -> List[dict]:
         return [{"drs_id":id} for id in contents]
 
     @staticmethod
@@ -104,16 +106,14 @@
             r'(?P<tzinfo>Z|[+-]\d{2}(?::?\d{2})?)?$'
         )
         if datetime_re.match(time) is not None:
             return time
 
     @staticmethod
     def checksums(checksums: List[dict]) -> list:
-        if not checksums:
-            return []
         for checksum in checksums:
             try:
                 int(checksum.get('checksum'), 16)
                 if not checksum.get('type') and checksum.get('checksum_type'):
                     checksum['type'] = checksum['checksum_type']
                     checksum.pop('checksum_type')
                 return checksums
```

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -459,55 +459,40 @@
 
         def __log(results: List[dict], output: str):
             self._stdout(results=results, output=output)
             for r in results:
                 msg = f"Register {r['id']}  is complete."
                 logging.info(msg)
 
-        if not stdin:
-            if kwargs.get('checksum', None) and kwargs.get('checksum_type', None):
-                kwargs['is_integrity'] = True
-            elif not kwargs.get('checksum', None) and not kwargs.get('checksum_type', None):
-                kwargs['is_integrity'] = False
-                cprint("WARNING: DRS objects registered without checksums will not undergo integrity checks "
-                       "during future DRS objects retrieval.")
-            else:
-                cprint('Give both checksum and checksum_type arguments to register the DRS object with checksum '
-                       'for integrity check, otherwise drop both arguments to register the DRS object without '
-                       'checksum', 'red')
-                return errno.EINVAL
-
         results = self._register_blob(drs_type=type, stdin=stdin, workspace=workspace, **kwargs)
         if isinstance(results, int):
             return results
         __log(results=results, output=output)
         return 0
 
     @staticmethod
     @exception_handler
     def _register_blob(drs_type: str, stdin: bool, workspace: str, **kwargs) -> List[dict]:
         backend = drs_register().load_register(workspace)
         if stdin:
             payloads = backend.create_payload(stdin=BaseDatahub._stdin(), type=drs_type, **kwargs)
         else:
-            if not kwargs['is_integrity']:
-                checksums = []
-            else:
-                checksums = [{"checksum": kwargs.get('checksum'), "checksum_type": kwargs.get('checksum_type')}]
-
             payloads = [{
                 "name": kwargs.get('name'),
                 "mime_type": kwargs.get('mime_type'),
                 "file_type": kwargs.get('file_type'),
                 "created_time": kwargs.get('created_time'),
                 "updated_time": kwargs.get('updated_time') if kwargs.get('updated_time') else kwargs.get(
                     'created_time'),
                 "size": kwargs.get('size'),
                 "access_methods":  json.loads(kwargs.get('access_methods')),
-                "checksums": checksums,
+                "checksums": [{
+                    "checksum": kwargs.get('checksum'),
+                    "checksum_type": kwargs.get('checksum_type'),
+                }],
                 "description": kwargs.get('description'),
                 "aliases": kwargs.get('aliases'),
                 "metadata": json.loads(kwargs.get('metadata')) if kwargs.get('metadata') else None,
                 "tags": kwargs.get('tags'),
                 "id": kwargs.get('id')
             }]
 
@@ -594,15 +579,15 @@
                 "contents": drs_ids
             }]
 
         results = backend.create_drsobjects(drs_type='bundle', payloads=payloads)
 
         return results
 
-    @command(aliases=["deregister"])
+    @command(aliases=["unregister"])
     @argument("ids",
               type=List[str],
               positional=False,
               description="Specify the IDs of the DRS objects that you want to delete "
                           "(optional).")
     @argument("names",
               type=List[str],
@@ -610,22 +595,22 @@
               description="Specify the names of the DRS objects that you want to delete "
                           "(optional).")
     @argument("tags",
               type=List[str],
               positional=False,
               description="Specify the labels of the DRS objects that you want to delete "
                           "(optional).")
-    def deregister(
+    def unregister(
             self,
             ids: List[str] = [],
             tags: List[str] = [],
             names: List[str] = [],
     ) -> int:
         """
-        Deregister DRS objects by DRS ID, DRS name, or DRS tag.
+        Unregister DRS objects by DRS ID, DRS name, or DRS tag.
         """
         if not ids and not names and not tags:
             cprint("Must specify one of the IDs, names or tags to identify DRS objects for deletion", "red")
             return errno.ENOENT
 
         resps = asyncio.run(utils.drs_delete(ids, names, tags, query_opts=f"?backend_content=false"))
         for r in resps:
```

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/internal/aiocopy.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/internal/aiocopy.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/internal/utils.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/storage/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/storage/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/utils/biomimetype.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/drs/utils/progressbar.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/exceptions.py` & `seqslab-cli-3.2.2a0/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/organization/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/organization/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/plugin.py` & `seqslab-cli-3.2.2a0/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/role/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/role/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/role/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/role/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/runsheet/runsheet.py` & `seqslab-cli-3.2.2a0/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/settings.py` & `seqslab-cli-3.2.2a0/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/statusbar.py` & `seqslab-cli-3.2.2a0/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/internal/utils.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/register/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/register/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/register/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/register/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/resource/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/template/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/trs/template/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/usage_logger.py` & `seqslab-cli-3.2.2a0/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/user/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/user/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/user/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/user/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/template/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/template/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/wes/utils.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/workspace/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/workspace/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/workspace/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab/workspace/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/python/seqslab_cli.egg-info/PKG-INFO` & `seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.2.2
+Version: 3.2.2a0
 Summary: Atgenomix SeqsLab Command Line Tool
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.2 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.2a0 Summary: Atgenomix
 SeqsLab Command Line Tool Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang Author-email: allen.chang@atgenomix.com License: Apache
 License, Version 2.0 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli Description:
 This package provides a unified command line interface to Atgenomix SeqsLab, a
 cloud-native biomedical informatics (BioMed IT) platform.   Table of Contents
    1. Getting_Started
```

### Comparing `seqslab-cli-3.2.2/python/seqslab_cli.egg-info/SOURCES.txt` & `seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.2/setup.py` & `seqslab-cli-3.2.2a0/setup.py`

 * *Files identical despite different names*

