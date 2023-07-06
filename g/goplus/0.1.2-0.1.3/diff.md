# Comparing `tmp/goplus-0.1.2.tar.gz` & `tmp/goplus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goplus-0.1.2.tar", last modified: Wed Jun 21 03:31:18 2023, max compression
+gzip compressed data, was "goplus-0.1.3.tar", last modified: Thu Jul  6 10:38:55 2023, max compression
```

## Comparing `goplus-0.1.2.tar` & `goplus-0.1.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 03:31:18.884714 goplus-0.1.2/
--rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.2/LICENSE
--rw-r--r--   0 cong       (501) staff       (20)     3211 2023-06-21 03:31:18.884587 goplus-0.1.2/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     2733 2023-06-02 06:08:47.000000 goplus-0.1.2/README.md
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 03:31:18.877059 goplus-0.1.2/goplus/
--rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)      654 2023-06-21 03:21:19.000000 goplus-0.1.2/goplus/__version__.py
--rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/address.py
--rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/approve.py
--rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/auth.py
--rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/base.py
--rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/chain.py
--rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/dapp.py
--rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/decode.py
--rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/errocode.py
--rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/nft.py
--rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/rug_pull.py
--rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.2/goplus/token.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 03:31:18.877563 goplus-0.1.2/goplus.egg-info/
--rw-r--r--   0 cong       (501) staff       (20)     3211 2023-06-21 03:31:18.000000 goplus-0.1.2/goplus.egg-info/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     4082 2023-06-21 03:31:18.000000 goplus-0.1.2/goplus.egg-info/SOURCES.txt
--rw-r--r--   0 cong       (501) staff       (20)        1 2023-06-21 03:31:18.000000 goplus-0.1.2/goplus.egg-info/dependency_links.txt
--rw-r--r--   0 cong       (501) staff       (20)       67 2023-06-21 03:31:18.000000 goplus-0.1.2/goplus.egg-info/requires.txt
--rw-r--r--   0 cong       (501) staff       (20)       22 2023-06-21 03:31:18.000000 goplus-0.1.2/goplus.egg-info/top_level.txt
--rw-r--r--   0 cong       (501) staff       (20)       38 2023-06-21 03:31:18.884750 goplus-0.1.2/setup.cfg
--rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.2/setup.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 03:31:18.878086 goplus-0.1.2/swagger_client/
--rw-r--r--   0 cong       (501) staff       (20)     6306 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/__init__.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 03:31:18.879296 goplus-0.1.2/swagger_client/api/
--rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.2/swagger_client/api/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)    10919 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/approve_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)    15210 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/approve_controller_v_2_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4981 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/contract_abi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4471 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/dapp_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5548 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/api/defi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5833 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/nft_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/token_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    10150 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/token_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4726 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api/website_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/api_client.py
--rw-r--r--   0 cong       (501) staff       (20)     8010 2023-05-30 08:59:54.000000 goplus-0.1.2/swagger_client/configuration.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 03:31:18.884415 goplus-0.1.2/swagger_client/models/
--rw-r--r--   0 cong       (501) staff       (20)     5480 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/models/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/abi_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/abi_param_info.py
--rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_erc1155_result.py
--rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_result.py
--rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/approve_token_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/audit_info.py
--rw-r--r--   0 cong       (501) staff       (20)    15392 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/contracts.py
--rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/contracts_security.py
--rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5579 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/get_access_token_request.py
--rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4619 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/models/get_defi_info_response.py
--rw-r--r--   0 cong       (501) staff       (20)    12280 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/models/get_defi_info_response_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/models/get_defi_info_response_result_owner.py
--rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/models/map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/parse_abi_data_request.py
--rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_address_contract.py
--rw-r--r--   0 cong       (501) staff       (20)    23058 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_address_contract_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5012 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4898 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4733 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info.py
--rw-r--r--   0 cong       (501) staff       (20)    42552 2023-06-02 06:08:47.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     4767 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5132 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5056 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5151 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4960 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_list_get_chains_list.py
--rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_list_get_chains_list_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_list_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     4838 2023-06-21 02:21:31.000000 goplus-0.1.2/swagger_client/models/response_wrapper_map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     4860 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4771 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_phishing_site_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4899 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_token_security.py
--rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_token_security_dex.py
--rw-r--r--   0 cong       (501) staff       (20)    10301 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_token_security_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)    70422 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapper_token_security_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4670 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/response_wrapperobject.py
--rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/models/ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.2/swagger_client/rest.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.592493 goplus-0.1.3/
+-rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.3/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:38:55.592368 goplus-0.1.3/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.1.3/README.md
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.577748 goplus-0.1.3/goplus/
+-rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)      654 2023-07-06 10:35:50.000000 goplus-0.1.3/goplus/__version__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/address.py
+-rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/approve.py
+-rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/auth.py
+-rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/base.py
+-rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/chain.py
+-rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/dapp.py
+-rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/decode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/errocode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/nft.py
+-rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/rug_pull.py
+-rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/token.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.578245 goplus-0.1.3/goplus.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     4082 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)       67 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       22 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/top_level.txt
+-rw-r--r--   0 cong       (501) staff       (20)       38 2023-07-06 10:38:55.592529 goplus-0.1.3/setup.cfg
+-rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.3/setup.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.580291 goplus-0.1.3/swagger_client/
+-rw-r--r--   0 cong       (501) staff       (20)     6306 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/__init__.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.582719 goplus-0.1.3/swagger_client/api/
+-rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.3/swagger_client/api/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)    10919 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/approve_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    15210 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/approve_controller_v_2_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4981 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/contract_abi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4471 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/dapp_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5548 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/api/defi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5833 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/nft_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/token_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    10150 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/token_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4726 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/website_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api_client.py
+-rw-r--r--   0 cong       (501) staff       (20)     8010 2023-05-30 08:59:54.000000 goplus-0.1.3/swagger_client/configuration.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.592091 goplus-0.1.3/swagger_client/models/
+-rw-r--r--   0 cong       (501) staff       (20)     5480 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/abi_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/abi_param_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_erc1155_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_token_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/audit_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    15392 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/contracts.py
+-rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/contracts_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.1.3/swagger_client/models/get_access_token_request.py
+-rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4619 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/get_defi_info_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    12280 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/get_defi_info_response_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/get_defi_info_response_result_owner.py
+-rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/parse_abi_data_request.py
+-rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_address_contract.py
+-rw-r--r--   0 cong       (501) staff       (20)    23058 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_address_contract_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5012 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4898 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4733 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    42552 2023-06-02 06:08:47.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
+-rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     4767 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     5132 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5056 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5151 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4960 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list.py
+-rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     4838 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/response_wrapper_map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     4860 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4771 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4899 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security_dex.py
+-rw-r--r--   0 cong       (501) staff       (20)    10301 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security_lp_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)    70422 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4670 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapperobject.py
+-rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/rest.py
```

### Comparing `goplus-0.1.2/LICENSE` & `goplus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/__init__.py` & `goplus-0.1.3/goplus/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/__version__.py` & `goplus-0.1.3/goplus/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (0, 1, 2)
+VERSION = (0, 1, 3)
 
 __version__ = ".".join(map(str, VERSION))
