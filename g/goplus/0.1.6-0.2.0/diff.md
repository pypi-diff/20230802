# Comparing `tmp/goplus-0.1.6.tar.gz` & `tmp/goplus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goplus-0.1.6.tar", last modified: Wed Aug  2 02:28:21 2023, max compression
+gzip compressed data, was "goplus-0.2.0.tar", last modified: Wed Aug  2 03:43:48 2023, max compression
```

## Comparing `goplus-0.1.6.tar` & `goplus-0.2.0.tar`

### file list

```diff
@@ -1,100 +1,99 @@
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 02:28:21.654117 goplus-0.1.6/
--rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.6/LICENSE
--rw-r--r--   0 cong       (501) staff       (20)      837 2023-08-02 02:28:21.653994 goplus-0.1.6/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.1.6/README.md
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 02:28:21.638535 goplus-0.1.6/goplus/
--rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)      654 2023-08-02 02:20:18.000000 goplus-0.1.6/goplus/__version__.py
--rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/address.py
--rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/approve.py
--rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/auth.py
--rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/base.py
--rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/chain.py
--rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/dapp.py
--rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/decode.py
--rw-r--r--   0 cong       (501) staff       (20)      708 2023-08-02 02:23:35.000000 goplus-0.1.6/goplus/errocode.py
--rw-r--r--   0 cong       (501) staff       (20)     1096 2023-08-02 02:25:02.000000 goplus-0.1.6/goplus/errorcode.py
--rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/nft.py
--rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/rug_pull.py
--rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.6/goplus/token.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 02:28:21.639020 goplus-0.1.6/goplus.egg-info/
--rw-r--r--   0 cong       (501) staff       (20)      837 2023-08-02 02:28:21.000000 goplus-0.1.6/goplus.egg-info/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     4173 2023-08-02 02:28:21.000000 goplus-0.1.6/goplus.egg-info/SOURCES.txt
--rw-r--r--   0 cong       (501) staff       (20)        1 2023-08-02 02:28:21.000000 goplus-0.1.6/goplus.egg-info/dependency_links.txt
--rw-r--r--   0 cong       (501) staff       (20)       67 2023-08-02 02:28:21.000000 goplus-0.1.6/goplus.egg-info/requires.txt
--rw-r--r--   0 cong       (501) staff       (20)       22 2023-08-02 02:28:21.000000 goplus-0.1.6/goplus.egg-info/top_level.txt
--rw-r--r--   0 cong       (501) staff       (20)       38 2023-08-02 02:28:21.654157 goplus-0.1.6/setup.cfg
--rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.6/setup.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 02:28:21.640099 goplus-0.1.6/swagger_client/
--rw-r--r--   0 cong       (501) staff       (20)     6427 2023-07-06 10:45:21.000000 goplus-0.1.6/swagger_client/__init__.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 02:28:21.642540 goplus-0.1.6/swagger_client/api/
--rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.6/swagger_client/api/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)    10907 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/api/approve_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)    16962 2023-08-02 02:06:01.000000 goplus-0.1.6/swagger_client/api/approve_controller_v_2_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4979 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/api/contract_abi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4469 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/api/dapp_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5546 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/api/defi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5831 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/api/nft_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/api/token_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    10214 2023-08-02 02:06:01.000000 goplus-0.1.6/swagger_client/api/token_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4724 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/api/website_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    25084 2023-07-26 13:12:08.000000 goplus-0.1.6/swagger_client/api_client.py
--rw-r--r--   0 cong       (501) staff       (20)     8010 2023-07-26 13:15:21.000000 goplus-0.1.6/swagger_client/configuration.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 02:28:21.653231 goplus-0.1.6/swagger_client/models/
--rw-r--r--   0 cong       (501) staff       (20)     5601 2023-07-06 10:45:21.000000 goplus-0.1.6/swagger_client/models/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/abi_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/abi_param_info.py
--rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_erc1155_result.py
--rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_result.py
--rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/approve_token_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/audit_info.py
--rw-r--r--   0 cong       (501) staff       (20)    15388 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/contracts.py
--rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/contracts_security.py
--rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.1.6/swagger_client/models/get_access_token_request.py
--rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4617 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/get_defi_info_response.py
--rw-r--r--   0 cong       (501) staff       (20)    12268 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/get_defi_info_response_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.6/swagger_client/models/get_defi_info_response_result_owner.py
--rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.6/swagger_client/models/map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/parse_abi_data_request.py
--rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_address_contract.py
--rw-r--r--   0 cong       (501) staff       (20)    23056 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_address_contract_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5010 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4896 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4731 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info.py
--rw-r--r--   0 cong       (501) staff       (20)    42512 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     4765 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5130 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5054 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5149 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4958 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_list_get_chains_list.py
--rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_list_get_chains_list_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_list_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     4836 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     4858 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4769 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_phishing_site_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4897 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_token_security.py
--rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/response_wrapper_token_security_dex.py
--rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.1.6/swagger_client/models/response_wrapper_token_security_locked_detail.py
--rw-r--r--   0 cong       (501) staff       (20)    10066 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_token_security_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)    70400 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapper_token_security_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4668 2023-07-21 07:25:36.000000 goplus-0.1.6/swagger_client/models/response_wrapperobject.py
--rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/models/ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.6/swagger_client/rest.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 03:43:48.920325 goplus-0.2.0/
+-rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.2.0/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-08-02 03:43:48.920178 goplus-0.2.0/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.2.0/README.md
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 03:43:48.903320 goplus-0.2.0/goplus/
+-rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)      654 2023-08-02 03:40:27.000000 goplus-0.2.0/goplus/__version__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/address.py
+-rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/approve.py
+-rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/auth.py
+-rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/base.py
+-rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/chain.py
+-rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/dapp.py
+-rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/decode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1096 2023-08-02 02:25:02.000000 goplus-0.2.0/goplus/errorcode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/nft.py
+-rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/rug_pull.py
+-rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.2.0/goplus/token.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 03:43:48.903825 goplus-0.2.0/goplus.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-08-02 03:43:48.000000 goplus-0.2.0/goplus.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     4154 2023-08-02 03:43:48.000000 goplus-0.2.0/goplus.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2023-08-02 03:43:48.000000 goplus-0.2.0/goplus.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)       67 2023-08-02 03:43:48.000000 goplus-0.2.0/goplus.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       22 2023-08-02 03:43:48.000000 goplus-0.2.0/goplus.egg-info/top_level.txt
+-rw-r--r--   0 cong       (501) staff       (20)       38 2023-08-02 03:43:48.920365 goplus-0.2.0/setup.cfg
+-rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.2.0/setup.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 03:43:48.904943 goplus-0.2.0/swagger_client/
+-rw-r--r--   0 cong       (501) staff       (20)     6427 2023-07-06 10:45:21.000000 goplus-0.2.0/swagger_client/__init__.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 03:43:48.908037 goplus-0.2.0/swagger_client/api/
+-rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.2.0/swagger_client/api/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)    10907 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/api/approve_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    16962 2023-08-02 02:06:01.000000 goplus-0.2.0/swagger_client/api/approve_controller_v_2_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4979 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/api/contract_abi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4469 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/api/dapp_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5546 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/api/defi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5831 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/api/nft_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/api/token_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    10214 2023-08-02 02:06:01.000000 goplus-0.2.0/swagger_client/api/token_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4724 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/api/website_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    25084 2023-07-26 13:12:08.000000 goplus-0.2.0/swagger_client/api_client.py
+-rw-r--r--   0 cong       (501) staff       (20)     8010 2023-07-26 13:15:21.000000 goplus-0.2.0/swagger_client/configuration.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-02 03:43:48.919800 goplus-0.2.0/swagger_client/models/
+-rw-r--r--   0 cong       (501) staff       (20)     5601 2023-07-06 10:45:21.000000 goplus-0.2.0/swagger_client/models/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/abi_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/abi_param_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_erc1155_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/approve_token_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/audit_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    15388 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/contracts.py
+-rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/contracts_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.2.0/swagger_client/models/get_access_token_request.py
+-rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4617 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/get_defi_info_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    12268 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/get_defi_info_response_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.2.0/swagger_client/models/get_defi_info_response_result_owner.py
+-rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.2.0/swagger_client/models/map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/parse_abi_data_request.py
+-rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_address_contract.py
+-rw-r--r--   0 cong       (501) staff       (20)    23056 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_address_contract_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5010 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4896 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4731 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    42512 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
+-rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     4765 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     5130 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5054 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5149 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4958 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_list_get_chains_list.py
+-rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_list_get_chains_list_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_list_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     4836 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     4858 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4769 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_phishing_site_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4897 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_token_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/response_wrapper_token_security_dex.py
+-rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.2.0/swagger_client/models/response_wrapper_token_security_locked_detail.py
+-rw-r--r--   0 cong       (501) staff       (20)    10066 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_token_security_lp_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)    70400 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapper_token_security_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4668 2023-07-21 07:25:36.000000 goplus-0.2.0/swagger_client/models/response_wrapperobject.py
+-rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/models/ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.2.0/swagger_client/rest.py
```

### Comparing `goplus-0.1.6/LICENSE` & `goplus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/PKG-INFO` & `goplus-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.6
+Version: 0.2.0
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.1.6/goplus/__init__.py` & `goplus-0.2.0/goplus/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/__version__.py` & `goplus-0.2.0/goplus/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (0, 1, 6)
+VERSION = (0, 2, 0)
 
 __version__ = ".".join(map(str, VERSION))
