# Comparing `tmp/neo3-boa-1.0.0.tar.gz` & `tmp/neo3-boa-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo3-boa-1.0.0.tar", last modified: Mon Jul 10 19:49:54 2023, max compression
+gzip compressed data, was "neo3-boa-1.0.1.tar", last modified: Wed Aug  2 16:37:58 2023, max compression
```

## Comparing `neo3-boa-1.0.0.tar` & `neo3-boa-1.0.1.tar`

### file list

```diff
@@ -1,820 +1,821 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.163769 neo3-boa-1.0.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4521 2023-07-10 19:49:54.163769 neo3-boa-1.0.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3047 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2313 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/boa3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/compile_time/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13554 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/compile_time/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5804 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/contract/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      435 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/blockchain/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10773 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/blockchain/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/blockchain/block.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1965 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/blockchain/signer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1531 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/blockchain/transaction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/blockchain/vmstate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6174 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/contract/callflagstype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1071 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/contract/contract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6750 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/contract/contractmanifest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/crypto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5095 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/crypto/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/crypto/namedcurve.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/iterator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/iterator/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/json/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      960 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/json/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/oracle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      199 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/oracle/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/oracle/oracleresponsecode.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3/builtin/interop/policy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1230 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/policy/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/interop/role/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      543 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/role/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/role/roletype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/interop/runtime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6715 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/runtime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/runtime/notification.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/runtime/triggertype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/interop/stdlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5564 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/stdlib/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/interop/storage/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3240 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/storage/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/storage/findoptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1055 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/storage/storagecontext.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1379 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/interop/storage/storagemap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1154 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/math.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/nativecontract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6777 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/contractmanagement.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3175 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/cryptolib.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3409 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/gas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9158 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/ledger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8874 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/neo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2291 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/oracle.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1679 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/policy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/rolemanagement.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7876 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/nativecontract/stdlib.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2733 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/type/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      795 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/type/helper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/builtin/vm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/builtin/vm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/cpm.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/internal/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.087769 neo3-boa-1.0.0/boa3/internal/analyser/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10820 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/analyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11125 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/astanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17364 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/astoptimizer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4737 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/builtinfunctioncallanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3047 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/constructanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10840 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/importanalyser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/analyser/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/model/ManifestSymbol.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/model/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/model/functionarguments.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/analyser/model/optimizer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/model/optimizer/Operation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3056 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/model/optimizer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1517 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/model/symbolscope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    65411 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/moduleanalyser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/analyser/supportedstandard/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      292 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/supportedstandard/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8135 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/supportedstandard/standardanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    82772 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/analyser/typeanalyser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/cli_commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/cli_commands/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3765 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/cli_commands/compile_command.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/cli_commands/icommand.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/compiler/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      883 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    89916 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/codegenerator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    51813 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/codegeneratorvisitor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1663 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/generatordata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4244 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/initstatementsvisitor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3350 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/methodtokencollection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3602 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/stackmemento.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/variablegenerationdata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6725 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/vmcodemap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11037 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/vmcodemapping.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3244 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/compiledmetadata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7451 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/compiler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/compileroutput.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/compiler/filegenerator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/filegenerator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35047 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/filegenerator/filegenerator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      925 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/compiler/filegenerator/importdata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1752 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      489 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/env.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/exception/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13198 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/exception/CompilerError.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4250 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/exception/CompilerWarning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/exception/InvalidPathException.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      334 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/exception/NotLoadedException.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/exception/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.091769 neo3-boa-1.0.0/boa3/internal/helpers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/helpers/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.095769 neo3-boa-1.0.0/boa3/internal/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1705 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/attribute.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.095769 neo3-boa-1.0.0/boa3/internal/model/builtin/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11741 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/builtin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1685 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/builtincallable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/builtinproperty.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      514 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/builtinsymbol.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.099769 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2773 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2816 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/appendmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2372 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/clearmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2652 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/copydictmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      389 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/copylistmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2631 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/copymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3724 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7709 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countsequencegenericmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5683 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countsequencemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countsequenceprimitivemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9111 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countstrmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3659 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/extendmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8497 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/indexbytesstringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2604 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/indexmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8292 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/indexsequencemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4116 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/insertmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6949 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/isdigitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6241 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/joinmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6649 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/lowermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1849 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/mapkeysmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1859 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/mapvaluesmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2652 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popdictdefaultmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      643 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popdictmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3822 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      800 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popsequencemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3095 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/removemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1726 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/reversemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7883 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/startswithmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10401 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/stripmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6650 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/uppermethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.099769 neo3-boa-1.0.0/boa3/internal/model/builtin/compile_time/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/compile_time/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/compile_time/neometadatatype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.099769 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/abortmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3166 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/neoaccountstatetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      854 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/nep11transferevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/nep17transferevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      567 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/contract/nep5transferevent.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.099769 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      999 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      814 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/builtindecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1367 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/classmethoddecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2817 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/contractdecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3441 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/displaynamedecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      352 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/instancemethoddecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/metadatadecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1467 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/propertydecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3203 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/publicdecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      232 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/staticmethoddecorator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.103769 neo3-boa-1.0.0/boa3/internal/model/builtin/internal/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      238 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/internal/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2038 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/internal/getenvmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/internal/innerdeploymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/internal/internalmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.103769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.103769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2484 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4020 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/blocktype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/currenthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      730 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/currentindexmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      800 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/getblockmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/getcontractmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionfromblockmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionheightmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      745 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionsignersmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionvmstatemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3636 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/signertype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3854 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/transactiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/vmstatetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessconditionenumtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3045 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessconditiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1652 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessruleactiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3264 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessruletype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1587 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessscopeenumtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.107769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1496 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1754 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/callflagstype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2049 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/callmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.107769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1521 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractabitype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1951 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1755 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractgrouptype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2236 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1905 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparametertype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2009 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1741 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3375 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contracttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      883 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/createmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      821 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/createmultisigaccountmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      698 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/createstandardaccountmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/destroymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      543 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getcallflagsmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getgasscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getminimumdeploymentfeemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getneoscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/updatemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1167 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contractgethashmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.107769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1061 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/checkmultisigmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      974 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/checksigmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1262 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/hash160method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1258 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/hash256method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/murmur32method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1614 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/namedcurvetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/ripemd160method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      489 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/sha256method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/verifywithecdsa.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18175 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interopevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interopinterfacetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1762 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interopmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.107769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      231 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1855 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/getiteratorvalue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1520 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/iteratorinitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/iteratornextmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2828 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/iteratortype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.107769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/json/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/json/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/json/jsondeserializemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/json/jsonserializemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      749 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1068 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Ledger/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Ledger/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Ledger/ledgermethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Neo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Neo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Neo/getneoscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Neo/neocontractmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Nep17/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Nep17/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1108 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Nep17/getnep17scripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      875 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Nep17/nep17method.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Oracle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Oracle/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1030 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Oracle/oraclemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1070 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      803 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1074 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/StdLib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/StdLib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1033 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      506 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5055 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/nativecontractmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.111769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/oraclegetpricemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1043 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/oraclerequestmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1742 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/oracleresponsecodetype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.115769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      532 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      506 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/getexecfeefactormethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/getfeeperbytemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/getstoragepricemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/isblockedmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.115769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/role/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      252 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/role/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      822 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/role/getdesignatedbyrolemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1555 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/role/roletype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.115769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2551 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      483 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/burngasmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/checkwitnessmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getaddressversionmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      715 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getblocktimemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getcallingscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getentryscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      839 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getexecutingscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      717 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getgasleftmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      780 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getinvocationcountermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      466 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getnetworkmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2238 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getnotificationsmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getplatformmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getrandommethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      522 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/gettriggermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1693 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/loadscriptmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/logmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3152 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/notificationtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/notifymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/scriptcontainermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1784 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/triggertype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.119769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1528 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/atoimethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base58checkdecodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base58checkencodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base58decodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base58encodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base64decodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base64encodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      500 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/deserializemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/itoamethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/memorycomparemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1217 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/memorysearchmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/serializemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.119769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1184 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/findoptionstype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.119769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      581 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1270 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2188 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontexttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2916 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagedeletemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4441 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagefindmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      601 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagegetcontextmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3412 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagegetmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagegetreadonlycontextmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.119769 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1326 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1318 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemapgetmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1631 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemapputmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4029 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemaptype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3282 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storageputmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.119769 neo3-boa-1.0.0/boa3/internal/model/builtin/math/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      418 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/math/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2625 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/math/decimalceil.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2590 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/math/decimalfloor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/math/powmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      755 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/math/sqrtmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.127769 neo3-boa-1.0.0/boa3/internal/model/builtin/method/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3698 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/absmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4429 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/boolmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      949 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/builtinevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6600 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/builtinmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      733 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/bytearrayencodingmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3780 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/bytearraymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/createeventmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3300 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/ecpointmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1848 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/ecpointtoscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2407 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/exceptionmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/exitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19709 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/intbytestringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      710 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/intintmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1585 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/intmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5585 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/isinstancemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1766 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/lenmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2535 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/listbytesstringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5630 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/listgenericmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      993 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/listmappingmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3490 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/listmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1091 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/listsequencemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4451 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/maxbytestringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      377 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/maxintmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5942 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/maxmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4455 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/minbytestringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      377 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/minintmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5896 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/minmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      749 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/printboolmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/printbytestringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/printclassmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/printintmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4822 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/printmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/printsequencemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4349 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/rangemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4970 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/reversedmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1614 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/strboolmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/strbytestringmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      633 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/strintmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1572 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/strmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4281 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/strsplitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/summethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1563 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/supermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2550 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/toboolmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4813 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/tobytesmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2537 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/tointmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5221 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/toscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2537 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/tostrmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4832 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/uint160method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4832 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/method/uint256method.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.127769 neo3-boa-1.0.0/boa3/internal/model/builtin/native/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.127769 neo3-boa-1.0.0/boa3/internal/model/builtin/native/contract_management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      125 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/contract_management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/contract_management/hasmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1566 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/contractmanagementclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/cryptolibclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1484 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/gasclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1392 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/inativecontractclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1517 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/ledgerclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2454 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nativecontract.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.131769 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1730 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getaccountstatemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      825 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getallcandidatesmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      783 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatesmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatevotemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getcommitteemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      495 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getgasperblockmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getnextblockvalidators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/registercandidatemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/unclaimedgasmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/unregistercandidatemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/unvote.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/vote.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3024 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/neoclass.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.131769 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/balanceofmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      525 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/decimalsmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/symbolmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/totalsupplymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1004 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/transfermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/oracleclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1280 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/policyclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/rolemanagementclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/builtin/native/stdlibclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7112 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/callable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/debuginstruction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1139 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/decorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1308 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/event.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      823 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/expression.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      833 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/identifiedsymbol.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.131769 neo3-boa-1.0.0/boa3/internal/model/imports/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/imports/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6500 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/imports/builtin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2849 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/imports/importsymbol.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4942 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/imports/package.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5833 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4285 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/module.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.131769 neo3-boa-1.0.0/boa3/internal/model/operation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.131769 neo3-boa-1.0.0/boa3/internal/model/operation/binary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.131769 neo3-boa-1.0.0/boa3/internal/model/operation/binary/additional/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/additional/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5881 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/additional/membership.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/additional/notmembership.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.135769 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1556 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/addition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2253 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/concat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1456 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/division.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/floordivision.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/listaddition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2827 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/modulo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1568 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/multiplication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1478 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/power.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2475 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/strbytesmultiplication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/subtraction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/binaryoperation.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.135769 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/booleanand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/booleanor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1525 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/leftshift.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1497 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/logicand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/logicor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1497 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/logicxor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1529 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/rightshift.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.135769 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1182 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1505 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/greaterthan.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/greaterthanorequal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/identity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/lessthan.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1516 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/lessthanorequal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1377 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/notidentity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1512 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/numericequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/numericinequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/objectequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1603 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/objectinequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4190 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/binaryop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3286 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/operation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2300 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/operator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.135769 neo3-boa-1.0.0/boa3/internal/model/operation/unary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      453 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1320 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/booleannot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1336 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/logicnot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/negative.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1606 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/noneidentity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/nonenotidentity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1390 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/positive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1485 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unary/unaryoperation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1973 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/operation/unaryop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      928 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/property.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.135769 neo3-boa-1.0.0/boa3/internal/model/standards/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/standards/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2243 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/standards/neostandard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2469 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/standards/nep11standard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1435 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/standards/nep17standard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/standards/standardmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      322 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/symbol.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.139769 neo3-boa-1.0.0/boa3/internal/model/type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.139769 neo3-boa-1.0.0/boa3/internal/model/type/annotation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/annotation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/annotation/metatype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1710 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/annotation/optionaltype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4093 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/annotation/uniontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      843 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/anytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      639 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/baseexceptiontype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.139769 neo3-boa-1.0.0/boa3/internal/model/type/classes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/classarraytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1587 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/classinitmethoddefault.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      119 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/classscope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/classstructtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8647 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/classtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1202 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/contractinterfaceclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1035 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/contractinterfacehash.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4631 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/pythonclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5768 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/classes/userclass.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.139769 neo3-boa-1.0.0/boa3/internal/model/type/collection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1470 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/genericcollectiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6127 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/icollection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.139769 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      892 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/genericmappingtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4114 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mappingtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.139769 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mutable/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mutable/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1347 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mutable/dicttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mutable/mutablemappingtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      627 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/buffertype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/ecpointtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1128 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/genericsequencetype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1186 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/genericmutablesequencetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1709 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/listtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1433 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/mutablesequencetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1412 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/rangetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1498 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/reversedtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1513 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/sequencetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1353 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/tupletype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1851 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/uint160type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1927 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/uint256type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5319 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/itype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1119 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/math.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/model/type/neo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/addresstype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/blockhashtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1699 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/opcodetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/publickeytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      622 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/scripthashlittleendiantype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      550 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/scripthashtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/neo/transactionidtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/model/type/primitive/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1209 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/booltype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/bytearraytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/bytestringtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1042 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/bytestype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1908 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/ibytestringtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1246 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/inttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1005 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/nonetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      193 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/primitivetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1733 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/primitive/strtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4639 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1874 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/typeutils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/model/type/typingmethod/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/typingmethod/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4456 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/type/typingmethod/casttypemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1759 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/model/variable.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/neo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2541 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/neo/contracts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       98 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/contracts/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2016 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/contracts/neffile.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.143769 neo3-boa-1.0.0/boa3/internal/neo/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/core/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/core/types/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/core/types/InteropInterface.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/core/types/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/cryptography/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      603 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/cryptography/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/smart_contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/smart_contract/VoidType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/smart_contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2267 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/smart_contract/notification.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4096 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/utils/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/vm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/CallCode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3476 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/TryCode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3284 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/VMCode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29012 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/Opcode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10557 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/OpcodeHelper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27309 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/OpcodeInfo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1209 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/OpcodeInformation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo/vm/type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1780 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/type/AbiType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/type/ContractParameterType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/type/Integer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2516 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/type/StackItem.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/type/String.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo/vm/type/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo3/contracts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2843 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/contracttypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1555 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/findoptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/namedcurve.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo3/contracts/native/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/native/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/native/nativetypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9076 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/contracts/nef.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo3/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/core/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23279 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/core/serialization.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.147769 neo3-boa-1.0.0/boa3/internal/neo3/core/types/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/core/types/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4432 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/core/types/biginteger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8211 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/core/types/uint.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/core/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3/internal/neo3/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/network/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3/internal/neo3/network/payloads/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      120 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/network/payloads/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1468 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/network/payloads/oracleresponsecode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/network/payloads/verification.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3/internal/neo3/vm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       29 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/vm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3/internal/neo3/vm/vmstate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.083769 neo3-boa-1.0.0/boa3_test/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/interface/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/interface/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1156 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/interface/itransactionobject.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/invokeresult.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2245 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neobatchinvoke.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1741 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neoinvoke.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2429 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neoinvokecollection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1915 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neoinvokeresult.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2165 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/signer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1898 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/testblock.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4483 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/testtransaction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      968 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/witness.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1200 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/witnessscope.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5316 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/contractcollection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2733 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/testcontract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/triggertype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/model/wallet/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/wallet/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1977 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/wallet/account.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      530 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/model/wallet/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       45 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8723 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/batch.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.151769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/batch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/batch/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/create.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      434 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/icheckpointcommand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/restore.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1727 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/deploy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/icontractcommand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/invoke.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      577 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/run.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/create/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1227 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/create/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/fastforward/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      948 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/fastforward/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/neoexpresscommand.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/reset/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      944 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/reset/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1041 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/block.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/ishowcommand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      694 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/transaction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/transfer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1414 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/transfer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1218 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoxp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoxp_contract.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/utils/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/model/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      969 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/model/neoxpaccount.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3326 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/model/neoxpconfig.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8510 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/neoxp/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.155769 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.159769 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/block.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/contract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1460 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/notification.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4193 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/storage.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/storagecollection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/transaction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      934 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/transactionlog.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19143 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/neo_test_runner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/testrunner/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      335 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/test_drive/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.159769 neo3-boa-1.0.0/boa3_test/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16870 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/boa_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2360 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/run_unit_tests.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.159769 neo3-boa-1.0.0/boa3_test/tests/test_classes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/TestExecutionException.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.159769 neo3-boa-1.0.0/boa3_test/tests/test_classes/binaryserializer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1974 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/binaryserializer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1699 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/block.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.159769 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1198 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neoabistruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neoeventstruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1746 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neomanifeststruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1174 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neomethodstruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1423 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neopermissionsstruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      975 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neostruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1558 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/contractcollection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/nativeaccountstate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/nativecontractprefix.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2542 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/signer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6453 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/storage.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3160 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/testcontract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2412 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/transaction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.159769 neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2202 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      681 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/transactionattributetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_classes/witness.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3044 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/boa3_test/tests/test_suite.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-10 19:49:54.163769 neo3-boa-1.0.0/neo3_boa.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4521 2023-07-10 19:49:54.000000 neo3-boa-1.0.0/neo3_boa.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37518 2023-07-10 19:49:54.000000 neo3-boa-1.0.0/neo3_boa.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-10 19:49:54.000000 neo3-boa-1.0.0/neo3_boa.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-07-10 19:49:54.000000 neo3-boa-1.0.0/neo3_boa.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-07-10 19:49:54.000000 neo3-boa-1.0.0/neo3_boa.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2023-07-10 19:49:54.000000 neo3-boa-1.0.0/neo3_boa.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      159 2023-07-10 19:49:54.163769 neo3-boa-1.0.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4985 2023-07-10 19:49:39.000000 neo3-boa-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.294289 neo3-boa-1.0.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4521 2023-08-02 16:37:58.294289 neo3-boa-1.0.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3047 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2313 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/boa3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/compile_time/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13554 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/compile_time/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5804 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/contract/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/interop/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      435 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/interop/blockchain/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10773 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/blockchain/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/blockchain/block.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1965 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/blockchain/signer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1531 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/blockchain/transaction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/blockchain/vmstate.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/interop/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6174 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/contract/callflagstype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1071 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/contract/contract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6750 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/contract/contractmanifest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/interop/crypto/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5095 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/crypto/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/crypto/namedcurve.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3/builtin/interop/iterator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/iterator/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/json/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      960 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/json/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/oracle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      199 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/oracle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/oracle/oracleresponsecode.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/policy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1230 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/policy/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/role/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      543 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/role/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/role/roletype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/runtime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6715 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/runtime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/runtime/notification.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/runtime/triggertype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/stdlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5564 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/stdlib/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/interop/storage/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3240 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/storage/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/storage/findoptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1055 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/storage/storagecontext.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1379 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/interop/storage/storagemap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1154 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/math.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/nativecontract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6777 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/contractmanagement.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3175 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/cryptolib.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3409 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/gas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9158 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/ledger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8874 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/neo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2291 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/oracle.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1679 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/policy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/rolemanagement.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7876 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/nativecontract/stdlib.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2733 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/type/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      795 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/type/helper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/builtin/vm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/builtin/vm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/cpm.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.210288 neo3-boa-1.0.1/boa3/internal/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/analyser/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10820 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/analyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11125 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/astanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17364 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/astoptimizer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4737 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/builtinfunctioncallanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3047 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/constructanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10840 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/importanalyser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/analyser/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/model/ManifestSymbol.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/model/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/model/functionarguments.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/analyser/model/optimizer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/model/optimizer/Operation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3056 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/model/optimizer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1517 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/model/symbolscope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    65944 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/moduleanalyser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/analyser/supportedstandard/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      292 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/supportedstandard/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8135 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/supportedstandard/standardanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    82772 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/analyser/typeanalyser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/cli_commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/cli_commands/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3765 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/cli_commands/compile_command.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/cli_commands/icommand.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/compiler/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.214288 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      883 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    89916 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/codegenerator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52138 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/codegeneratorvisitor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1663 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/generatordata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4244 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/initstatementsvisitor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3350 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/methodtokencollection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3602 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/stackmemento.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/variablegenerationdata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6725 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/vmcodemap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11037 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/vmcodemapping.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3244 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/compiledmetadata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7451 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/compiler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/compileroutput.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.218288 neo3-boa-1.0.1/boa3/internal/compiler/filegenerator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/filegenerator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35047 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/filegenerator/filegenerator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      925 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/compiler/filegenerator/importdata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1752 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      489 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/env.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.218288 neo3-boa-1.0.1/boa3/internal/exception/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13198 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/exception/CompilerError.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4250 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/exception/CompilerWarning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/exception/InvalidPathException.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      334 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/exception/NotLoadedException.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/exception/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.218288 neo3-boa-1.0.1/boa3/internal/helpers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/helpers/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.218288 neo3-boa-1.0.1/boa3/internal/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1705 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/attribute.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.218288 neo3-boa-1.0.1/boa3/internal/model/builtin/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11741 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/builtin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1685 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/builtincallable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/builtinproperty.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      514 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/builtinsymbol.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.222288 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2773 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2816 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/appendmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2372 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/clearmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2652 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/copydictmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      389 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/copylistmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2631 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/copymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3724 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7709 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countsequencegenericmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5683 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countsequencemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countsequenceprimitivemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9111 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countstrmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3659 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/extendmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8497 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/indexbytesstringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2604 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/indexmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8292 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/indexsequencemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4116 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/insertmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6949 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/isdigitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6241 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/joinmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6649 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/lowermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1849 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/mapkeysmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1859 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/mapvaluesmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2652 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popdictdefaultmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      643 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popdictmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3822 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      800 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popsequencemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3095 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/removemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1726 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/reversemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7883 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/startswithmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10401 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/stripmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6650 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/uppermethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.222288 neo3-boa-1.0.1/boa3/internal/model/builtin/compile_time/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/compile_time/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/compile_time/neometadatatype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.222288 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/abortmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3166 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/neoaccountstatetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      854 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/nep11transferevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/nep17transferevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      567 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/contract/nep5transferevent.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.226288 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      999 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      814 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/builtindecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1367 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/classmethoddecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2817 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/contractdecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3441 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/displaynamedecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      352 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/instancemethoddecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/metadatadecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1467 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/propertydecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3203 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/publicdecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      232 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/staticmethoddecorator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.226288 neo3-boa-1.0.1/boa3/internal/model/builtin/internal/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      238 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/internal/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2038 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/internal/getenvmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/internal/innerdeploymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/internal/internalmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.226288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.230288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2484 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4020 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/blocktype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/currenthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      730 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/currentindexmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      800 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/getblockmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/getcontractmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionfromblockmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionheightmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      745 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionsignersmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionvmstatemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3636 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/signertype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3854 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/transactiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/vmstatetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessconditionenumtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3045 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessconditiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1652 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessruleactiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3264 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessruletype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1587 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessscopeenumtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.230288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1496 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1754 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/callflagstype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2049 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/callmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.230288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1521 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractabitype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1951 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1755 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractgrouptype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2236 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1905 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparametertype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2009 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1741 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3375 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contracttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      883 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/createmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      821 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/createmultisigaccountmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      698 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/createstandardaccountmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/destroymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      543 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getcallflagsmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getgasscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getminimumdeploymentfeemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getneoscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/updatemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1167 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contractgethashmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1061 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/checkmultisigmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      974 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/checksigmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1262 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/hash160method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1258 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/hash256method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/murmur32method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1614 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/namedcurvetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/ripemd160method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      489 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/sha256method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/verifywithecdsa.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18175 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interopevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interopinterfacetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1762 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interopmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      231 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1855 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/getiteratorvalue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1520 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/iteratorinitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/iteratornextmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2828 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/iteratortype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/json/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/json/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/json/jsondeserializemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/json/jsonserializemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      749 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1068 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Ledger/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Ledger/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Ledger/ledgermethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Neo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Neo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Neo/getneoscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Neo/neocontractmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.234288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Nep17/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Nep17/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1108 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Nep17/getnep17scripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      875 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Nep17/nep17method.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.238288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Oracle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Oracle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1030 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Oracle/oraclemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.238288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1070 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      803 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.238288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1074 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.238288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/StdLib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/StdLib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1033 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      506 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5055 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/nativecontractmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.238288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/oraclegetpricemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1043 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/oraclerequestmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1742 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/oracleresponsecodetype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.242288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      532 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      506 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/getexecfeefactormethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/getfeeperbytemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/getstoragepricemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/isblockedmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.242288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/role/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      252 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/role/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      822 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/role/getdesignatedbyrolemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1555 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/role/roletype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.242288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2551 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      483 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/burngasmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/checkwitnessmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getaddressversionmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      715 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getblocktimemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getcallingscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getentryscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      839 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getexecutingscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      717 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getgasleftmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      780 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getinvocationcountermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      466 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getnetworkmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2238 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getnotificationsmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getplatformmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getrandommethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      522 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/gettriggermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1693 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/loadscriptmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/logmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3152 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/notificationtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/notifymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/scriptcontainermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1784 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/triggertype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.246288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1528 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/atoimethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base58checkdecodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base58checkencodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base58decodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base58encodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base64decodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base64encodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      500 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/deserializemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/itoamethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/memorycomparemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1217 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/memorysearchmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/serializemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.246288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1184 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/findoptionstype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.246288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      581 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1270 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2188 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontexttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2916 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagedeletemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4441 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagefindmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      601 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagegetcontextmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3412 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagegetmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagegetreadonlycontextmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.246288 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1326 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1318 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemapgetmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1631 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemapputmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4029 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemaptype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3282 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storageputmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.250288 neo3-boa-1.0.1/boa3/internal/model/builtin/math/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      418 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/math/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2625 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/math/decimalceil.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2590 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/math/decimalfloor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/math/powmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      755 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/math/sqrtmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.254288 neo3-boa-1.0.1/boa3/internal/model/builtin/method/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3698 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/absmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4429 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/boolmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      949 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/builtinevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6600 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/builtinmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      733 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/bytearrayencodingmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3780 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/bytearraymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/createeventmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3300 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/ecpointmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1848 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/ecpointtoscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2407 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/exceptionmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/exitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19709 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/intbytestringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      710 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/intintmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1585 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/intmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5585 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/isinstancemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1766 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/lenmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2535 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/listbytesstringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5630 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/listgenericmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      993 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/listmappingmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3490 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/listmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1091 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/listsequencemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4451 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/maxbytestringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      377 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/maxintmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5942 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/maxmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4455 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/minbytestringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      377 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/minintmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5896 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/minmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      749 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/printboolmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/printbytestringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/printclassmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/printintmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4822 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/printmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/printsequencemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4349 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/rangemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4970 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/reversedmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1614 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/strboolmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/strbytestringmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      633 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/strintmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1572 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/strmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4281 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/strsplitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/summethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1563 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/supermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2550 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/toboolmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4813 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/tobytesmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2537 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/tointmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5221 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/toscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2537 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/tostrmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4832 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/uint160method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4832 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/method/uint256method.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.254288 neo3-boa-1.0.1/boa3/internal/model/builtin/native/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.258288 neo3-boa-1.0.1/boa3/internal/model/builtin/native/contract_management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      125 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/contract_management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/contract_management/hasmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1566 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/contractmanagementclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/cryptolibclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1484 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/gasclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1392 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/inativecontractclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1517 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/ledgerclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2454 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nativecontract.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.258288 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1730 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getaccountstatemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      825 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getallcandidatesmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      783 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatesmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatevotemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getcommitteemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      495 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getgasperblockmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getnextblockvalidators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/registercandidatemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/unclaimedgasmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/unregistercandidatemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/unvote.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/vote.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3024 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/neoclass.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.258288 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/balanceofmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      525 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/decimalsmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/symbolmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/totalsupplymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1004 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/transfermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/oracleclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1280 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/policyclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/rolemanagementclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/builtin/native/stdlibclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7112 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/callable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/debuginstruction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1139 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/decorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1308 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/event.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      823 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/expression.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      833 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/identifiedsymbol.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.258288 neo3-boa-1.0.1/boa3/internal/model/imports/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/imports/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6500 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/imports/builtin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2849 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/imports/importsymbol.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4942 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/imports/package.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5833 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4285 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/module.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.258288 neo3-boa-1.0.1/boa3/internal/model/operation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.258288 neo3-boa-1.0.1/boa3/internal/model/operation/binary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.262288 neo3-boa-1.0.1/boa3/internal/model/operation/binary/additional/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/additional/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5881 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/additional/membership.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/additional/notmembership.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.262288 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1556 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/addition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2253 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/concat.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1456 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/division.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/floordivision.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/listaddition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2827 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/modulo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1568 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/multiplication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1478 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/power.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2475 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/strbytesmultiplication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/subtraction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/binaryoperation.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.262288 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/booleanand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/booleanor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1525 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/leftshift.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1497 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/logicand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/logicor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1497 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/logicxor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1529 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/rightshift.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.266289 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1182 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1505 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/greaterthan.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/greaterthanorequal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/identity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/lessthan.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1516 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/lessthanorequal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1377 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/notidentity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1512 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/numericequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/numericinequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/objectequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1603 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/objectinequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4190 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/binaryop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3286 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/operation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2300 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/operator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.266289 neo3-boa-1.0.1/boa3/internal/model/operation/unary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      453 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1320 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/booleannot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1336 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/logicnot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/negative.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1606 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/noneidentity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/nonenotidentity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1390 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/positive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1485 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unary/unaryoperation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1973 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/operation/unaryop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      928 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/property.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.266289 neo3-boa-1.0.1/boa3/internal/model/standards/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/standards/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2243 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/standards/neostandard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2469 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/standards/nep11standard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1435 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/standards/nep17standard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/standards/standardmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      322 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/symbol.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.266289 neo3-boa-1.0.1/boa3/internal/model/type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.266289 neo3-boa-1.0.1/boa3/internal/model/type/annotation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/annotation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/annotation/metatype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1710 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/annotation/optionaltype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4093 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/annotation/uniontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      843 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/anytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      639 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/baseexceptiontype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.270289 neo3-boa-1.0.1/boa3/internal/model/type/classes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/classarraytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1587 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/classinitmethoddefault.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      119 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/classscope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/classstructtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8647 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/classtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1202 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/contractinterfaceclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1035 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/contractinterfacehash.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4631 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/pythonclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5768 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/classes/userclass.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.270289 neo3-boa-1.0.1/boa3/internal/model/type/collection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1470 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/genericcollectiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6127 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/icollection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.270289 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      892 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/genericmappingtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4114 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mappingtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.270289 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mutable/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mutable/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1347 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mutable/dicttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mutable/mutablemappingtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.270289 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      627 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/buffertype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/ecpointtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1128 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/genericsequencetype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.270289 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1186 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/genericmutablesequencetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1709 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/listtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1433 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/mutablesequencetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1412 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/rangetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1498 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/reversedtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1513 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/sequencetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1353 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/tupletype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1851 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/uint160type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1927 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/uint256type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5319 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/itype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1119 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/math.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/model/type/neo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/addresstype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/blockhashtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1699 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/opcodetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/publickeytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      622 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/scripthashlittleendiantype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      550 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/scripthashtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/neo/transactionidtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/model/type/primitive/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1209 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/booltype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/bytearraytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/bytestringtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1042 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/bytestype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1908 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/ibytestringtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1246 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/inttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1005 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/nonetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      193 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/primitivetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1733 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/primitive/strtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4639 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1874 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/typeutils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/model/type/typingmethod/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/typingmethod/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4456 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/type/typingmethod/casttypemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1759 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/model/variable.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2541 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/contracts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       98 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/contracts/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2016 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/contracts/neffile.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/core/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/core/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/core/types/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/core/types/InteropInterface.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/core/types/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/cryptography/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      603 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/cryptography/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/smart_contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/smart_contract/VoidType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/smart_contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2267 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/smart_contract/notification.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.274289 neo3-boa-1.0.1/boa3/internal/neo/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4096 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/utils/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo/vm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/CallCode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3476 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/TryCode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3284 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/VMCode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29012 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/Opcode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10557 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/OpcodeHelper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27309 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/OpcodeInfo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1209 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/OpcodeInformation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo/vm/type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1780 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/type/AbiType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/type/ContractParameterType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/type/Integer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2516 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/type/StackItem.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/type/String.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo/vm/type/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/contracts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2843 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/contracttypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1555 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/findoptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/namedcurve.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/contracts/native/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/native/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/native/nativetypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9076 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/contracts/nef.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/core/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/core/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23279 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/core/serialization.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/core/types/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/core/types/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4432 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/core/types/biginteger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8211 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/core/types/uint.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/core/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/network/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/network/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.278289 neo3-boa-1.0.1/boa3/internal/neo3/network/payloads/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      120 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/network/payloads/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1468 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/network/payloads/oracleresponsecode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/network/payloads/verification.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3/internal/neo3/vm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       29 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/vm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/neo3/vm/vmstate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3/internal/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.206288 neo3-boa-1.0.1/boa3_test/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/interface/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/interface/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1156 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/interface/itransactionobject.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/invokeresult.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2245 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neobatchinvoke.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1741 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neoinvoke.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2429 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neoinvokecollection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1915 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neoinvokeresult.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/network/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2165 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/signer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1898 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/testblock.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4483 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/testtransaction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      968 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/witness.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1200 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/witnessscope.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5316 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/contractcollection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2733 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/testcontract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/triggertype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/model/wallet/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/wallet/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1977 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/wallet/account.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      530 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/model/wallet/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.282289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       45 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8723 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/batch.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/batch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/batch/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/create.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      434 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/icheckpointcommand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/restore.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1727 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/deploy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/icontractcommand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/invoke.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      577 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/run.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/create/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1227 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/create/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/fastforward/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      948 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/fastforward/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/neoexpresscommand.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/reset/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      944 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/reset/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1041 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/block.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/ishowcommand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      694 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/transaction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/transfer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1414 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/transfer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1218 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoxp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoxp_contract.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/utils/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/model/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      969 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/model/neoxpaccount.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3326 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/model/neoxpconfig.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8510 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/neoxp/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.286289 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.290289 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/block.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/contract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1460 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/notification.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4193 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/storage.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/storagecollection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/transaction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      934 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/transactionlog.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19143 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/neo_test_runner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/testrunner/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      335 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/test_drive/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.290289 neo3-boa-1.0.1/boa3_test/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16870 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/boa_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2360 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/run_unit_tests.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.290289 neo3-boa-1.0.1/boa3_test/tests/test_classes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/TestExecutionException.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.290289 neo3-boa-1.0.1/boa3_test/tests/test_classes/binaryserializer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1974 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/binaryserializer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1699 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/block.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.290289 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1198 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neoabistruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neoeventstruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1746 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neomanifeststruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1174 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neomethodstruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1423 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neopermissionsstruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      975 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neostruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1558 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/contractcollection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/nativeaccountstate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/nativecontractprefix.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2542 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/signer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6453 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/storage.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3160 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/testcontract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2412 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/transaction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.290289 neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2202 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      681 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/transactionattributetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_classes/witness.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3044 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/boa3_test/tests/test_suite.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-02 16:37:58.294289 neo3-boa-1.0.1/neo3_boa.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4521 2023-08-02 16:37:58.000000 neo3-boa-1.0.1/neo3_boa.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37541 2023-08-02 16:37:58.000000 neo3-boa-1.0.1/neo3_boa.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-02 16:37:58.000000 neo3-boa-1.0.1/neo3_boa.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-08-02 16:37:58.000000 neo3-boa-1.0.1/neo3_boa.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-08-02 16:37:58.000000 neo3-boa-1.0.1/neo3_boa.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2023-08-02 16:37:58.000000 neo3-boa-1.0.1/neo3_boa.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      159 2023-08-02 16:37:58.294289 neo3-boa-1.0.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4985 2023-08-02 16:37:42.000000 neo3-boa-1.0.1/setup.py
```

### Comparing `neo3-boa-1.0.0/LICENSE` & `neo3-boa-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/PKG-INFO` & `neo3-boa-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo3-boa
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python compiler for the Neo3 Virtual Machine
 Home-page: https://github.com/CityOfZion/neo3-boa
 License: Apache License 2.0
 Description: 
         ============================================
         Python compiler for the Neo3 Virtual Machine
         ============================================