```

### Comparing `goplus-0.1.2/goplus/address.py` & `goplus-0.1.3/goplus/address.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/approve.py` & `goplus-0.1.3/goplus/approve.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/auth.py` & `goplus-0.1.3/goplus/auth.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/base.py` & `goplus-0.1.3/goplus/base.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/chain.py` & `goplus-0.1.3/goplus/chain.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/dapp.py` & `goplus-0.1.3/goplus/dapp.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/decode.py` & `goplus-0.1.3/goplus/decode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/errocode.py` & `goplus-0.1.3/goplus/errocode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/nft.py` & `goplus-0.1.3/goplus/nft.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/phishing_site.py` & `goplus-0.1.3/goplus/phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/rug_pull.py` & `goplus-0.1.3/goplus/rug_pull.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus/token.py` & `goplus-0.1.3/goplus/token.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/goplus.egg-info/SOURCES.txt` & `goplus-0.1.3/goplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/setup.py` & `goplus-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/__init__.py` & `goplus-0.1.3/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/__init__.py` & `goplus-0.1.3/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/approve_controller_v_1_api.py` & `goplus-0.1.3/swagger_client/api/approve_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/approve_controller_v_2_api.py` & `goplus-0.1.3/swagger_client/api/approve_controller_v_2_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/contract_abi_controller_api.py` & `goplus-0.1.3/swagger_client/api/contract_abi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/dapp_controller_api.py` & `goplus-0.1.3/swagger_client/api/dapp_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/defi_controller_api.py` & `goplus-0.1.3/swagger_client/api/defi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/nft_controller_api.py` & `goplus-0.1.3/swagger_client/api/nft_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/token_controller_api.py` & `goplus-0.1.3/swagger_client/api/token_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/token_controller_v_1_api.py` & `goplus-0.1.3/swagger_client/api/token_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api/website_controller_api.py` & `goplus-0.1.3/swagger_client/api/website_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/api_client.py` & `goplus-0.1.3/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/configuration.py` & `goplus-0.1.3/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/__init__.py` & `goplus-0.1.3/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/abi_address_info.py` & `goplus-0.1.3/swagger_client/models/abi_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/abi_param_info.py` & `goplus-0.1.3/swagger_client/models/abi_param_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_address_info.py` & `goplus-0.1.3/swagger_client/models/approve_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_erc1155_result.py` & `goplus-0.1.3/swagger_client/models/approve_erc1155_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_nft1155_list_response.py` & `goplus-0.1.3/swagger_client/models/approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_nft_list_response.py` & `goplus-0.1.3/swagger_client/models/approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_result.py` & `goplus-0.1.3/swagger_client/models/approve_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_token_out_list_response.py` & `goplus-0.1.3/swagger_client/models/approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/approve_token_result.py` & `goplus-0.1.3/swagger_client/models/approve_token_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/audit_info.py` & `goplus-0.1.3/swagger_client/models/audit_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/contract_approve_response.py` & `goplus-0.1.3/swagger_client/models/contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/contracts.py` & `goplus-0.1.3/swagger_client/models/contracts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/contracts_security.py` & `goplus-0.1.3/swagger_client/models/contracts_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/dapp_contract_security_response.py` & `goplus-0.1.3/swagger_client/models/dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/get_access_token_request.py` & `goplus-0.1.3/swagger_client/models/get_access_token_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,26 +74,26 @@
 
         self._app_key = app_key
 
     @property
     def sign(self):
         """Gets the sign of this GetAccessTokenRequest.  # noqa: E501
 
-        Concatenate app_key, time, app_secret in turn, and do sha1().app_key = mBOMg20QW11BbtyH4Zh0 \\n\" +             \"time = 1647847498 \\n\" +             \"app_secret = V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh \\n\" +             \"sign = sha1(mBOMg20QW11BbtyH4Zh01647847498V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh)\\n\" +             \"        = 7293d385b9225b3c3f232b76ba97255d0e21063e  # noqa: E501
+        Sign Method Concatenate app_key, time, app_secret in turn, and do sha1() . Example app_key = mBOMg20QW11BbtyH4Zh0 time = 1647847498 app_secret = V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh sign = sha1(mBOMg20QW11BbtyH4Zh01647847498V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh)        = 7293d385b9225b3c3f232b76ba97255d0e21063e  # noqa: E501
 
         :return: The sign of this GetAccessTokenRequest.  # noqa: E501
         :rtype: str
         """
         return self._sign
 
     @sign.setter
     def sign(self, sign):
         """Sets the sign of this GetAccessTokenRequest.
 
-        Concatenate app_key, time, app_secret in turn, and do sha1().app_key = mBOMg20QW11BbtyH4Zh0 \\n\" +             \"time = 1647847498 \\n\" +             \"app_secret = V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh \\n\" +             \"sign = sha1(mBOMg20QW11BbtyH4Zh01647847498V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh)\\n\" +             \"        = 7293d385b9225b3c3f232b76ba97255d0e21063e  # noqa: E501
+        Sign Method Concatenate app_key, time, app_secret in turn, and do sha1() . Example app_key = mBOMg20QW11BbtyH4Zh0 time = 1647847498 app_secret = V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh sign = sha1(mBOMg20QW11BbtyH4Zh01647847498V6aRfxlPJwN3ViJSIFSCdxPvneajuJsh)        = 7293d385b9225b3c3f232b76ba97255d0e21063e  # noqa: E501
 
         :param sign: The sign of this GetAccessTokenRequest.  # noqa: E501
         :type: str
         """
         if sign is None:
             raise ValueError("Invalid value for `sign`, must not be `None`")  # noqa: E501