```

### Comparing `goplus-0.1.6/goplus/address.py` & `goplus-0.2.0/goplus/address.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/approve.py` & `goplus-0.2.0/goplus/approve.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/auth.py` & `goplus-0.2.0/goplus/auth.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/base.py` & `goplus-0.2.0/goplus/base.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/chain.py` & `goplus-0.2.0/goplus/chain.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/dapp.py` & `goplus-0.2.0/goplus/dapp.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/decode.py` & `goplus-0.2.0/goplus/decode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/errorcode.py` & `goplus-0.2.0/goplus/errorcode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/nft.py` & `goplus-0.2.0/goplus/nft.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/phishing_site.py` & `goplus-0.2.0/goplus/phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/rug_pull.py` & `goplus-0.2.0/goplus/rug_pull.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus/token.py` & `goplus-0.2.0/goplus/token.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/goplus.egg-info/PKG-INFO` & `goplus-0.2.0/goplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.6
+Version: 0.2.0
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.1.6/goplus.egg-info/SOURCES.txt` & `goplus-0.2.0/goplus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 goplus/address.py
 goplus/approve.py
 goplus/auth.py
 goplus/base.py
 goplus/chain.py
 goplus/dapp.py
 goplus/decode.py
-goplus/errocode.py
 goplus/errorcode.py
 goplus/nft.py
 goplus/phishing_site.py
 goplus/rug_pull.py
 goplus/token.py
 goplus.egg-info/PKG-INFO
 goplus.egg-info/SOURCES.txt
