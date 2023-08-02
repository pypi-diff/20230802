# Comparing `tmp/web3-6.7.0.tar.gz` & `tmp/web3-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3-6.7.0.tar", last modified: Wed Jul 26 18:44:05 2023, max compression
+gzip compressed data, was "web3-6.8.0.tar", last modified: Wed Aug  2 17:57:26 2023, max compression
```

## Comparing `web3-6.7.0.tar` & `web3-6.8.0.tar`

### file list

```diff
@@ -1,347 +1,347 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.608199 web3-6.7.0/
--rw-r--r--   0 eve        (501) staff       (20)     1090 2023-07-26 18:35:55.000000 web3-6.7.0/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      249 2023-07-26 18:35:55.000000 web3-6.7.0/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     2198 2023-07-26 18:44:05.608037 web3-6.7.0/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1294 2023-06-26 17:45:20.000000 web3-6.7.0/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.547500 web3-6.7.0/ens/
--rw-r--r--   0 eve        (501) staff       (20)      285 2023-06-26 17:45:20.000000 web3-6.7.0/ens/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    17017 2023-07-26 18:35:55.000000 web3-6.7.0/ens/_normalization.py
--rw-r--r--   0 eve        (501) staff       (20)    34745 2023-07-26 18:35:55.000000 web3-6.7.0/ens/abis.py
--rw-r--r--   0 eve        (501) staff       (20)    22277 2023-07-26 18:35:55.000000 web3-6.7.0/ens/async_ens.py
--rw-r--r--   0 eve        (501) staff       (20)       41 2023-06-26 17:45:20.000000 web3-6.7.0/ens/auto.py
--rw-r--r--   0 eve        (501) staff       (20)     3477 2023-07-26 18:35:55.000000 web3-6.7.0/ens/base_ens.py
--rw-r--r--   0 eve        (501) staff       (20)      913 2023-07-26 18:35:55.000000 web3-6.7.0/ens/constants.py
--rw-r--r--   0 eve        (501) staff       (20)   148604 2023-07-26 18:35:55.000000 web3-6.7.0/ens/contract_data.py
--rw-r--r--   0 eve        (501) staff       (20)    21517 2023-07-26 18:35:55.000000 web3-6.7.0/ens/ens.py
--rw-r--r--   0 eve        (501) staff       (20)     2390 2023-06-26 17:45:20.000000 web3-6.7.0/ens/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.547959 web3-6.7.0/ens/specs/
--rw-r--r--   0 eve        (501) staff       (20)    48402 2023-07-26 18:35:55.000000 web3-6.7.0/ens/specs/nf.json
--rw-r--r--   0 eve        (501) staff       (20)  3115333 2023-07-26 18:35:55.000000 web3-6.7.0/ens/specs/normalization_spec.json
--rw-r--r--   0 eve        (501) staff       (20)     9279 2023-07-26 18:35:55.000000 web3-6.7.0/ens/utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.552050 web3-6.7.0/ethpm/
--rw-r--r--   0 eve        (501) staff       (20)      580 2023-06-07 20:55:14.000000 web3-6.7.0/ethpm/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.553295 web3-6.7.0/ethpm/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2511 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/_utils/backend.py
--rw-r--r--   0 eve        (501) staff       (20)     1477 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/_utils/cache.py
--rw-r--r--   0 eve        (501) staff       (20)     2848 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/_utils/chains.py
--rw-r--r--   0 eve        (501) staff       (20)     1030 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/_utils/contract.py
--rw-r--r--   0 eve        (501) staff       (20)     5263 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/_utils/deployments.py
--rw-r--r--   0 eve        (501) staff       (20)     2717 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/_utils/ipfs.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.553664 web3-6.7.0/ethpm/_utils/protobuf/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/_utils/protobuf/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1938 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-r--r--   0 eve        (501) staff       (20)     1488 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/_utils/registry.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.553895 web3-6.7.0/ethpm/assets/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.554025 web3-6.7.0/ethpm/assets/ens/
--rw-r--r--   0 eve        (501) staff       (20)    74682 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/ens/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.554543 web3-6.7.0/ethpm/assets/escrow/
--rw-r--r--   0 eve        (501) staff       (20)     8007 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/escrow/with_bytecode_v3.json
--rw-r--r--   0 eve        (501) staff       (20)      760 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/assets/ipfs_file.proto
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.554826 web3-6.7.0/ethpm/assets/owned/
--rw-r--r--   0 eve        (501) staff       (20)     2655 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/owned/output_v3.json
--rw-r--r--   0 eve        (501) staff       (20)      746 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/owned/with_contract_type_v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.556747 web3-6.7.0/ethpm/assets/registry/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.560820 web3-6.7.0/ethpm/assets/registry/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     3129 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/Authority.sol
--rw-r--r--   0 eve        (501) staff       (20)     2876 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
--rw-r--r--   0 eve        (501) staff       (20)     6380 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/PackageDB.sol
--rw-r--r--   0 eve        (501) staff       (20)    10553 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/PackageRegistry.sol
--rw-r--r--   0 eve        (501) staff       (20)     2966 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 eve        (501) staff       (20)     9041 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/ReleaseDB.sol
--rw-r--r--   0 eve        (501) staff       (20)     4980 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
--rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/solc_input.json
--rw-r--r--   0 eve        (501) staff       (20)   727775 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/solc_output.json
--rw-r--r--   0 eve        (501) staff       (20)   270218 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/registry/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.560959 web3-6.7.0/ethpm/assets/safe-math-lib/
--rw-r--r--   0 eve        (501) staff       (20)     2845 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.562403 web3-6.7.0/ethpm/assets/simple-registry/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.563590 web3-6.7.0/ethpm/assets/simple-registry/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1841 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/simple-registry/contracts/Ownable.sol
--rw-r--r--   0 eve        (501) staff       (20)    12350 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
--rw-r--r--   0 eve        (501) staff       (20)     3278 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 eve        (501) staff       (20)      950 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/simple-registry/solc_input.json
--rw-r--r--   0 eve        (501) staff       (20)   199338 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/simple-registry/solc_output.json
--rw-r--r--   0 eve        (501) staff       (20)    75677 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/simple-registry/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.564254 web3-6.7.0/ethpm/assets/standard-token/
--rw-r--r--   0 eve        (501) staff       (20)    22292 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/standard-token/output_v3.json
--rw-r--r--   0 eve        (501) staff       (20)     8765 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/standard-token/with_bytecode_v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.565067 web3-6.7.0/ethpm/assets/vyper_registry/
--rw-r--r--   0 eve        (501) staff       (20)    81363 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/vyper_registry/0.1.0.json
--rw-r--r--   0 eve        (501) staff       (20)     6339 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/vyper_registry/registry.vy
--rw-r--r--   0 eve        (501) staff       (20)     7596 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/assets/vyper_registry/registry_with_delete.vy
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.565717 web3-6.7.0/ethpm/backends/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      956 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)     3006 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/backends/http.py
--rw-r--r--   0 eve        (501) staff       (20)     6551 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/backends/ipfs.py
--rw-r--r--   0 eve        (501) staff       (20)     4174 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/backends/registry.py
--rw-r--r--   0 eve        (501) staff       (20)      405 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     6303 2023-07-26 18:35:55.000000 web3-6.7.0/ethpm/contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1890 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/dependencies.py
--rw-r--r--   0 eve        (501) staff       (20)     2134 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/deployments.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.541802 web3-6.7.0/ethpm/ethpm-spec/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.541572 web3-6.7.0/ethpm/ethpm-spec/examples/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.566440 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/
--rw-r--r--   0 eve        (501) staff       (20)     6810 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5361 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.566719 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      888 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
--rw-r--r--   0 eve        (501) staff       (20)      644 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
--rw-r--r--   0 eve        (501) staff       (20)    11598 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     8669 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/escrow/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.567270 web3-6.7.0/ethpm/ethpm-spec/examples/owned/
--rw-r--r--   0 eve        (501) staff       (20)      544 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      443 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.567410 web3-6.7.0/ethpm/ethpm-spec/examples/owned/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      222 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
--rw-r--r--   0 eve        (501) staff       (20)      728 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/owned/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.567901 web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/
--rw-r--r--   0 eve        (501) staff       (20)     5272 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5030 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
--rw-r--r--   0 eve        (501) staff       (20)     5220 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     4993 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.568557 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/
--rw-r--r--   0 eve        (501) staff       (20)     3976 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3143 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.568812 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      802 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
--rw-r--r--   0 eve        (501) staff       (20)     5517 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3289 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.569366 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/
--rw-r--r--   0 eve        (501) staff       (20)     3794 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3238 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.569620 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1155 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
--rw-r--r--   0 eve        (501) staff       (20)     2949 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
--rw-r--r--   0 eve        (501) staff       (20)    17129 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     6100 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.570248 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/
--rw-r--r--   0 eve        (501) staff       (20)      590 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      507 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.570481 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      396 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
--rw-r--r--   0 eve        (501) staff       (20)      786 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/transferable/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.571215 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/
--rw-r--r--   0 eve        (501) staff       (20)     6669 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5456 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.572073 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1454 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
--rw-r--r--   0 eve        (501) staff       (20)     9710 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     7326 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.571800 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/
--rw-r--r--   0 eve        (501) staff       (20)     8052 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     6657 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.571938 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      621 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
--rw-r--r--   0 eve        (501) staff       (20)    12191 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     9503 2022-04-27 21:13:00.000000 web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.572458 web3-6.7.0/ethpm/ethpm-spec/spec/
--rw-r--r--   0 eve        (501) staff       (20)    10302 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/spec/package.spec.json
--rw-r--r--   0 eve        (501) staff       (20)    12879 2021-02-11 20:53:14.000000 web3-6.7.0/ethpm/ethpm-spec/spec/v3.spec.json
--rw-r--r--   0 eve        (501) staff       (20)     1194 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    14494 2023-07-26 18:35:55.000000 web3-6.7.0/ethpm/package.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.575742 web3-6.7.0/ethpm/tools/
--rw-r--r--   0 eve        (501) staff       (20)      103 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/tools/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    27045 2023-07-26 18:35:55.000000 web3-6.7.0/ethpm/tools/builder.py
--rw-r--r--   0 eve        (501) staff       (20)    10373 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/tools/checker.py
--rw-r--r--   0 eve        (501) staff       (20)      475 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/tools/get_manifest.py
--rw-r--r--   0 eve        (501) staff       (20)     4368 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/uri.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.576580 web3-6.7.0/ethpm/validation/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/validation/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4716 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/validation/manifest.py
--rw-r--r--   0 eve        (501) staff       (20)     1072 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/validation/misc.py
--rw-r--r--   0 eve        (501) staff       (20)     2317 2023-04-06 21:34:13.000000 web3-6.7.0/ethpm/validation/package.py
--rw-r--r--   0 eve        (501) staff       (20)     4873 2023-06-26 17:45:20.000000 web3-6.7.0/ethpm/validation/uri.py
--rw-r--r--   0 eve        (501) staff       (20)     1202 2023-07-07 17:27:16.000000 web3-6.7.0/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-07-26 18:44:05.608233 web3-6.7.0/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     3076 2023-07-26 18:43:59.000000 web3-6.7.0/setup.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.580173 web3-6.7.0/web3/
--rw-r--r--   0 eve        (501) staff       (20)      804 2023-07-26 18:35:55.000000 web3-6.7.0/web3/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.587592 web3-6.7.0/web3/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    31000 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      456 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/async_caching.py
--rw-r--r--   0 eve        (501) staff       (20)     8123 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/async_transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     2059 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1489 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/caching.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.587742 web3-6.7.0/web3/_utils/compat/
--rw-r--r--   0 eve        (501) staff       (20)      580 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/compat/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5425 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/contract_error_handling.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.587988 web3-6.7.0/web3/_utils/contract_sources/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/contract_sources/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     6492 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/contract_sources/compile_contracts.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.592210 web3-6.7.0/web3/_utils/contract_sources/contract_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      517 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-r--r--   0 eve        (501) staff       (20)     5344 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/address_reflector.py
--rw-r--r--   0 eve        (501) staff       (20)    18852 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    14783 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     6089 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     6334 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-r--r--   0 eve        (501) staff       (20)    37881 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     5573 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/event_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)    15824 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)     1651 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     7637 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/math_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    16716 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-r--r--   0 eve        (501) staff       (20)    32645 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)    15579 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/panic_errors_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1825 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/payable_tester.py
--rw-r--r--   0 eve        (501) staff       (20)    17290 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     5264 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     4264 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/revert_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     3555 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)     8238 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/storage_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    11586 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/string_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    23180 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)    14980 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     1640 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     1738 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/decorators.py
--rw-r--r--   0 eve        (501) staff       (20)      144 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/empty.py
--rw-r--r--   0 eve        (501) staff       (20)     9065 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)     2388 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/ens.py
--rw-r--r--   0 eve        (501) staff       (20)    17198 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/events.py
--rw-r--r--   0 eve        (501) staff       (20)     2113 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/fee_utils.py
--rw-r--r--   0 eve        (501) staff       (20)    11886 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/filters.py
--rw-r--r--   0 eve        (501) staff       (20)     3071 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/formatters.py
--rw-r--r--   0 eve        (501) staff       (20)       55 2023-04-06 21:34:13.000000 web3-6.7.0/web3/_utils/function_identifiers.py
--rw-r--r--   0 eve        (501) staff       (20)      195 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/http.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/hypothesis.py
--rw-r--r--   0 eve        (501) staff       (20)     1047 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/math.py
--rw-r--r--   0 eve        (501) staff       (20)    31322 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/method_formatters.py
--rw-r--r--   0 eve        (501) staff       (20)     1146 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/miner.py
--rw-r--r--   0 eve        (501) staff       (20)     3147 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/module.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.594779 web3-6.7.0/web3/_utils/module_testing/
--rw-r--r--   0 eve        (501) staff       (20)      539 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/module_testing/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)   179917 2023-07-26 18:36:00.000000 web3-6.7.0/web3/_utils/module_testing/eth_module.py
--rw-r--r--   0 eve        (501) staff       (20)     3406 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/module_testing/go_ethereum_admin_module.py
--rw-r--r--   0 eve        (501) staff       (20)    10432 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/module_testing/go_ethereum_personal_module.py
--rw-r--r--   0 eve        (501) staff       (20)     1176 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
--rw-r--r--   0 eve        (501) staff       (20)     4825 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/module_testing/module_testing_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1272 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/module_testing/net_module.py
--rw-r--r--   0 eve        (501) staff       (20)     9613 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/module_testing/web3_module.py
--rw-r--r--   0 eve        (501) staff       (20)     7447 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/normalizers.py
--rw-r--r--   0 eve        (501) staff       (20)     8833 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/request.py
--rw-r--r--   0 eve        (501) staff       (20)     9611 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/rpc_abi.py
--rw-r--r--   0 eve        (501) staff       (20)     4207 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/threads.py
--rw-r--r--   0 eve        (501) staff       (20)     8737 2023-07-07 17:27:16.000000 web3-6.7.0/web3/_utils/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      816 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/type_conversion.py
--rw-r--r--   0 eve        (501) staff       (20)     2279 2023-07-26 18:35:55.000000 web3-6.7.0/web3/_utils/utility_methods.py
--rw-r--r--   0 eve        (501) staff       (20)     6291 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/validation.py
--rw-r--r--   0 eve        (501) staff       (20)      994 2023-06-26 17:45:20.000000 web3-6.7.0/web3/_utils/windows.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.595146 web3-6.7.0/web3/auto/
--rw-r--r--   0 eve        (501) staff       (20)       44 2023-06-26 17:45:20.000000 web3-6.7.0/web3/auto/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      263 2023-07-26 18:35:55.000000 web3-6.7.0/web3/auto/gethdev.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.595646 web3-6.7.0/web3/beacon/
--rw-r--r--   0 eve        (501) staff       (20)       91 2023-06-26 17:45:20.000000 web3-6.7.0/web3/beacon/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1516 2023-06-26 17:45:20.000000 web3-6.7.0/web3/beacon/api_endpoints.py
--rw-r--r--   0 eve        (501) staff       (20)     5421 2023-06-26 17:45:20.000000 web3-6.7.0/web3/beacon/async_beacon.py
--rw-r--r--   0 eve        (501) staff       (20)     4772 2023-06-26 17:45:20.000000 web3-6.7.0/web3/beacon/main.py
--rw-r--r--   0 eve        (501) staff       (20)      396 2023-06-26 17:45:20.000000 web3-6.7.0/web3/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.596310 web3-6.7.0/web3/contract/
--rw-r--r--   0 eve        (501) staff       (20)      215 2023-06-26 17:45:20.000000 web3-6.7.0/web3/contract/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    19820 2023-07-26 18:35:55.000000 web3-6.7.0/web3/contract/async_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    35727 2023-07-26 18:35:55.000000 web3-6.7.0/web3/contract/base_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    18940 2023-07-26 18:35:55.000000 web3-6.7.0/web3/contract/contract.py
--rw-r--r--   0 eve        (501) staff       (20)    12309 2023-07-26 18:35:55.000000 web3-6.7.0/web3/contract/utils.py
--rw-r--r--   0 eve        (501) staff       (20)     9104 2023-07-07 17:27:16.000000 web3-6.7.0/web3/datastructures.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.597072 web3-6.7.0/web3/eth/
--rw-r--r--   0 eve        (501) staff       (20)      166 2023-06-26 17:45:20.000000 web3-6.7.0/web3/eth/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    22466 2023-07-26 18:35:55.000000 web3-6.7.0/web3/eth/async_eth.py
--rw-r--r--   0 eve        (501) staff       (20)     5943 2023-06-26 17:45:20.000000 web3-6.7.0/web3/eth/base_eth.py
--rw-r--r--   0 eve        (501) staff       (20)    19339 2023-07-26 18:35:55.000000 web3-6.7.0/web3/eth/eth.py
--rw-r--r--   0 eve        (501) staff       (20)     6445 2023-07-26 18:35:55.000000 web3-6.7.0/web3/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.597538 web3-6.7.0/web3/gas_strategies/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/gas_strategies/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      352 2023-07-26 18:36:00.000000 web3-6.7.0/web3/gas_strategies/rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     9010 2023-06-26 17:45:20.000000 web3-6.7.0/web3/gas_strategies/time_based.py
--rw-r--r--   0 eve        (501) staff       (20)    11826 2023-06-26 17:45:20.000000 web3-6.7.0/web3/geth.py
--rw-r--r--   0 eve        (501) staff       (20)      198 2023-04-06 21:34:13.000000 web3-6.7.0/web3/logs.py
--rw-r--r--   0 eve        (501) staff       (20)    15049 2023-07-26 18:35:55.000000 web3-6.7.0/web3/main.py
--rw-r--r--   0 eve        (501) staff       (20)    12170 2023-07-26 18:35:55.000000 web3-6.7.0/web3/manager.py
--rw-r--r--   0 eve        (501) staff       (20)     8430 2023-07-07 17:27:26.000000 web3-6.7.0/web3/method.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.601775 web3-6.7.0/web3/middleware/
--rw-r--r--   0 eve        (501) staff       (20)     3848 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      239 2023-04-06 21:34:13.000000 web3-6.7.0/web3/middleware/abi.py
--rw-r--r--   0 eve        (501) staff       (20)     3222 2023-07-07 17:27:16.000000 web3-6.7.0/web3/middleware/async_cache.py
--rw-r--r--   0 eve        (501) staff       (20)     2630 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/attrdict.py
--rw-r--r--   0 eve        (501) staff       (20)     1785 2023-06-26 17:45:20.000000 web3-6.7.0/web3/middleware/buffered_gas_estimate.py
--rw-r--r--   0 eve        (501) staff       (20)    12880 2023-07-07 17:27:16.000000 web3-6.7.0/web3/middleware/cache.py
--rw-r--r--   0 eve        (501) staff       (20)     1167 2023-06-26 17:45:20.000000 web3-6.7.0/web3/middleware/exception_handling.py
--rw-r--r--   0 eve        (501) staff       (20)     4453 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/exception_retry_request.py
--rw-r--r--   0 eve        (501) staff       (20)    21131 2023-06-26 17:45:20.000000 web3-6.7.0/web3/middleware/filter.py
--rw-r--r--   0 eve        (501) staff       (20)     6434 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/fixture.py
--rw-r--r--   0 eve        (501) staff       (20)     5647 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/formatting.py
--rw-r--r--   0 eve        (501) staff       (20)     4317 2023-07-26 18:36:00.000000 web3-6.7.0/web3/middleware/gas_price_strategy.py
--rw-r--r--   0 eve        (501) staff       (20)     1657 2023-06-26 17:45:20.000000 web3-6.7.0/web3/middleware/geth_poa.py
--rw-r--r--   0 eve        (501) staff       (20)     3336 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/names.py
--rw-r--r--   0 eve        (501) staff       (20)      246 2023-06-15 16:48:05.000000 web3-6.7.0/web3/middleware/normalize_request_parameters.py
--rw-r--r--   0 eve        (501) staff       (20)      351 2023-06-15 16:48:05.000000 web3-6.7.0/web3/middleware/pythonic.py
--rw-r--r--   0 eve        (501) staff       (20)     6605 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/signing.py
--rw-r--r--   0 eve        (501) staff       (20)     1014 2023-06-26 17:45:20.000000 web3-6.7.0/web3/middleware/simulate_unmined_transaction.py
--rw-r--r--   0 eve        (501) staff       (20)     3739 2023-06-26 17:45:20.000000 web3-6.7.0/web3/middleware/stalecheck.py
--rw-r--r--   0 eve        (501) staff       (20)     4548 2023-07-26 18:35:55.000000 web3-6.7.0/web3/middleware/validation.py
--rw-r--r--   0 eve        (501) staff       (20)     4516 2023-07-26 18:35:55.000000 web3-6.7.0/web3/module.py
--rw-r--r--   0 eve        (501) staff       (20)     1562 2023-06-26 17:45:20.000000 web3-6.7.0/web3/net.py
--rw-r--r--   0 eve        (501) staff       (20)    21608 2023-07-26 18:35:55.000000 web3-6.7.0/web3/pm.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.603016 web3-6.7.0/web3/providers/
--rw-r--r--   0 eve        (501) staff       (20)      529 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4381 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/async_base.py
--rw-r--r--   0 eve        (501) staff       (20)     2879 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/async_rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     3447 2023-07-12 20:46:12.000000 web3-6.7.0/web3/providers/auto.py
--rw-r--r--   0 eve        (501) staff       (20)     4149 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.603844 web3-6.7.0/web3/providers/eth_tester/
--rw-r--r--   0 eve        (501) staff       (20)       97 2023-06-26 17:45:20.000000 web3-6.7.0/web3/providers/eth_tester/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    14740 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/eth_tester/defaults.py
--rw-r--r--   0 eve        (501) staff       (20)     5512 2023-07-07 17:27:16.000000 web3-6.7.0/web3/providers/eth_tester/main.py
--rw-r--r--   0 eve        (501) staff       (20)    12861 2023-07-07 17:27:16.000000 web3-6.7.0/web3/providers/eth_tester/middleware.py
--rw-r--r--   0 eve        (501) staff       (20)     6374 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/ipc.py
--rw-r--r--   0 eve        (501) staff       (20)     6513 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/persistent.py
--rw-r--r--   0 eve        (501) staff       (20)     2686 2023-06-26 17:45:20.000000 web3-6.7.0/web3/providers/rpc.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.604420 web3-6.7.0/web3/providers/websocket/
--rw-r--r--   0 eve        (501) staff       (20)      133 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/websocket/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3929 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/websocket/websocket.py
--rw-r--r--   0 eve        (501) staff       (20)     3809 2023-07-26 18:35:55.000000 web3-6.7.0/web3/providers/websocket/websocket_v2.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.604548 web3-6.7.0/web3/scripts/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/scripts/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.604722 web3-6.7.0/web3/scripts/release/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/scripts/release/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1534 2023-06-26 17:45:20.000000 web3-6.7.0/web3/scripts/release/test_package.py
--rw-r--r--   0 eve        (501) staff       (20)      951 2023-04-06 21:34:13.000000 web3-6.7.0/web3/testing.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.604866 web3-6.7.0/web3/tools/
--rw-r--r--   0 eve        (501) staff       (20)       73 2023-04-06 21:34:13.000000 web3-6.7.0/web3/tools/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.605765 web3-6.7.0/web3/tools/benchmark/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/tools/benchmark/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5886 2023-07-20 21:55:14.000000 web3-6.7.0/web3/tools/benchmark/main.py
--rw-r--r--   0 eve        (501) staff       (20)     3435 2023-07-26 18:35:55.000000 web3-6.7.0/web3/tools/benchmark/node.py
--rw-r--r--   0 eve        (501) staff       (20)      912 2023-06-26 17:45:20.000000 web3-6.7.0/web3/tools/benchmark/reporting.py
--rw-r--r--   0 eve        (501) staff       (20)     1722 2023-07-20 21:55:14.000000 web3-6.7.0/web3/tools/benchmark/utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.606789 web3-6.7.0/web3/tools/pytest_ethereum/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.7.0/web3/tools/pytest_ethereum/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4158 2023-06-26 17:45:20.000000 web3-6.7.0/web3/tools/pytest_ethereum/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1423 2023-06-26 17:45:20.000000 web3-6.7.0/web3/tools/pytest_ethereum/deployer.py
--rw-r--r--   0 eve        (501) staff       (20)      380 2023-04-06 21:34:13.000000 web3-6.7.0/web3/tools/pytest_ethereum/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)     3927 2023-06-26 17:45:20.000000 web3-6.7.0/web3/tools/pytest_ethereum/linker.py
--rw-r--r--   0 eve        (501) staff       (20)      645 2023-06-26 17:45:20.000000 web3-6.7.0/web3/tools/pytest_ethereum/plugins.py
--rw-r--r--   0 eve        (501) staff       (20)     2968 2023-07-07 17:27:16.000000 web3-6.7.0/web3/tracing.py
--rw-r--r--   0 eve        (501) staff       (20)    12459 2023-07-26 18:35:55.000000 web3-6.7.0/web3/types.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.607829 web3-6.7.0/web3/utils/
--rw-r--r--   0 eve        (501) staff       (20)      454 2023-06-26 17:45:20.000000 web3-6.7.0/web3/utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      498 2023-06-26 17:45:20.000000 web3-6.7.0/web3/utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      967 2023-06-26 17:45:20.000000 web3-6.7.0/web3/utils/address.py
--rw-r--r--   0 eve        (501) staff       (20)     3096 2023-06-26 17:45:20.000000 web3-6.7.0/web3/utils/async_exception_handling.py
--rw-r--r--   0 eve        (501) staff       (20)     1662 2023-07-26 18:35:55.000000 web3-6.7.0/web3/utils/caching.py
--rw-r--r--   0 eve        (501) staff       (20)     3052 2023-06-26 17:45:20.000000 web3-6.7.0/web3/utils/exception_handling.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 18:44:05.581031 web3-6.7.0/web3.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     2198 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)    10038 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)       64 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/entry_points.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)     1139 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       15 2023-07-26 18:44:05.000000 web3-6.7.0/web3.egg-info/top_level.txt
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.648816 web3-6.8.0/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1090 2023-07-12 17:40:11.000000 web3-6.8.0/LICENSE
+-rw-r--r--   0 fselmo     (501) staff       (20)      249 2023-07-25 23:52:38.000000 web3-6.8.0/MANIFEST.in
+-rw-r--r--   0 fselmo     (501) staff       (20)     2198 2023-08-02 17:57:26.648202 web3-6.8.0/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     1294 2023-07-06 23:00:21.000000 web3-6.8.0/README.md
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.242064 web3-6.8.0/ens/
+-rw-r--r--   0 fselmo     (501) staff       (20)      285 2023-07-11 21:56:12.000000 web3-6.8.0/ens/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17017 2023-07-12 17:40:11.000000 web3-6.8.0/ens/_normalization.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    34745 2023-07-12 17:40:11.000000 web3-6.8.0/ens/abis.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    22277 2023-07-25 23:52:38.000000 web3-6.8.0/ens/async_ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       41 2023-07-06 23:00:21.000000 web3-6.8.0/ens/auto.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3477 2023-07-12 22:07:02.000000 web3-6.8.0/ens/base_ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      913 2023-07-25 23:52:38.000000 web3-6.8.0/ens/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)   148604 2023-07-25 23:52:38.000000 web3-6.8.0/ens/contract_data.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    21517 2023-07-25 23:52:38.000000 web3-6.8.0/ens/ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2390 2023-07-06 23:00:21.000000 web3-6.8.0/ens/exceptions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.244072 web3-6.8.0/ens/specs/
+-rw-r--r--   0 fselmo     (501) staff       (20)    48402 2023-07-12 17:40:11.000000 web3-6.8.0/ens/specs/nf.json
+-rw-r--r--   0 fselmo     (501) staff       (20)  3115333 2023-07-12 17:40:11.000000 web3-6.8.0/ens/specs/normalization_spec.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     9279 2023-07-12 22:07:02.000000 web3-6.8.0/ens/utils.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.264899 web3-6.8.0/ethpm/
+-rw-r--r--   0 fselmo     (501) staff       (20)      580 2023-07-12 17:40:11.000000 web3-6.8.0/ethpm/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.271158 web3-6.8.0/ethpm/_utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/_utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2511 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/_utils/backend.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1477 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/_utils/cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2848 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/_utils/chains.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1030 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/_utils/contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5263 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/_utils/deployments.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2717 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/_utils/ipfs.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.272313 web3-6.8.0/ethpm/_utils/protobuf/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-11-22 17:31:20.000000 web3-6.8.0/ethpm/_utils/protobuf/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1938 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1488 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/_utils/registry.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.273326 web3-6.8.0/ethpm/assets/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.273989 web3-6.8.0/ethpm/assets/ens/
+-rw-r--r--   0 fselmo     (501) staff       (20)    74682 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/ens/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.275426 web3-6.8.0/ethpm/assets/escrow/
+-rw-r--r--   0 fselmo     (501) staff       (20)     8007 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/escrow/with_bytecode_v3.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      760 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/assets/ipfs_file.proto
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.276720 web3-6.8.0/ethpm/assets/owned/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2655 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/owned/output_v3.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      746 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/owned/with_contract_type_v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.282218 web3-6.8.0/ethpm/assets/registry/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.289897 web3-6.8.0/ethpm/assets/registry/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3129 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/Authority.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     2876 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     6380 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/PackageDB.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    10553 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     2966 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     9041 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/ReleaseDB.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     4980 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     1046 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/solc_input.json
+-rw-r--r--   0 fselmo     (501) staff       (20)   727775 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/registry/solc_output.json
+-rw-r--r--   0 fselmo     (501) staff       (20)   270218 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/registry/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.290569 web3-6.8.0/ethpm/assets/safe-math-lib/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2845 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.294312 web3-6.8.0/ethpm/assets/simple-registry/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.297167 web3-6.8.0/ethpm/assets/simple-registry/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1841 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/simple-registry/contracts/Ownable.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    12350 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     3278 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      950 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/simple-registry/solc_input.json
+-rw-r--r--   0 fselmo     (501) staff       (20)   199338 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/simple-registry/solc_output.json
+-rw-r--r--   0 fselmo     (501) staff       (20)    75677 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/simple-registry/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.298782 web3-6.8.0/ethpm/assets/standard-token/
+-rw-r--r--   0 fselmo     (501) staff       (20)    22292 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/standard-token/output_v3.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     8765 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/assets/standard-token/with_bytecode_v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.302379 web3-6.8.0/ethpm/assets/vyper_registry/
+-rw-r--r--   0 fselmo     (501) staff       (20)    81363 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/vyper_registry/0.1.0.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     6339 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/vyper_registry/registry.vy
+-rw-r--r--   0 fselmo     (501) staff       (20)     7596 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/assets/vyper_registry/registry_with_delete.vy
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.308548 web3-6.8.0/ethpm/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/backends/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      956 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/backends/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3006 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/backends/http.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6551 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/backends/ipfs.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4174 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/backends/registry.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      405 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6303 2023-07-12 17:40:11.000000 web3-6.8.0/ethpm/contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1890 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/dependencies.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2134 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/deployments.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.225583 web3-6.8.0/ethpm/ethpm-spec/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.225168 web3-6.8.0/ethpm/ethpm-spec/examples/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.313359 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/
+-rw-r--r--   0 fselmo     (501) staff       (20)     6810 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5361 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.315519 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      888 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      644 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    11598 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     8669 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/escrow/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.319173 web3-6.8.0/ethpm/ethpm-spec/examples/owned/
+-rw-r--r--   0 fselmo     (501) staff       (20)      544 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      443 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.319971 web3-6.8.0/ethpm/ethpm-spec/examples/owned/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      222 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      728 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      478 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/owned/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.324868 web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/
+-rw-r--r--   0 fselmo     (501) staff       (20)     5272 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5030 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5220 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     4993 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.329500 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3976 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     3143 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.331804 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      802 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     5517 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     3289 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.336326 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3794 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     3238 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.338563 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1155 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     2949 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    17129 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     6100 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.343719 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/
+-rw-r--r--   0 fselmo     (501) staff       (20)      590 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      507 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.344500 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      396 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      786 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      548 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/transferable/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.351186 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/
+-rw-r--r--   0 fselmo     (501) staff       (20)     6669 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5456 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.359732 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1454 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     9710 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     7326 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.356106 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/
+-rw-r--r--   0 fselmo     (501) staff       (20)     8052 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     6657 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.358482 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      621 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    12191 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     9503 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.362310 web3-6.8.0/ethpm/ethpm-spec/spec/
+-rw-r--r--   0 fselmo     (501) staff       (20)    10302 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/spec/package.spec.json
+-rw-r--r--   0 fselmo     (501) staff       (20)    12879 2023-01-03 18:30:11.000000 web3-6.8.0/ethpm/ethpm-spec/spec/v3.spec.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     1194 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14494 2023-07-26 18:18:03.000000 web3-6.8.0/ethpm/package.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.367293 web3-6.8.0/ethpm/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)      103 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/tools/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    27045 2023-07-26 18:18:03.000000 web3-6.8.0/ethpm/tools/builder.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    10373 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/tools/checker.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      475 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/tools/get_manifest.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4368 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/uri.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.376884 web3-6.8.0/ethpm/validation/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.8.0/ethpm/validation/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4716 2023-03-13 21:36:03.000000 web3-6.8.0/ethpm/validation/manifest.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1072 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/validation/misc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2317 2022-08-03 17:01:33.000000 web3-6.8.0/ethpm/validation/package.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4873 2023-07-06 23:00:21.000000 web3-6.8.0/ethpm/validation/uri.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1202 2023-07-06 23:00:21.000000 web3-6.8.0/pyproject.toml
+-rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-08-02 17:57:26.648984 web3-6.8.0/setup.cfg
+-rw-r--r--   0 fselmo     (501) staff       (20)     3076 2023-08-02 17:56:53.000000 web3-6.8.0/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.409620 web3-6.8.0/web3/
+-rw-r--r--   0 fselmo     (501) staff       (20)      804 2023-07-25 23:52:38.000000 web3-6.8.0/web3/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.505256 web3-6.8.0/web3/_utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.8.0/web3/_utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    31000 2023-07-12 22:07:02.000000 web3-6.8.0/web3/_utils/abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      456 2023-07-28 20:52:39.000000 web3-6.8.0/web3/_utils/async_caching.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8123 2023-07-12 17:40:11.000000 web3-6.8.0/web3/_utils/async_transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2059 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1489 2023-07-28 19:11:51.000000 web3-6.8.0/web3/_utils/caching.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.506330 web3-6.8.0/web3/_utils/compat/
+-rw-r--r--   0 fselmo     (501) staff       (20)      606 2023-08-02 17:52:22.000000 web3-6.8.0/web3/_utils/compat/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5425 2023-07-25 23:52:38.000000 web3-6.8.0/web3/_utils/contract_error_handling.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.508020 web3-6.8.0/web3/_utils/contract_sources/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6492 2023-07-12 17:40:11.000000 web3-6.8.0/web3/_utils/contract_sources/compile_contracts.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.530109 web3-6.8.0/web3/_utils/contract_sources/contract_data/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      517 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5344 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/address_reflector.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    18852 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14783 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6089 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6334 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    37881 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5573 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/event_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15824 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1651 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7637 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/math_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    16716 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    32645 2023-07-07 18:03:19.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15579 2023-07-12 17:40:11.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/panic_errors_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1825 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/payable_tester.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17290 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5264 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4264 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/revert_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3555 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8238 2023-07-12 17:40:11.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/storage_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11586 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/string_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    23180 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14980 2023-07-07 21:28:03.000000 web3-6.8.0/web3/_utils/contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1640 2023-03-13 21:36:03.000000 web3-6.8.0/web3/_utils/datatypes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1738 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/decorators.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      144 2023-03-13 21:36:03.000000 web3-6.8.0/web3/_utils/empty.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9065 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/encoding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2388 2023-07-12 22:07:02.000000 web3-6.8.0/web3/_utils/ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17198 2023-07-12 17:40:11.000000 web3-6.8.0/web3/_utils/events.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2113 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/fee_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11886 2023-07-07 21:28:03.000000 web3-6.8.0/web3/_utils/filters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3071 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/formatters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       55 2022-01-11 17:23:55.000000 web3-6.8.0/web3/_utils/function_identifiers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      195 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/http.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-03-13 21:36:03.000000 web3-6.8.0/web3/_utils/hypothesis.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1047 2023-03-13 21:36:03.000000 web3-6.8.0/web3/_utils/math.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    31322 2023-07-25 23:52:38.000000 web3-6.8.0/web3/_utils/method_formatters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1146 2023-03-13 21:36:03.000000 web3-6.8.0/web3/_utils/miner.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3147 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/module.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.538311 web3-6.8.0/web3/_utils/module_testing/
+-rw-r--r--   0 fselmo     (501) staff       (20)      539 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)   179917 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/eth_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3406 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/go_ethereum_admin_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    10432 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/go_ethereum_personal_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1176 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4825 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/module_testing_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1272 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/net_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9613 2023-07-28 20:36:45.000000 web3-6.8.0/web3/_utils/module_testing/web3_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7447 2023-07-12 22:07:02.000000 web3-6.8.0/web3/_utils/normalizers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8833 2023-07-14 19:57:51.000000 web3-6.8.0/web3/_utils/request.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9611 2023-07-26 20:43:07.000000 web3-6.8.0/web3/_utils/rpc_abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4207 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/threads.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8737 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      816 2023-07-06 23:00:21.000000 web3-6.8.0/web3/_utils/type_conversion.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2279 2023-07-25 23:52:38.000000 web3-6.8.0/web3/_utils/utility_methods.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6291 2023-07-07 21:28:03.000000 web3-6.8.0/web3/_utils/validation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      994 2023-03-13 21:36:03.000000 web3-6.8.0/web3/_utils/windows.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.539453 web3-6.8.0/web3/auto/
+-rw-r--r--   0 fselmo     (501) staff       (20)       44 2023-07-06 23:00:21.000000 web3-6.8.0/web3/auto/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      263 2023-02-18 04:25:14.000000 web3-6.8.0/web3/auto/gethdev.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.544723 web3-6.8.0/web3/beacon/
+-rw-r--r--   0 fselmo     (501) staff       (20)       91 2023-07-06 23:00:21.000000 web3-6.8.0/web3/beacon/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1516 2023-07-06 23:00:21.000000 web3-6.8.0/web3/beacon/api_endpoints.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5421 2023-07-06 23:00:21.000000 web3-6.8.0/web3/beacon/async_beacon.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4772 2023-07-06 23:00:21.000000 web3-6.8.0/web3/beacon/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      396 2023-03-13 21:36:03.000000 web3-6.8.0/web3/constants.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.550382 web3-6.8.0/web3/contract/
+-rw-r--r--   0 fselmo     (501) staff       (20)      215 2023-07-06 23:00:21.000000 web3-6.8.0/web3/contract/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    19820 2023-07-12 17:40:11.000000 web3-6.8.0/web3/contract/async_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    35727 2023-07-12 17:40:11.000000 web3-6.8.0/web3/contract/base_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    18940 2023-07-12 17:40:11.000000 web3-6.8.0/web3/contract/contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12309 2023-07-12 17:40:11.000000 web3-6.8.0/web3/contract/utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9104 2023-07-06 23:00:21.000000 web3-6.8.0/web3/datastructures.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.556244 web3-6.8.0/web3/eth/
+-rw-r--r--   0 fselmo     (501) staff       (20)      166 2023-07-06 23:00:21.000000 web3-6.8.0/web3/eth/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    22529 2023-08-01 21:40:11.000000 web3-6.8.0/web3/eth/async_eth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5943 2023-07-06 23:00:21.000000 web3-6.8.0/web3/eth/base_eth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    19339 2023-07-12 17:40:11.000000 web3-6.8.0/web3/eth/eth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6445 2023-07-17 22:10:32.000000 web3-6.8.0/web3/exceptions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.560231 web3-6.8.0/web3/gas_strategies/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.8.0/web3/gas_strategies/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      352 2023-07-26 18:18:03.000000 web3-6.8.0/web3/gas_strategies/rpc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9010 2023-07-06 23:00:21.000000 web3-6.8.0/web3/gas_strategies/time_based.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11826 2023-07-06 23:00:21.000000 web3-6.8.0/web3/geth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      198 2022-09-26 17:05:32.000000 web3-6.8.0/web3/logs.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15445 2023-08-01 21:40:11.000000 web3-6.8.0/web3/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12170 2023-07-28 19:11:19.000000 web3-6.8.0/web3/manager.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8430 2023-07-18 03:17:32.000000 web3-6.8.0/web3/method.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.615386 web3-6.8.0/web3/middleware/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3848 2023-07-12 22:07:02.000000 web3-6.8.0/web3/middleware/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      239 2023-01-31 22:25:40.000000 web3-6.8.0/web3/middleware/abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3222 2023-07-14 19:57:51.000000 web3-6.8.0/web3/middleware/async_cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2630 2023-07-25 23:52:38.000000 web3-6.8.0/web3/middleware/attrdict.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1785 2023-07-06 23:00:21.000000 web3-6.8.0/web3/middleware/buffered_gas_estimate.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12880 2023-07-12 17:40:11.000000 web3-6.8.0/web3/middleware/cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1167 2023-03-13 21:36:03.000000 web3-6.8.0/web3/middleware/exception_handling.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4453 2023-07-12 17:40:11.000000 web3-6.8.0/web3/middleware/exception_retry_request.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    21131 2023-07-06 23:00:21.000000 web3-6.8.0/web3/middleware/filter.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6434 2023-07-25 23:52:38.000000 web3-6.8.0/web3/middleware/fixture.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5647 2023-07-25 23:52:38.000000 web3-6.8.0/web3/middleware/formatting.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4317 2023-07-26 18:18:03.000000 web3-6.8.0/web3/middleware/gas_price_strategy.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1657 2023-07-18 20:58:19.000000 web3-6.8.0/web3/middleware/geth_poa.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4087 2023-08-02 16:21:06.000000 web3-6.8.0/web3/middleware/names.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      246 2022-12-08 21:12:34.000000 web3-6.8.0/web3/middleware/normalize_request_parameters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      351 2023-02-03 21:22:38.000000 web3-6.8.0/web3/middleware/pythonic.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6605 2023-07-26 20:30:08.000000 web3-6.8.0/web3/middleware/signing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1014 2023-07-06 23:00:21.000000 web3-6.8.0/web3/middleware/simulate_unmined_transaction.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3739 2023-07-06 23:00:21.000000 web3-6.8.0/web3/middleware/stalecheck.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4548 2023-07-12 22:07:02.000000 web3-6.8.0/web3/middleware/validation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4516 2023-07-25 23:52:38.000000 web3-6.8.0/web3/module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1562 2023-03-13 21:36:03.000000 web3-6.8.0/web3/net.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    21608 2023-07-26 18:18:03.000000 web3-6.8.0/web3/pm.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.621899 web3-6.8.0/web3/providers/
+-rw-r--r--   0 fselmo     (501) staff       (20)      529 2023-07-25 23:52:38.000000 web3-6.8.0/web3/providers/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4381 2023-07-25 23:52:38.000000 web3-6.8.0/web3/providers/async_base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2879 2023-07-12 17:40:11.000000 web3-6.8.0/web3/providers/async_rpc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3447 2023-07-06 23:00:21.000000 web3-6.8.0/web3/providers/auto.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4149 2023-07-25 23:52:38.000000 web3-6.8.0/web3/providers/base.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.626572 web3-6.8.0/web3/providers/eth_tester/
+-rw-r--r--   0 fselmo     (501) staff       (20)       97 2023-07-06 23:00:21.000000 web3-6.8.0/web3/providers/eth_tester/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14740 2023-07-12 22:07:02.000000 web3-6.8.0/web3/providers/eth_tester/defaults.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5861 2023-08-02 17:52:22.000000 web3-6.8.0/web3/providers/eth_tester/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12861 2023-07-19 14:33:01.000000 web3-6.8.0/web3/providers/eth_tester/middleware.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6374 2023-07-25 23:52:38.000000 web3-6.8.0/web3/providers/ipc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6513 2023-07-28 19:11:19.000000 web3-6.8.0/web3/providers/persistent.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2686 2023-03-13 21:36:03.000000 web3-6.8.0/web3/providers/rpc.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.628504 web3-6.8.0/web3/providers/websocket/
+-rw-r--r--   0 fselmo     (501) staff       (20)      133 2023-07-25 23:52:38.000000 web3-6.8.0/web3/providers/websocket/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3929 2023-07-25 23:52:38.000000 web3-6.8.0/web3/providers/websocket/websocket.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4529 2023-08-01 21:40:11.000000 web3-6.8.0/web3/providers/websocket/websocket_v2.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.8.0/web3/py.typed
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.629023 web3-6.8.0/web3/scripts/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.8.0/web3/scripts/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.629785 web3-6.8.0/web3/scripts/release/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.8.0/web3/scripts/release/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1534 2023-03-13 21:36:03.000000 web3-6.8.0/web3/scripts/release/test_package.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      951 2023-03-13 21:36:03.000000 web3-6.8.0/web3/testing.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.630519 web3-6.8.0/web3/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)       73 2022-09-26 17:05:32.000000 web3-6.8.0/web3/tools/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.634053 web3-6.8.0/web3/tools/benchmark/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-08-03 17:01:33.000000 web3-6.8.0/web3/tools/benchmark/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5886 2023-07-06 23:00:21.000000 web3-6.8.0/web3/tools/benchmark/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3435 2023-07-12 17:40:11.000000 web3-6.8.0/web3/tools/benchmark/node.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      912 2023-03-13 21:36:03.000000 web3-6.8.0/web3/tools/benchmark/reporting.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1722 2023-02-13 20:41:33.000000 web3-6.8.0/web3/tools/benchmark/utils.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.639370 web3-6.8.0/web3/tools/pytest_ethereum/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.8.0/web3/tools/pytest_ethereum/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4158 2023-07-06 23:00:21.000000 web3-6.8.0/web3/tools/pytest_ethereum/_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1423 2023-07-06 23:00:21.000000 web3-6.8.0/web3/tools/pytest_ethereum/deployer.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      380 2021-11-01 21:09:29.000000 web3-6.8.0/web3/tools/pytest_ethereum/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3927 2023-03-13 21:36:03.000000 web3-6.8.0/web3/tools/pytest_ethereum/linker.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      645 2023-07-06 23:00:21.000000 web3-6.8.0/web3/tools/pytest_ethereum/plugins.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2968 2023-07-06 23:00:21.000000 web3-6.8.0/web3/tracing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12396 2023-08-02 17:52:22.000000 web3-6.8.0/web3/types.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.647210 web3-6.8.0/web3/utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)      454 2023-07-06 23:00:21.000000 web3-6.8.0/web3/utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      498 2023-03-13 21:36:03.000000 web3-6.8.0/web3/utils/abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      967 2023-07-06 23:00:21.000000 web3-6.8.0/web3/utils/address.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3096 2023-07-06 23:00:21.000000 web3-6.8.0/web3/utils/async_exception_handling.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1662 2023-07-25 23:52:38.000000 web3-6.8.0/web3/utils/caching.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3052 2023-07-06 23:00:21.000000 web3-6.8.0/web3/utils/exception_handling.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-08-02 17:57:26.420290 web3-6.8.0/web3.egg-info/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2198 2023-08-02 17:57:26.000000 web3-6.8.0/web3.egg-info/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)    10038 2023-08-02 17:57:26.000000 web3-6.8.0/web3.egg-info/SOURCES.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-08-02 17:57:26.000000 web3-6.8.0/web3.egg-info/dependency_links.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       64 2023-08-02 17:57:26.000000 web3-6.8.0/web3.egg-info/entry_points.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-07-18 23:06:02.000000 web3-6.8.0/web3.egg-info/not-zip-safe
+-rw-r--r--   0 fselmo     (501) staff       (20)     1139 2023-08-02 17:57:26.000000 web3-6.8.0/web3.egg-info/requires.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       15 2023-08-02 17:57:26.000000 web3-6.8.0/web3.egg-info/top_level.txt
```

### Comparing `web3-6.7.0/LICENSE` & `web3-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/PKG-INFO` & `web3-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.7.0
+Version: 6.8.0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.7.0/README.md` & `web3-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/_normalization.py` & `web3-6.8.0/ens/_normalization.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/abis.py` & `web3-6.8.0/ens/abis.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/async_ens.py` & `web3-6.8.0/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/base_ens.py` & `web3-6.8.0/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/constants.py` & `web3-6.8.0/ens/constants.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/contract_data.py` & `web3-6.8.0/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/ens.py` & `web3-6.8.0/ens/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/exceptions.py` & `web3-6.8.0/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/specs/nf.json` & `web3-6.8.0/ens/specs/nf.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/specs/normalization_spec.json` & `web3-6.8.0/ens/specs/normalization_spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ens/utils.py` & `web3-6.8.0/ens/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/__init__.py` & `web3-6.8.0/ethpm/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/backend.py` & `web3-6.8.0/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/cache.py` & `web3-6.8.0/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/chains.py` & `web3-6.8.0/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/contract.py` & `web3-6.8.0/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/deployments.py` & `web3-6.8.0/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/ipfs.py` & `web3-6.8.0/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `web3-6.8.0/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/_utils/registry.py` & `web3-6.8.0/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/ens/v3.json` & `web3-6.8.0/ethpm/assets/ens/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/escrow/with_bytecode_v3.json` & `web3-6.8.0/ethpm/assets/escrow/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/ipfs_file.proto` & `web3-6.8.0/ethpm/assets/ipfs_file.proto`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/owned/output_v3.json` & `web3-6.8.0/ethpm/assets/owned/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/owned/with_contract_type_v3.json` & `web3-6.8.0/ethpm/assets/owned/with_contract_type_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/Authority.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/Authority.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/PackageDB.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/PackageDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/PackageRegistry.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/ReleaseDB.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/ReleaseDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/contracts/ReleaseValidator.sol` & `web3-6.8.0/ethpm/assets/registry/contracts/ReleaseValidator.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/solc_input.json` & `web3-6.8.0/ethpm/assets/registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/solc_output.json` & `web3-6.8.0/ethpm/assets/registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/registry/v3.json` & `web3-6.8.0/ethpm/assets/registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json` & `web3-6.8.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/simple-registry/contracts/Ownable.sol` & `web3-6.8.0/ethpm/assets/simple-registry/contracts/Ownable.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol` & `web3-6.8.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol` & `web3-6.8.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/simple-registry/solc_input.json` & `web3-6.8.0/ethpm/assets/simple-registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/simple-registry/solc_output.json` & `web3-6.8.0/ethpm/assets/simple-registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/simple-registry/v3.json` & `web3-6.8.0/ethpm/assets/simple-registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/standard-token/output_v3.json` & `web3-6.8.0/ethpm/assets/standard-token/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/standard-token/with_bytecode_v3.json` & `web3-6.8.0/ethpm/assets/standard-token/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/vyper_registry/0.1.0.json` & `web3-6.8.0/ethpm/assets/vyper_registry/0.1.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/vyper_registry/registry.vy` & `web3-6.8.0/ethpm/assets/vyper_registry/registry.vy`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/assets/vyper_registry/registry_with_delete.vy` & `web3-6.8.0/ethpm/assets/vyper_registry/registry_with_delete.vy`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/backends/base.py` & `web3-6.8.0/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/backends/http.py` & `web3-6.8.0/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/backends/ipfs.py` & `web3-6.8.0/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/backends/registry.py` & `web3-6.8.0/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/contract.py` & `web3-6.8.0/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/dependencies.py` & `web3-6.8.0/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/deployments.py` & `web3-6.8.0/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/escrow/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/escrow/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/piper-coin/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/piper-coin/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/standard-token/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/standard-token/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/transferable/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/transferable/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json` & `web3-6.8.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/spec/package.spec.json` & `web3-6.8.0/ethpm/ethpm-spec/spec/package.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/ethpm-spec/spec/v3.spec.json` & `web3-6.8.0/ethpm/ethpm-spec/spec/v3.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/exceptions.py` & `web3-6.8.0/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/package.py` & `web3-6.8.0/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/tools/builder.py` & `web3-6.8.0/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/tools/checker.py` & `web3-6.8.0/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/uri.py` & `web3-6.8.0/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/validation/manifest.py` & `web3-6.8.0/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/validation/misc.py` & `web3-6.8.0/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/validation/package.py` & `web3-6.8.0/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/ethpm/validation/uri.py` & `web3-6.8.0/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/pyproject.toml` & `web3-6.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/setup.py` & `web3-6.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="web3",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="6.7.0",
+    version="6.8.0",
     description="""web3.py""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/web3.py",
     include_package_data=True,
```

### Comparing `web3-6.7.0/web3/__init__.py` & `web3-6.8.0/web3/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/abi.py` & `web3-6.8.0/web3/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/async_transactions.py` & `web3-6.8.0/web3/_utils/async_transactions.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/blocks.py` & `web3-6.8.0/web3/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/caching.py` & `web3-6.8.0/web3/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/compat/__init__.py` & `web3-6.8.0/web3/_utils/compat/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 # or use the back-ported version of the type.
 
 # Once web3 supports >= the noted python version, the type may be directly
 # imported from `typing`
 
 from typing_extensions import (  # noqa: F401
     Literal,  # py38
+    NotRequired,  # py311
     Protocol,  # py38
     TypedDict,  # py38
     Self,  # py311
 )
```

### Comparing `web3-6.7.0/web3/_utils/contract_error_handling.py` & `web3-6.8.0/web3/_utils/contract_error_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/compile_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/address_reflector.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/arrays_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/arrays_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/emitter_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/event_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/extended_resolver.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/math_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/math_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/panic_errors_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/panic_errors_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/payable_tester.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/payable_tester.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/revert_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/revert_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/simple_resolver.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/simple_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/storage_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/storage_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/string_contract.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/string_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py` & `web3-6.8.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/contracts.py` & `web3-6.8.0/web3/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/datatypes.py` & `web3-6.8.0/web3/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/decorators.py` & `web3-6.8.0/web3/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/encoding.py` & `web3-6.8.0/web3/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/ens.py` & `web3-6.8.0/web3/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/events.py` & `web3-6.8.0/web3/_utils/events.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/fee_utils.py` & `web3-6.8.0/web3/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/filters.py` & `web3-6.8.0/web3/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/formatters.py` & `web3-6.8.0/web3/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/math.py` & `web3-6.8.0/web3/_utils/math.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/method_formatters.py` & `web3-6.8.0/web3/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/miner.py` & `web3-6.8.0/web3/_utils/miner.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module.py` & `web3-6.8.0/web3/_utils/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/__init__.py` & `web3-6.8.0/web3/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/eth_module.py` & `web3-6.8.0/web3/_utils/module_testing/eth_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/go_ethereum_admin_module.py` & `web3-6.8.0/web3/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/go_ethereum_personal_module.py` & `web3-6.8.0/web3/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/go_ethereum_txpool_module.py` & `web3-6.8.0/web3/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/module_testing_utils.py` & `web3-6.8.0/web3/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/net_module.py` & `web3-6.8.0/web3/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/module_testing/web3_module.py` & `web3-6.8.0/web3/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/normalizers.py` & `web3-6.8.0/web3/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/request.py` & `web3-6.8.0/web3/_utils/request.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/rpc_abi.py` & `web3-6.8.0/web3/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/threads.py` & `web3-6.8.0/web3/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/transactions.py` & `web3-6.8.0/web3/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/type_conversion.py` & `web3-6.8.0/web3/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/utility_methods.py` & `web3-6.8.0/web3/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/validation.py` & `web3-6.8.0/web3/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/_utils/windows.py` & `web3-6.8.0/web3/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/beacon/api_endpoints.py` & `web3-6.8.0/web3/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/beacon/async_beacon.py` & `web3-6.8.0/web3/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/beacon/main.py` & `web3-6.8.0/web3/beacon/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/contract/async_contract.py` & `web3-6.8.0/web3/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/contract/base_contract.py` & `web3-6.8.0/web3/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/contract/contract.py` & `web3-6.8.0/web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/contract/utils.py` & `web3-6.8.0/web3/contract/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/datastructures.py` & `web3-6.8.0/web3/datastructures.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/eth/async_eth.py` & `web3-6.8.0/web3/eth/async_eth.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     Nonce,
     SignedTx,
     SubscriptionType,
     SyncStatus,
     TxData,
     TxParams,
     TxReceipt,
-    TxTypeSubscriptionArg,
     Wei,
     _Hash32,
 )
 from web3.utils import (
     async_handle_offchain_lookup,
 )
 
@@ -665,28 +664,31 @@
         mungers=[default_root_munger],
     )
 
     _subscribe_with_args: Method[
         Callable[
             [
                 SubscriptionType,
-                Optional[Union[LogsSubscriptionArg, TxTypeSubscriptionArg]],
+                Optional[Union[LogsSubscriptionArg, bool]],
             ],
             Awaitable[HexStr],
         ]
     ] = Method(
         RPC.eth_subscribe,
         mungers=[default_root_munger],
     )
 
     async def subscribe(
         self,
         subscription_type: SubscriptionType,
         subscription_arg: Optional[
-            Union[LogsSubscriptionArg, TxTypeSubscriptionArg]
+            Union[
+                LogsSubscriptionArg,  # logs, optional filter params
+                bool,  # newPendingTransactions, full_transactions
+            ]
         ] = None,
     ) -> HexStr:
         if not isinstance(self.w3.provider, PersistentConnectionProvider):
             raise MethodUnavailable(
                 "eth_subscribe is only supported with providers that support "
                 "persistent connections."
             )
```

### Comparing `web3-6.7.0/web3/eth/base_eth.py` & `web3-6.8.0/web3/eth/base_eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/eth/eth.py` & `web3-6.8.0/web3/eth/eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/exceptions.py` & `web3-6.8.0/web3/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/gas_strategies/time_based.py` & `web3-6.8.0/web3/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/geth.py` & `web3-6.8.0/web3/geth.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/main.py` & `web3-6.8.0/web3/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     wraps,
 )
 from hexbytes import (
     HexBytes,
 )
 from typing import (
     Any,
+    AsyncIterator,
     Dict,
     List,
     Optional,
     Sequence,
     Type,
     TYPE_CHECKING,
     Union,
@@ -534,14 +535,24 @@
     ) -> None:
         if not isinstance(provider, PersistentConnectionProvider):
             raise Web3ValidationError(
                 "Provider must inherit from PersistentConnectionProvider class."
             )
         AsyncWeb3.__init__(self, provider, middlewares, modules, external_modules, ens)
 
+    # async for w3 in w3.persistent_websocket(provider)
+    async def __aiter__(self) -> AsyncIterator["_PersistentConnectionWeb3"]:
+        while True:
+            try:
+                yield self
+            except Exception:
+                # provider should handle connection / reconnection
+                continue
+
+    # async with w3.persistent_websocket(provider) as w3
     async def __aenter__(self) -> "_PersistentConnectionWeb3":
         await self.provider.connect()
         return self
 
     async def __aexit__(
         self,
         exc_type: Type[BaseException],
```

### Comparing `web3-6.7.0/web3/manager.py` & `web3-6.8.0/web3/manager.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/method.py` & `web3-6.8.0/web3/method.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/__init__.py` & `web3-6.8.0/web3/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/async_cache.py` & `web3-6.8.0/web3/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/attrdict.py` & `web3-6.8.0/web3/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/buffered_gas_estimate.py` & `web3-6.8.0/web3/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/cache.py` & `web3-6.8.0/web3/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/exception_handling.py` & `web3-6.8.0/web3/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/exception_retry_request.py` & `web3-6.8.0/web3/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/filter.py` & `web3-6.8.0/web3/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/fixture.py` & `web3-6.8.0/web3/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/formatting.py` & `web3-6.8.0/web3/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/gas_price_strategy.py` & `web3-6.8.0/web3/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/geth_poa.py` & `web3-6.8.0/web3/middleware/geth_poa.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/names.py` & `web3-6.8.0/web3/middleware/names.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         request_formatters=abi_request_formatters(normalizers, RPC_ABIS)
     )
 
 
 # -- async -- #
 
 
+def _is_logs_subscription_with_optional_args(method: RPCEndpoint, params: Any) -> bool:
+    return method == "eth_subscribe" and len(params) == 2 and params[0] == "logs"
+
+
 async def async_format_all_ens_names_to_address(
     async_web3: "AsyncWeb3",
     abi_types_for_method: Sequence[Any],
     data: Sequence[Any],
 ) -> Sequence[Any]:
     # provide a stepwise version of what the curried formatters do
     abi_typed_params = abi_data_tree(abi_types_for_method, data)
@@ -107,16 +111,31 @@
 
 async def async_name_to_address_middleware(
     make_request: Callable[[RPCEndpoint, Any], Any],
     async_w3: "AsyncWeb3",
 ) -> AsyncMiddlewareCoroutine:
     async def middleware(method: RPCEndpoint, params: Any) -> Any:
         abi_types_for_method = RPC_ABIS.get(method, None)
+
         if abi_types_for_method is not None:
-            params = await async_apply_ens_to_address_conversion(
-                async_w3,
-                params,
-                abi_types_for_method,
-            )
+            if _is_logs_subscription_with_optional_args(method, params):
+                # eth_subscribe optional logs params are unique.
+                # Handle them separately here.
+                (formatted_dict,) = await async_apply_ens_to_address_conversion(
+                    async_w3,
+                    (params[1],),
+                    {
+                        "address": "address",
+                        "topics": "bytes32[]",
+                    },
+                )
+                params = (params[0], formatted_dict)
+
+            else:
+                params = await async_apply_ens_to_address_conversion(
+                    async_w3,
+                    params,
+                    abi_types_for_method,
+                )
         return await make_request(method, params)
 
     return middleware
```

### Comparing `web3-6.7.0/web3/middleware/signing.py` & `web3-6.8.0/web3/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/simulate_unmined_transaction.py` & `web3-6.8.0/web3/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/stalecheck.py` & `web3-6.8.0/web3/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/middleware/validation.py` & `web3-6.8.0/web3/middleware/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/module.py` & `web3-6.8.0/web3/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/net.py` & `web3-6.8.0/web3/net.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/pm.py` & `web3-6.8.0/web3/pm.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/__init__.py` & `web3-6.8.0/web3/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/async_base.py` & `web3-6.8.0/web3/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/async_rpc.py` & `web3-6.8.0/web3/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/auto.py` & `web3-6.8.0/web3/providers/auto.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/base.py` & `web3-6.8.0/web3/providers/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/eth_tester/defaults.py` & `web3-6.8.0/web3/providers/eth_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/eth_tester/main.py` & `web3-6.8.0/web3/providers/eth_tester/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     BaseProvider,
 )
 from web3.providers.async_base import (
     AsyncBaseProvider,
 )
 from web3.types import (
     RPCEndpoint,
+    RPCError,
     RPCResponse,
 )
 
 from .middleware import (
     async_default_transaction_fields_middleware,
     async_ethereum_tester_middleware,
     default_transaction_fields_middleware,
@@ -131,14 +132,27 @@
     def make_request(self, method: RPCEndpoint, params: Any) -> RPCResponse:
         return _make_request(method, params, self.api_endpoints, self.ethereum_tester)
 
     def is_connected(self, show_traceback: bool = False) -> Literal[True]:
         return True
 
 
+def _make_response(result: Any, message: str = "") -> RPCResponse:
+    if isinstance(result, Exception):
+        return RPCResponse(
+            {
+                "id": 1,
+                "jsonrpc": "2.0",
+                "error": RPCError({"code": -32601, "message": message}),
+            }
+        )
+
+    return RPCResponse({"id": 1, "jsonrpc": "2.0", "result": result})
+
+
 def _make_request(
     method: RPCEndpoint,
     params: Any,
     api_endpoints: Dict[str, Dict[str, Any]],
     ethereum_tester_instance: "EthereumTester",
 ) -> RPCResponse:
     # do not import eth_tester derivatives until runtime,
@@ -147,22 +161,20 @@
         TransactionFailed,
     )
 
     namespace, _, endpoint = method.partition("_")
 
     try:
         delegator = api_endpoints[namespace][endpoint]
-    except KeyError:
-        return RPCResponse({"error": f"Unknown RPC Endpoint: {method}"})
+    except KeyError as e:
+        return _make_response(e, f"Unknown RPC Endpoint: {method}")
     try:
         response = delegator(ethereum_tester_instance, params)
-    except NotImplementedError:
-        return RPCResponse(
-            {"error": f"RPC Endpoint has not been implemented: {method}"}
-        )
+    except NotImplementedError as e:
+        return _make_response(e, f"RPC Endpoint has not been implemented: {method}")
     except TransactionFailed as e:
         first_arg = e.args[0]
         try:
             # sometimes eth-tester wraps an exception in another exception
             raw_error_msg = (
                 first_arg if not isinstance(first_arg, Exception) else first_arg.args[0]
             )
@@ -171,10 +183,8 @@
                 if is_bytes(raw_error_msg)
                 else raw_error_msg
             )
         except InsufficientDataBytes:
             reason = first_arg
         raise TransactionFailed(f"execution reverted: {reason}")
     else:
-        return {
-            "result": response,
-        }
+        return _make_response(response)
```

### Comparing `web3-6.7.0/web3/providers/eth_tester/middleware.py` & `web3-6.8.0/web3/providers/eth_tester/middleware.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/ipc.py` & `web3-6.8.0/web3/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/persistent.py` & `web3-6.8.0/web3/providers/persistent.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/rpc.py` & `web3-6.8.0/web3/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/websocket/websocket.py` & `web3-6.8.0/web3/providers/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/providers/websocket/websocket_v2.py` & `web3-6.8.0/web3/providers/websocket/websocket_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 def get_default_endpoint() -> URI:
     return URI(os.environ.get("WEB3_WS_PROVIDER_URI", "ws://127.0.0.1:8546"))
 
 
 class WebsocketProviderV2(PersistentConnectionProvider):
     logger = logging.getLogger("web3.providers.WebsocketProviderV2")
     is_async: bool = True
+    _max_connection_retries: int = 5
 
     def __init__(
         self,
         endpoint_uri: Optional[Union[URI, str]] = None,
         websocket_kwargs: Optional[Dict[str, Any]] = None,
         call_timeout: Optional[int] = None,
     ) -> None:
@@ -90,35 +91,51 @@
         return f"Websocket connection: {self.endpoint_uri}"
 
     async def is_connected(self, show_traceback: bool = False) -> bool:
         if not self.ws:
             return False
 
         try:
-            pong_waiter = await self.ws.ping()
-            await asyncio.wait_for(pong_waiter, timeout=self.call_timeout)
+            await self.ws.pong()
             return True
 
-        except (WebSocketException, asyncio.TimeoutError) as e:
+        except WebSocketException as e:
             if show_traceback:
                 raise ProviderConnectionError(
                     f"Error connecting to endpoint: '{self.endpoint_uri}'"
                 ) from e
             return False
 
     async def connect(self) -> None:
-        try:
-            self.ws = await connect(self.endpoint_uri, **self.websocket_kwargs)
-        except Exception as e:
-            raise ProviderConnectionError(
-                f"Could not connect to endpoint: {self.endpoint_uri}"
-            ) from e
+        _connection_attempts = 0
+        _backoff_rate_change = 1.75
+        _backoff_time = 1.75
+
+        while _connection_attempts != self._max_connection_retries:
+            try:
+                _connection_attempts += 1
+                self.ws = await connect(self.endpoint_uri, **self.websocket_kwargs)
+                break
+            except WebSocketException as e:
+                if _connection_attempts == self._max_connection_retries:
+                    raise ProviderConnectionError(
+                        f"Could not connect to endpoint: {self.endpoint_uri}. "
+                        f"Retries exceeded max of {self._max_connection_retries}."
+                    ) from e
+                self.logger.info(
+                    f"Could not connect to endpoint: {self.endpoint_uri}. Retrying in "
+                    f"{round(_backoff_time, 1)} seconds.",
+                    exc_info=True,
+                )
+                await asyncio.sleep(_backoff_time)
+                _backoff_time *= _backoff_rate_change
 
     async def disconnect(self) -> None:
         await self.ws.close()
+        self.ws = None
 
         # clear the provider request cache after disconnecting
         self._async_response_processing_cache.clear()
 
     async def make_request(self, method: RPCEndpoint, params: Any) -> None:
         request_data = self.encode_rpc_request(method, params)
```

### Comparing `web3-6.7.0/web3/scripts/release/test_package.py` & `web3-6.8.0/web3/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/testing.py` & `web3-6.8.0/web3/testing.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/benchmark/main.py` & `web3-6.8.0/web3/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/benchmark/node.py` & `web3-6.8.0/web3/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/benchmark/reporting.py` & `web3-6.8.0/web3/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/benchmark/utils.py` & `web3-6.8.0/web3/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/pytest_ethereum/_utils.py` & `web3-6.8.0/web3/tools/pytest_ethereum/_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/pytest_ethereum/deployer.py` & `web3-6.8.0/web3/tools/pytest_ethereum/deployer.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/pytest_ethereum/linker.py` & `web3-6.8.0/web3/tools/pytest_ethereum/linker.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tools/pytest_ethereum/plugins.py` & `web3-6.8.0/web3/tools/pytest_ethereum/plugins.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/tracing.py` & `web3-6.8.0/web3/tracing.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/types.py` & `web3-6.8.0/web3/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 )
 from hexbytes import (
     HexBytes,
 )
 
 from web3._utils.compat import (
     Literal,
+    NotRequired,
     TypedDict,
 )
 from web3._utils.function_identifiers import (
     FallbackFn,
     ReceiveFn,
 )
 from web3.datastructures import (
@@ -125,15 +126,15 @@
     transactionHash: HexBytes
     transactionIndex: int
 
 
 class RPCError(TypedDict):
     code: int
     message: str
-    data: Optional[str]
+    data: NotRequired[str]
 
 
 # syntax b/c "from" keyword not allowed w/ class construction
 TxData = TypedDict(
     "TxData",
     {
         "accessList": AccessList,
@@ -542,11 +543,7 @@
     address: Union[
         Address,
         ChecksumAddress,
         ENS,
         Sequence[Union[Address, ChecksumAddress, ENS]],
     ]
     topics: Sequence[Union[HexStr, Sequence[HexStr]]]
-
-
-class TxTypeSubscriptionArg(TypedDict, total=False):
-    full_transactions: bool
```

### Comparing `web3-6.7.0/web3/utils/address.py` & `web3-6.8.0/web3/utils/address.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/utils/async_exception_handling.py` & `web3-6.8.0/web3/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/utils/caching.py` & `web3-6.8.0/web3/utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3/utils/exception_handling.py` & `web3-6.8.0/web3/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3.egg-info/PKG-INFO` & `web3-6.8.0/web3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.7.0
+Version: 6.8.0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.7.0/web3.egg-info/SOURCES.txt` & `web3-6.8.0/web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `web3-6.7.0/web3.egg-info/requires.txt` & `web3-6.8.0/web3.egg-info/requires.txt`

 * *Files identical despite different names*