```

### Comparing `goplus-0.1.2/swagger_client/models/get_access_token_response.py` & `goplus-0.1.3/swagger_client/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/get_defi_info_response.py` & `goplus-0.1.3/swagger_client/models/get_defi_info_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/get_defi_info_response_result.py` & `goplus-0.1.3/swagger_client/models/get_defi_info_response_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/get_defi_info_response_result_owner.py` & `goplus-0.1.3/swagger_client/models/get_defi_info_response_result_owner.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/json_object.py` & `goplus-0.1.3/swagger_client/models/json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/map_string_string.py` & `goplus-0.1.3/swagger_client/models/map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/parse_abi_data_request.py` & `goplus-0.1.3/swagger_client/models/parse_abi_data_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/parse_abi_data_response.py` & `goplus-0.1.3/swagger_client/models/parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_address_contract.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_address_contract.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_address_contract_result.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_address_contract_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_contract_approve_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_dapp_contract_security_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_access_token_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_json_object.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_list_approve_nft_list_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_list_get_chains_list.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_list_get_chains_list_result.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_list_json_object.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_list_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_map_string_string.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_parse_abi_data_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_phishing_site.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_phishing_site_result.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_ta_token_security_response.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_token_security.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_token_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_token_security_dex.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_token_security_dex.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_token_security_lp_holders.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_token_security_lp_holders.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapper_token_security_result.py` & `goplus-0.1.3/swagger_client/models/response_wrapper_token_security_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/response_wrapperobject.py` & `goplus-0.1.3/swagger_client/models/response_wrapperobject.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/models/ta_token_security_response.py` & `goplus-0.1.3/swagger_client/models/ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.2/swagger_client/rest.py` & `goplus-0.1.3/swagger_client/rest.py`

 * *Files identical despite different names*