```

### Comparing `neo3-boa-1.0.0/README.rst` & `neo3-boa-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/boa3.py` & `neo3-boa-1.0.1/boa3/boa3.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/compile_time/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/compile_time/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/contract/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/blockchain/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/blockchain/block.py` & `neo3-boa-1.0.1/boa3/builtin/interop/blockchain/block.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/blockchain/signer.py` & `neo3-boa-1.0.1/boa3/builtin/interop/blockchain/signer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/blockchain/transaction.py` & `neo3-boa-1.0.1/boa3/builtin/interop/blockchain/transaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/contract/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/contract/contract.py` & `neo3-boa-1.0.1/boa3/builtin/interop/contract/contract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/contract/contractmanifest.py` & `neo3-boa-1.0.1/boa3/builtin/interop/contract/contractmanifest.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/crypto/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/iterator/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/json/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/json/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/policy/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/role/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/role/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/runtime/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/runtime/notification.py` & `neo3-boa-1.0.1/boa3/builtin/interop/runtime/notification.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/stdlib/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/stdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/storage/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/interop/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/storage/storagecontext.py` & `neo3-boa-1.0.1/boa3/builtin/interop/storage/storagecontext.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/interop/storage/storagemap.py` & `neo3-boa-1.0.1/boa3/builtin/interop/storage/storagemap.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/math.py` & `neo3-boa-1.0.1/boa3/builtin/math.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/contractmanagement.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/contractmanagement.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/cryptolib.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/cryptolib.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/gas.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/gas.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/ledger.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/ledger.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/neo.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/neo.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/oracle.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/oracle.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/policy.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/policy.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/rolemanagement.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/rolemanagement.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/nativecontract/stdlib.py` & `neo3-boa-1.0.1/boa3/builtin/nativecontract/stdlib.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/type/__init__.py` & `neo3-boa-1.0.1/boa3/builtin/type/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/builtin/type/helper.py` & `neo3-boa-1.0.1/boa3/builtin/type/helper.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/cli.py` & `neo3-boa-1.0.1/boa3/cli.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/cpm.py` & `neo3-boa-1.0.1/boa3/cpm.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/analyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/analyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/astanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/astanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/astoptimizer.py` & `neo3-boa-1.0.1/boa3/internal/analyser/astoptimizer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/builtinfunctioncallanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/builtinfunctioncallanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/constructanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/constructanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/importanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/importanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/model/functionarguments.py` & `neo3-boa-1.0.1/boa3/internal/analyser/model/functionarguments.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/model/optimizer/Operation.py` & `neo3-boa-1.0.1/boa3/internal/analyser/model/optimizer/Operation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/model/optimizer/__init__.py` & `neo3-boa-1.0.1/boa3/internal/analyser/model/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/model/symbolscope.py` & `neo3-boa-1.0.1/boa3/internal/analyser/model/symbolscope.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/moduleanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/moduleanalyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,27 +381,41 @@
                     other_instructions.append(node)
 
             module: ast.Module = ast.parse('')
             module.body = imports + [function] + other_instructions
             ast.copy_location(module, function)
             namespace = {}
 