```

### Comparing `goplus-0.1.6/setup.py` & `goplus-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/__init__.py` & `goplus-0.2.0/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/__init__.py` & `goplus-0.2.0/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/approve_controller_v_1_api.py` & `goplus-0.2.0/swagger_client/api/approve_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/approve_controller_v_2_api.py` & `goplus-0.2.0/swagger_client/api/approve_controller_v_2_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/contract_abi_controller_api.py` & `goplus-0.2.0/swagger_client/api/contract_abi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/dapp_controller_api.py` & `goplus-0.2.0/swagger_client/api/dapp_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/defi_controller_api.py` & `goplus-0.2.0/swagger_client/api/defi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/nft_controller_api.py` & `goplus-0.2.0/swagger_client/api/nft_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/token_controller_api.py` & `goplus-0.2.0/swagger_client/api/token_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/token_controller_v_1_api.py` & `goplus-0.2.0/swagger_client/api/token_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api/website_controller_api.py` & `goplus-0.2.0/swagger_client/api/website_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/api_client.py` & `goplus-0.2.0/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/configuration.py` & `goplus-0.2.0/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/__init__.py` & `goplus-0.2.0/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/abi_address_info.py` & `goplus-0.2.0/swagger_client/models/abi_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/abi_param_info.py` & `goplus-0.2.0/swagger_client/models/abi_param_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_address_info.py` & `goplus-0.2.0/swagger_client/models/approve_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_erc1155_result.py` & `goplus-0.2.0/swagger_client/models/approve_erc1155_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_nft1155_list_response.py` & `goplus-0.2.0/swagger_client/models/approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_nft_list_response.py` & `goplus-0.2.0/swagger_client/models/approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_result.py` & `goplus-0.2.0/swagger_client/models/approve_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_token_out_list_response.py` & `goplus-0.2.0/swagger_client/models/approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/approve_token_result.py` & `goplus-0.2.0/swagger_client/models/approve_token_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/audit_info.py` & `goplus-0.2.0/swagger_client/models/audit_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/contract_approve_response.py` & `goplus-0.2.0/swagger_client/models/contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/contracts.py` & `goplus-0.2.0/swagger_client/models/contracts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/contracts_security.py` & `goplus-0.2.0/swagger_client/models/contracts_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/dapp_contract_security_response.py` & `goplus-0.2.0/swagger_client/models/dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/get_access_token_request.py` & `goplus-0.2.0/swagger_client/models/get_access_token_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/get_access_token_response.py` & `goplus-0.2.0/swagger_client/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/get_defi_info_response.py` & `goplus-0.2.0/swagger_client/models/get_defi_info_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/get_defi_info_response_result.py` & `goplus-0.2.0/swagger_client/models/get_defi_info_response_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/get_defi_info_response_result_owner.py` & `goplus-0.2.0/swagger_client/models/get_defi_info_response_result_owner.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/json_object.py` & `goplus-0.2.0/swagger_client/models/json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/map_string_string.py` & `goplus-0.2.0/swagger_client/models/map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/parse_abi_data_request.py` & `goplus-0.2.0/swagger_client/models/parse_abi_data_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/parse_abi_data_response.py` & `goplus-0.2.0/swagger_client/models/parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_address_contract.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_address_contract.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_address_contract_result.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_address_contract_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_contract_approve_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_dapp_contract_security_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_access_token_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_json_object.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_list_approve_nft_list_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_list_approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_list_get_chains_list.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_list_get_chains_list.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_list_get_chains_list_result.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_list_get_chains_list_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_list_json_object.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_list_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_map_string_string.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_parse_abi_data_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_phishing_site.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_phishing_site_result.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_phishing_site_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_ta_token_security_response.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_token_security.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_token_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_token_security_dex.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_token_security_dex.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_token_security_locked_detail.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_token_security_locked_detail.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_token_security_lp_holders.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_token_security_lp_holders.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapper_token_security_result.py` & `goplus-0.2.0/swagger_client/models/response_wrapper_token_security_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/response_wrapperobject.py` & `goplus-0.2.0/swagger_client/models/response_wrapperobject.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/models/ta_token_security_response.py` & `goplus-0.2.0/swagger_client/models/ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.6/swagger_client/rest.py` & `goplus-0.2.0/swagger_client/rest.py`

 * *Files identical despite different names*