+            import sys
+            file_dir = os.path.abspath(os.path.dirname(self.filename))
+            sys_path = sys.path.copy()
+
             try:
+                from boa3.internal import utils
+                if os.path.abspath(self.root_folder) != file_dir:
+                    sc_paths = [os.path.abspath(self.root_folder), file_dir]
+                else:
+                    sc_paths = [file_dir]
+
+                sys.path = sc_paths + utils.list_inner_packages(file_dir) + sys_path
+
                 # executes the function
                 code = compile(module, filename='<boa3>', mode='exec')
                 exec(code, namespace)
             except ModuleNotFoundError:
                 # will fail if any imports can't be executed
                 # in this case, the error is already logged
                 return
             except BaseException as inner_exception:
                 # reordering the module tree may raise unexpected exceptions
                 # ignore if it has generated the metadata function
                 if function.name not in namespace:
                     raise inner_exception
+            finally:
+                sys.path = sys_path
 
             obj: Any = namespace[function.name]()
             node: ast.AST = function.body[-1] if len(function.body) > 0 else function
             # return must be a NeoMetadata object
             if not isinstance(obj, NeoMetadata):
                 obj_type = self.get_type(obj).identifier if self.get_type(obj) is not Type.any else type(obj).__name__
                 self._log_error(
```

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/supportedstandard/standardanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/supportedstandard/standardanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/analyser/typeanalyser.py` & `neo3-boa-1.0.1/boa3/internal/analyser/typeanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/cli_commands/compile_command.py` & `neo3-boa-1.0.1/boa3/internal/cli_commands/compile_command.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/__init__.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/codegenerator.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/codegenerator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/codegeneratorvisitor.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/codegeneratorvisitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,14 +941,23 @@
         if name not in self._symbols:
             hashed_name = self._get_unique_name(name, self._tree)
             if hashed_name not in self._symbols and hasattr(name_node, 'origin'):
                 hashed_name = self._get_unique_name(name, name_node.origin)
 
             if hashed_name in self._symbols:
                 name = hashed_name
+
+        else:
+            if name not in self.generator.symbol_table:
+                symbol = self._symbols[name]
+                for symbol_id, internal_symbol in self.generator.symbol_table.items():
+                    if internal_symbol == symbol:
+                        name = symbol_id
+                        break
+
         return self.build_data(name_node, name)
 
     def visit_Starred(self, starred: ast.Starred) -> GeneratorData:
         value_data = self.visit_to_generate(starred.value)
         self.generator.convert_starred_variable()
 
         starred_data = value_data.copy(starred)
```

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/generatordata.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/generatordata.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/initstatementsvisitor.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/initstatementsvisitor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/methodtokencollection.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/methodtokencollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/stackmemento.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/stackmemento.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/vmcodemap.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/vmcodemap.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/codegenerator/vmcodemapping.py` & `neo3-boa-1.0.1/boa3/internal/compiler/codegenerator/vmcodemapping.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/compiledmetadata.py` & `neo3-boa-1.0.1/boa3/internal/compiler/compiledmetadata.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/compiler.py` & `neo3-boa-1.0.1/boa3/internal/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/filegenerator/filegenerator.py` & `neo3-boa-1.0.1/boa3/internal/compiler/filegenerator/filegenerator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/compiler/filegenerator/importdata.py` & `neo3-boa-1.0.1/boa3/internal/compiler/filegenerator/importdata.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/constants.py` & `neo3-boa-1.0.1/boa3/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/exception/CompilerError.py` & `neo3-boa-1.0.1/boa3/internal/exception/CompilerError.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/exception/CompilerWarning.py` & `neo3-boa-1.0.1/boa3/internal/exception/CompilerWarning.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/attribute.py` & `neo3-boa-1.0.1/boa3/internal/model/attribute.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/builtin.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/builtin.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/builtincallable.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/builtincallable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/builtinproperty.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/builtinproperty.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/builtinsymbol.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/builtinsymbol.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/appendmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/appendmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/clearmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/clearmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/copydictmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/copydictmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/copymethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/copymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countsequencegenericmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countsequencegenericmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countsequencemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countsequencemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countsequenceprimitivemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countsequenceprimitivemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/countstrmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/countstrmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/extendmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/extendmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/indexbytesstringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/indexbytesstringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/indexmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/indexmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/indexsequencemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/indexsequencemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/insertmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/insertmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/isdigitmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/isdigitmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/joinmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/joinmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/lowermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/lowermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/mapkeysmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/mapkeysmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/mapvaluesmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/mapvaluesmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popdictdefaultmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popdictdefaultmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popdictmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popdictmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/popsequencemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/popsequencemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/removemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/removemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/reversemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/reversemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/startswithmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/startswithmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/stripmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/stripmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/classmethod/uppermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/classmethod/uppermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/contract/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/contract/abortmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/contract/abortmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/contract/neoaccountstatetype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/contract/neoaccountstatetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/contract/nep11transferevent.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/contract/nep11transferevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/contract/nep17transferevent.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/contract/nep17transferevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/contract/nep5transferevent.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/contract/nep5transferevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/builtindecorator.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/builtindecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/classmethoddecorator.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/classmethoddecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/contractdecorator.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/contractdecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/displaynamedecorator.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/displaynamedecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/propertydecorator.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/propertydecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/decorator/publicdecorator.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/decorator/publicdecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/internal/getenvmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/internal/getenvmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/internal/innerdeploymethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/internal/innerdeploymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/internal/internalmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/internal/internalmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/blocktype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/blocktype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/currenthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/currenthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/currentindexmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/currentindexmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/getblockmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/getblockmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/getcontractmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/getcontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionfromblockmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionfromblockmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionheightmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionheightmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionsignersmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionsignersmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/gettransactionvmstatemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/gettransactionvmstatemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/signertype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/signertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/transactiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/transactiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/vmstatetype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/vmstatetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessconditionenumtype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessconditionenumtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessconditiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessconditiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessruleactiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessruleactiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessruletype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessruletype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/blockchain/witnessscopeenumtype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/blockchain/witnessscopeenumtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/callflagstype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/callflagstype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/callmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/callmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractabitype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractabitype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractgrouptype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractgrouptype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparametertype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractparametertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/contracttype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/contracttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/createmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/createmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/createmultisigaccountmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/createmultisigaccountmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/createstandardaccountmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/createstandardaccountmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getcallflagsmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getcallflagsmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getgasscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getgasscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getminimumdeploymentfeemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getminimumdeploymentfeemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/getneoscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/getneoscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contract/updatemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contract/updatemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/contractgethashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/contractgethashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/checkmultisigmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/checkmultisigmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/checksigmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/checksigmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/hash160method.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/hash160method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/hash256method.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/hash256method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/murmur32method.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/murmur32method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/namedcurvetype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/namedcurvetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/crypto/verifywithecdsa.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/crypto/verifywithecdsa.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interop.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interop.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interopevent.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interopevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interopinterfacetype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interopinterfacetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/interopmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/interopmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/getiteratorvalue.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/getiteratorvalue.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/iteratorinitmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/iteratorinitmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/iteratornextmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/iteratornextmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/iterator/iteratortype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/iterator/iteratortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Ledger/ledgermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Ledger/ledgermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Neo/getneoscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Neo/getneoscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Neo/neocontractmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Neo/neocontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Nep17/getnep17scripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Nep17/getnep17scripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Nep17/nep17method.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Nep17/nep17method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/Oracle/oraclemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/Oracle/oraclemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/nativecontract/nativecontractmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/nativecontract/nativecontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/oraclegetpricemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/oraclegetpricemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/oraclerequestmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/oraclerequestmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/oracle/oracleresponsecodetype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/oracle/oracleresponsecodetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/policy/isblockedmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/policy/isblockedmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/role/getdesignatedbyrolemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/role/getdesignatedbyrolemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/role/roletype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/role/roletype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/checkwitnessmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/checkwitnessmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getaddressversionmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getaddressversionmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getblocktimemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getblocktimemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getcallingscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getcallingscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getentryscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getentryscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getexecutingscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getexecutingscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getgasleftmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getgasleftmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getinvocationcountermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getinvocationcountermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getnotificationsmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getnotificationsmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/getplatformmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/getplatformmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/gettriggermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/gettriggermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/loadscriptmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/loadscriptmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/notificationtype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/notificationtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/notifymethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/notifymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/scriptcontainermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/scriptcontainermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/runtime/triggertype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/runtime/triggertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/atoimethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/atoimethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base58checkdecodemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base58checkdecodemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/base58checkencodemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/base58checkencodemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/itoamethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/itoamethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/memorycomparemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/memorycomparemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/stdlib/memorysearchmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/stdlib/memorysearchmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/findoptionstype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/findoptionstype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontexttype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagecontext/storagecontexttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagedeletemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagedeletemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagefindmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagefindmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagegetcontextmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagegetcontextmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagegetmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagegetmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagegetreadonlycontextmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagegetreadonlycontextmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemapgetmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemapgetmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemapputmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemapputmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storagemap/storagemaptype.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storagemap/storagemaptype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/interop/storage/storageputmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/interop/storage/storageputmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/math/decimalceil.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/math/decimalceil.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/math/decimalfloor.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/math/decimalfloor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/math/powmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/math/powmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/math/sqrtmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/math/sqrtmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/absmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/absmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/boolmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/boolmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/builtinevent.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/builtinevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/builtinmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/builtinmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/bytearrayencodingmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/bytearrayencodingmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/bytearraymethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/bytearraymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/createeventmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/createeventmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/ecpointmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/ecpointmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/ecpointtoscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/ecpointtoscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/exceptionmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/exceptionmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/exitmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/exitmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/intbytestringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/intbytestringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/intintmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/intintmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/intmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/intmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/isinstancemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/isinstancemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/lenmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/lenmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/listbytesstringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/listbytesstringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/listgenericmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/listgenericmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/listmappingmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/listmappingmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/listmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/listmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/listsequencemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/listsequencemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/maxbytestringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/maxbytestringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/maxmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/maxmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/minbytestringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/minbytestringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/minmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/minmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/printboolmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/printboolmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/printbytestringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/printbytestringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/printclassmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/printclassmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/printintmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/printintmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/printmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/printmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/printsequencemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/printsequencemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/rangemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/rangemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/reversedmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/reversedmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/strboolmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/strboolmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/strbytestringmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/strbytestringmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/strintmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/strintmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/strmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/strmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/strsplitmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/strsplitmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/summethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/summethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/supermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/supermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/toboolmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/toboolmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/tobytesmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/tobytesmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/tointmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/tointmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/toscripthashmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/toscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/tostrmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/tostrmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/uint160method.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/uint160method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/method/uint256method.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/method/uint256method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/contract_management/hasmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/contract_management/hasmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/contractmanagementclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/contractmanagementclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/cryptolibclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/cryptolibclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/gasclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/gasclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/inativecontractclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/inativecontractclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/ledgerclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/ledgerclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nativecontract.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nativecontract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getaccountstatemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getaccountstatemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getallcandidatesmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getallcandidatesmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatesmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatesmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatevotemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getcandidatevotemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getcommitteemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getcommitteemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/getnextblockvalidators.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/getnextblockvalidators.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/registercandidatemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/registercandidatemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/unclaimedgasmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/unclaimedgasmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/unregistercandidatemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/unregistercandidatemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/unvote.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/unvote.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neo_contract_methods/vote.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neo_contract_methods/vote.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/neoclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/neoclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/balanceofmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/balanceofmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/decimalsmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/decimalsmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/symbolmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/symbolmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/totalsupplymethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/totalsupplymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/nep17_methods/transfermethod.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/nep17_methods/transfermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/oracleclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/oracleclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/policyclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/policyclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/rolemanagementclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/rolemanagementclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/builtin/native/stdlibclass.py` & `neo3-boa-1.0.1/boa3/internal/model/builtin/native/stdlibclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/callable.py` & `neo3-boa-1.0.1/boa3/internal/model/callable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/debuginstruction.py` & `neo3-boa-1.0.1/boa3/internal/model/debuginstruction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/decorator.py` & `neo3-boa-1.0.1/boa3/internal/model/decorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/event.py` & `neo3-boa-1.0.1/boa3/internal/model/event.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/expression.py` & `neo3-boa-1.0.1/boa3/internal/model/expression.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/identifiedsymbol.py` & `neo3-boa-1.0.1/boa3/internal/model/identifiedsymbol.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/imports/builtin.py` & `neo3-boa-1.0.1/boa3/internal/model/imports/builtin.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/imports/importsymbol.py` & `neo3-boa-1.0.1/boa3/internal/model/imports/importsymbol.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/imports/package.py` & `neo3-boa-1.0.1/boa3/internal/model/imports/package.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/method.py` & `neo3-boa-1.0.1/boa3/internal/model/method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/module.py` & `neo3-boa-1.0.1/boa3/internal/model/module.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/additional/membership.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/additional/membership.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/additional/notmembership.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/additional/notmembership.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/addition.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/addition.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/concat.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/concat.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/division.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/division.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/floordivision.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/floordivision.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/listaddition.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/listaddition.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/modulo.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/modulo.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/multiplication.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/multiplication.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/power.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/power.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/strbytesmultiplication.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/strbytesmultiplication.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/arithmetic/subtraction.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/arithmetic/subtraction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/binaryoperation.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/binaryoperation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/booleanand.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/booleanand.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/booleanor.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/booleanor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/leftshift.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/leftshift.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/logicand.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/logicand.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/logicor.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/logicor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/logicxor.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/logicxor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/logical/rightshift.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/logical/rightshift.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/greaterthan.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/greaterthan.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/greaterthanorequal.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/greaterthanorequal.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/identity.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/identity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/lessthan.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/lessthan.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/lessthanorequal.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/lessthanorequal.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/notidentity.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/notidentity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/numericequality.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/numericequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/numericinequality.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/numericinequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/objectequality.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/objectequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binary/relational/objectinequality.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binary/relational/objectinequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/binaryop.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/binaryop.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/operation.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/operation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/operator.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/operator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/booleannot.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/booleannot.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/logicnot.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/logicnot.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/negative.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/negative.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/noneidentity.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/noneidentity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/nonenotidentity.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/nonenotidentity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/positive.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/positive.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unary/unaryoperation.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unary/unaryoperation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/operation/unaryop.py` & `neo3-boa-1.0.1/boa3/internal/model/operation/unaryop.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/property.py` & `neo3-boa-1.0.1/boa3/internal/model/property.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/standards/neostandard.py` & `neo3-boa-1.0.1/boa3/internal/model/standards/neostandard.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/standards/nep11standard.py` & `neo3-boa-1.0.1/boa3/internal/model/standards/nep11standard.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/standards/nep17standard.py` & `neo3-boa-1.0.1/boa3/internal/model/standards/nep17standard.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/standards/standardmethod.py` & `neo3-boa-1.0.1/boa3/internal/model/standards/standardmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/annotation/metatype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/annotation/metatype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/annotation/optionaltype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/annotation/optionaltype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/annotation/uniontype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/annotation/uniontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/anytype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/anytype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/baseexceptiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/baseexceptiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/classarraytype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/classarraytype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/classinitmethoddefault.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/classinitmethoddefault.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/classstructtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/classstructtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/classtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/classtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/contractinterfaceclass.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/contractinterfaceclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/contractinterfacehash.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/contractinterfacehash.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/pythonclass.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/pythonclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/classes/userclass.py` & `neo3-boa-1.0.1/boa3/internal/model/type/classes/userclass.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/genericcollectiontype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/genericcollectiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/icollection.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/icollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/genericmappingtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/genericmappingtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mappingtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mappingtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mutable/dicttype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mutable/dicttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/mapping/mutable/mutablemappingtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/mapping/mutable/mutablemappingtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/buffertype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/buffertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/ecpointtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/ecpointtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/genericsequencetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/genericsequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/genericmutablesequencetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/genericmutablesequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/listtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/listtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/mutable/mutablesequencetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/mutable/mutablesequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/rangetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/rangetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/reversedtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/reversedtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/sequencetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/sequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/tupletype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/tupletype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/uint160type.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/uint160type.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/collection/sequence/uint256type.py` & `neo3-boa-1.0.1/boa3/internal/model/type/collection/sequence/uint256type.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/itype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/itype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/math.py` & `neo3-boa-1.0.1/boa3/internal/model/type/math.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/__init__.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/blockhashtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/blockhashtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/opcodetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/opcodetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/publickeytype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/publickeytype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/scripthashlittleendiantype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/scripthashlittleendiantype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/scripthashtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/scripthashtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/neo/transactionidtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/neo/transactionidtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/booltype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/booltype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/bytearraytype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/bytearraytype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/bytestringtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/bytestringtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/bytestype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/bytestype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/ibytestringtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/ibytestringtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/inttype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/inttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/nonetype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/nonetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/primitive/strtype.py` & `neo3-boa-1.0.1/boa3/internal/model/type/primitive/strtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/type.py` & `neo3-boa-1.0.1/boa3/internal/model/type/type.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/typeutils.py` & `neo3-boa-1.0.1/boa3/internal/model/type/typeutils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/type/typingmethod/casttypemethod.py` & `neo3-boa-1.0.1/boa3/internal/model/type/typingmethod/casttypemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/model/variable.py` & `neo3-boa-1.0.1/boa3/internal/model/variable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/__init__.py` & `neo3-boa-1.0.1/boa3/internal/neo/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/contracts/neffile.py` & `neo3-boa-1.0.1/boa3/internal/neo/contracts/neffile.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/cryptography/__init__.py` & `neo3-boa-1.0.1/boa3/internal/neo/cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/smart_contract/notification.py` & `neo3-boa-1.0.1/boa3/internal/neo/smart_contract/notification.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/utils/__init__.py` & `neo3-boa-1.0.1/boa3/internal/neo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/CallCode.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/CallCode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/TryCode.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/TryCode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/VMCode.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/VMCode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/Opcode.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/Opcode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/OpcodeHelper.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/OpcodeHelper.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/OpcodeInfo.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/OpcodeInfo.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/opcode/OpcodeInformation.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/opcode/OpcodeInformation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/type/AbiType.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/type/AbiType.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/type/ContractParameterType.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/type/ContractParameterType.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/type/Integer.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/type/Integer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo/vm/type/StackItem.py` & `neo3-boa-1.0.1/boa3/internal/neo/vm/type/StackItem.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/contracts/contracttypes.py` & `neo3-boa-1.0.1/boa3/internal/neo3/contracts/contracttypes.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/contracts/findoptions.py` & `neo3-boa-1.0.1/boa3/internal/neo3/contracts/findoptions.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/contracts/native/nativetypes.py` & `neo3-boa-1.0.1/boa3/internal/neo3/contracts/native/nativetypes.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/contracts/nef.py` & `neo3-boa-1.0.1/boa3/internal/neo3/contracts/nef.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/core/serialization.py` & `neo3-boa-1.0.1/boa3/internal/neo3/core/serialization.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/core/types/biginteger.py` & `neo3-boa-1.0.1/boa3/internal/neo3/core/types/biginteger.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/core/types/uint.py` & `neo3-boa-1.0.1/boa3/internal/neo3/core/types/uint.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/core/utils.py` & `neo3-boa-1.0.1/boa3/internal/neo3/core/utils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/network/payloads/oracleresponsecode.py` & `neo3-boa-1.0.1/boa3/internal/neo3/network/payloads/oracleresponsecode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/network/payloads/verification.py` & `neo3-boa-1.0.1/boa3/internal/neo3/network/payloads/verification.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3/internal/neo3/vm/vmstate.py` & `neo3-boa-1.0.1/boa3/internal/neo3/vm/vmstate.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/interface/itransactionobject.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/interface/itransactionobject.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neobatchinvoke.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neobatchinvoke.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neoinvoke.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neoinvoke.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neoinvokecollection.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neoinvokecollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/invoker/neoinvokeresult.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/invoker/neoinvokeresult.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/signer.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/signer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/testblock.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/testblock.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/testtransaction.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/testtransaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/witness.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/witness.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/network/payloads/witnessscope.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/network/payloads/witnessscope.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/contractcollection.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/contractcollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/testcontract.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/testcontract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/smart_contract/triggertype.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/smart_contract/triggertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/wallet/account.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/wallet/account.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/model/wallet/utils.py` & `neo3-boa-1.0.1/boa3_test/test_drive/model/wallet/utils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/batch.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/batch.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/batch/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/create.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/create.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/restore.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/checkpoint/restore.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/deploy.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/deploy.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/invoke.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/invoke.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/list.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/list.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/run.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/contract/run.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/create/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/create/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/fastforward/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/fastforward/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/neoexpresscommand.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/neoexpresscommand.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/reset/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/reset/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/block.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/block.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/transaction.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/show/transaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoexpresscommand/transfer/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoexpresscommand/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoxp.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoxp.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/neoxp_contract.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/neoxp_contract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/command/utils/__init__.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/command/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/model/neoxpaccount.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/model/neoxpaccount.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/model/neoxpconfig.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/model/neoxpconfig.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/neoxp/utils.py` & `neo3-boa-1.0.1/boa3_test/test_drive/neoxp/utils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/block.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/block.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/contract.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/contract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/log.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/log.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/notification.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/notification.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/storage.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/storage.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/storagecollection.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/storagecollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/transaction.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/transaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/blockchain/transactionlog.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/blockchain/transactionlog.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/neo_test_runner.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/neo_test_runner.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/test_drive/testrunner/utils.py` & `neo3-boa-1.0.1/boa3_test/test_drive/testrunner/utils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/boa_test.py` & `neo3-boa-1.0.1/boa3_test/tests/boa_test.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/run_unit_tests.py` & `neo3-boa-1.0.1/boa3_test/tests/run_unit_tests.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/binaryserializer/__init__.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/binaryserializer/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/block.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/block.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neoabistruct.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neoabistruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neoeventstruct.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neoeventstruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neomanifeststruct.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neomanifeststruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neomethodstruct.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neomethodstruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neopermissionsstruct.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neopermissionsstruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contract/neostruct.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contract/neostruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/contractcollection.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/contractcollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/nativeaccountstate.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/nativeaccountstate.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/nativecontractprefix.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/nativecontractprefix.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/signer.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/signer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/storage.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/storage.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/testcontract.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/testcontract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/transaction.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/transaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py` & `neo3-boa-1.0.1/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/boa3_test/tests/test_suite.py` & `neo3-boa-1.0.1/boa3_test/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-1.0.0/neo3_boa.egg-info/PKG-INFO` & `neo3-boa-1.0.1/neo3_boa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo3-boa
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python compiler for the Neo3 Virtual Machine
 Home-page: https://github.com/CityOfZion/neo3-boa
 License: Apache License 2.0
 Description: 
         ============================================
         Python compiler for the Neo3 Virtual Machine
         ============================================
```

### Comparing `neo3-boa-1.0.0/neo3_boa.egg-info/SOURCES.txt` & `neo3-boa-1.0.1/neo3_boa.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 boa3/builtin/nativecontract/stdlib.py
 boa3/builtin/type/__init__.py
 boa3/builtin/type/helper.py
 boa3/builtin/vm/__init__.py
 boa3/internal/__init__.py
 boa3/internal/constants.py
 boa3/internal/env.py
+boa3/internal/utils.py
 boa3/internal/analyser/__init__.py
 boa3/internal/analyser/analyser.py
 boa3/internal/analyser/astanalyser.py
 boa3/internal/analyser/astoptimizer.py
 boa3/internal/analyser/builtinfunctioncallanalyser.py
 boa3/internal/analyser/constructanalyser.py
 boa3/internal/analyser/importanalyser.py
```

### Comparing `neo3-boa-1.0.0/setup.py` & `neo3-boa-1.0.1/setup.py`

 * *Files identical despite different names*

