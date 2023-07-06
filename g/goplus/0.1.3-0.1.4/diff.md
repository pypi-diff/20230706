# Comparing `tmp/goplus-0.1.3.tar.gz` & `tmp/goplus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goplus-0.1.3.tar", last modified: Thu Jul  6 10:38:55 2023, max compression
+gzip compressed data, was "goplus-0.1.4.tar", last modified: Thu Jul  6 10:46:47 2023, max compression
```

## Comparing `goplus-0.1.3.tar` & `goplus-0.1.4.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.592493 goplus-0.1.3/
--rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.3/LICENSE
--rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:38:55.592368 goplus-0.1.3/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.1.3/README.md
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.577748 goplus-0.1.3/goplus/
--rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)      654 2023-07-06 10:35:50.000000 goplus-0.1.3/goplus/__version__.py
--rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/address.py
--rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/approve.py
--rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/auth.py
--rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/base.py
--rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/chain.py
--rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/dapp.py
--rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/decode.py
--rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/errocode.py
--rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/nft.py
--rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/rug_pull.py
--rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.3/goplus/token.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.578245 goplus-0.1.3/goplus.egg-info/
--rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     4082 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/SOURCES.txt
--rw-r--r--   0 cong       (501) staff       (20)        1 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/dependency_links.txt
--rw-r--r--   0 cong       (501) staff       (20)       67 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/requires.txt
--rw-r--r--   0 cong       (501) staff       (20)       22 2023-07-06 10:38:55.000000 goplus-0.1.3/goplus.egg-info/top_level.txt
--rw-r--r--   0 cong       (501) staff       (20)       38 2023-07-06 10:38:55.592529 goplus-0.1.3/setup.cfg
--rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.3/setup.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.580291 goplus-0.1.3/swagger_client/
--rw-r--r--   0 cong       (501) staff       (20)     6306 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/__init__.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.582719 goplus-0.1.3/swagger_client/api/
--rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.3/swagger_client/api/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)    10919 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/approve_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)    15210 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/approve_controller_v_2_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4981 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/contract_abi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4471 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/dapp_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5548 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/api/defi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5833 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/nft_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/token_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    10150 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/token_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4726 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api/website_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/api_client.py
--rw-r--r--   0 cong       (501) staff       (20)     8010 2023-05-30 08:59:54.000000 goplus-0.1.3/swagger_client/configuration.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:38:55.592091 goplus-0.1.3/swagger_client/models/
--rw-r--r--   0 cong       (501) staff       (20)     5480 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/abi_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/abi_param_info.py
--rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_erc1155_result.py
--rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_result.py
--rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/approve_token_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/audit_info.py
--rw-r--r--   0 cong       (501) staff       (20)    15392 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/contracts.py
--rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/contracts_security.py
--rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.1.3/swagger_client/models/get_access_token_request.py
--rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4619 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/get_defi_info_response.py
--rw-r--r--   0 cong       (501) staff       (20)    12280 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/get_defi_info_response_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/get_defi_info_response_result_owner.py
--rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/parse_abi_data_request.py
--rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_address_contract.py
--rw-r--r--   0 cong       (501) staff       (20)    23058 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_address_contract_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5012 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4898 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4733 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info.py
--rw-r--r--   0 cong       (501) staff       (20)    42552 2023-06-02 06:08:47.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     4767 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5132 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5056 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5151 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4960 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list.py
--rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_list_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     4838 2023-06-21 02:21:31.000000 goplus-0.1.3/swagger_client/models/response_wrapper_map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     4860 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4771 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4899 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security.py
--rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security_dex.py
--rw-r--r--   0 cong       (501) staff       (20)    10301 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)    70422 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapper_token_security_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4670 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/response_wrapperobject.py
--rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/models/ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.3/swagger_client/rest.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.936354 goplus-0.1.4/
+-rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.4/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:46:47.936240 goplus-0.1.4/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.1.4/README.md
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.925484 goplus-0.1.4/goplus/
+-rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)      654 2023-07-06 10:45:38.000000 goplus-0.1.4/goplus/__version__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/address.py
+-rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/approve.py
+-rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/auth.py
+-rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/base.py
+-rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/chain.py
+-rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/dapp.py
+-rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/decode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/errocode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/nft.py
+-rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/rug_pull.py
+-rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/token.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.925948 goplus-0.1.4/goplus.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     4153 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)       67 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       22 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/top_level.txt
+-rw-r--r--   0 cong       (501) staff       (20)       38 2023-07-06 10:46:47.936387 goplus-0.1.4/setup.cfg
+-rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.4/setup.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.926786 goplus-0.1.4/swagger_client/
+-rw-r--r--   0 cong       (501) staff       (20)     6427 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/__init__.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.928649 goplus-0.1.4/swagger_client/api/
+-rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.4/swagger_client/api/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)    10919 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/approve_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    15210 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/approve_controller_v_2_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4981 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/contract_abi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4471 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/dapp_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5548 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/api/defi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5833 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/nft_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/token_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    10150 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/token_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4726 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/website_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api_client.py
+-rw-r--r--   0 cong       (501) staff       (20)     8010 2023-05-30 08:59:54.000000 goplus-0.1.4/swagger_client/configuration.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.936076 goplus-0.1.4/swagger_client/models/
+-rw-r--r--   0 cong       (501) staff       (20)     5601 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/models/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/abi_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/abi_param_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_erc1155_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_token_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/audit_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    15392 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/contracts.py
+-rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/contracts_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.1.4/swagger_client/models/get_access_token_request.py
+-rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4619 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/get_defi_info_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    12280 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/get_defi_info_response_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/get_defi_info_response_result_owner.py
+-rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/parse_abi_data_request.py
+-rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_address_contract.py
+-rw-r--r--   0 cong       (501) staff       (20)    23058 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_address_contract_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5012 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4898 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4733 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    42552 2023-06-02 06:08:47.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
+-rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     4767 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     5132 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5056 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5151 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4960 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list.py
+-rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     4838 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/response_wrapper_map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     4860 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4771 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4899 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_dex.py
+-rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_locked_detail.py
+-rw-r--r--   0 cong       (501) staff       (20)    10070 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_lp_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)    70422 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4670 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapperobject.py
+-rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/rest.py
```

### Comparing `goplus-0.1.3/LICENSE` & `goplus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/PKG-INFO` & `goplus-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.3
+Version: 0.1.4
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.1.3/goplus/__init__.py` & `goplus-0.1.4/goplus/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/__version__.py` & `goplus-0.1.4/goplus/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (0, 1, 3)
+VERSION = (0, 1, 4)
 
 __version__ = ".".join(map(str, VERSION))
```

### Comparing `goplus-0.1.3/goplus/address.py` & `goplus-0.1.4/goplus/address.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/approve.py` & `goplus-0.1.4/goplus/approve.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/auth.py` & `goplus-0.1.4/goplus/auth.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/base.py` & `goplus-0.1.4/goplus/base.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/chain.py` & `goplus-0.1.4/goplus/chain.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/dapp.py` & `goplus-0.1.4/goplus/dapp.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/decode.py` & `goplus-0.1.4/goplus/decode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/errocode.py` & `goplus-0.1.4/goplus/errocode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/nft.py` & `goplus-0.1.4/goplus/nft.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/phishing_site.py` & `goplus-0.1.4/goplus/phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/rug_pull.py` & `goplus-0.1.4/goplus/rug_pull.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus/token.py` & `goplus-0.1.4/goplus/token.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/goplus.egg-info/PKG-INFO` & `goplus-0.1.4/goplus.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.3
+Version: 0.1.4
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.1.3/goplus.egg-info/SOURCES.txt` & `goplus-0.1.4/goplus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,11 +80,12 @@
 swagger_client/models/response_wrapper_map_string_string.py
 swagger_client/models/response_wrapper_parse_abi_data_response.py
 swagger_client/models/response_wrapper_phishing_site.py
 swagger_client/models/response_wrapper_phishing_site_result.py
 swagger_client/models/response_wrapper_ta_token_security_response.py
 swagger_client/models/response_wrapper_token_security.py
 swagger_client/models/response_wrapper_token_security_dex.py
+swagger_client/models/response_wrapper_token_security_locked_detail.py
 swagger_client/models/response_wrapper_token_security_lp_holders.py
 swagger_client/models/response_wrapper_token_security_result.py
 swagger_client/models/response_wrapperobject.py
 swagger_client/models/ta_token_security_response.py
```

### Comparing `goplus-0.1.3/setup.py` & `goplus-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/__init__.py` & `goplus-0.1.4/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,11 +73,12 @@
 from swagger_client.models.response_wrapper_map_string_string import ResponseWrapperMapStringString
 from swagger_client.models.response_wrapper_parse_abi_data_response import ResponseWrapperParseAbiDataResponse
 from swagger_client.models.response_wrapper_phishing_site import ResponseWrapperPhishingSite
 from swagger_client.models.response_wrapper_phishing_site_result import ResponseWrapperPhishingSiteResult
 from swagger_client.models.response_wrapper_ta_token_security_response import ResponseWrapperTaTokenSecurityResponse
 from swagger_client.models.response_wrapper_token_security import ResponseWrapperTokenSecurity
 from swagger_client.models.response_wrapper_token_security_dex import ResponseWrapperTokenSecurityDex
+from swagger_client.models.response_wrapper_token_security_locked_detail import ResponseWrapperTokenSecurityLockedDetail
 from swagger_client.models.response_wrapper_token_security_lp_holders import ResponseWrapperTokenSecurityLpHolders
 from swagger_client.models.response_wrapper_token_security_result import ResponseWrapperTokenSecurityResult
 from swagger_client.models.response_wrapperobject import ResponseWrapperobject
 from swagger_client.models.ta_token_security_response import TaTokenSecurityResponse
```

### Comparing `goplus-0.1.3/swagger_client/api/__init__.py` & `goplus-0.1.4/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/approve_controller_v_1_api.py` & `goplus-0.1.4/swagger_client/api/approve_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/approve_controller_v_2_api.py` & `goplus-0.1.4/swagger_client/api/approve_controller_v_2_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/contract_abi_controller_api.py` & `goplus-0.1.4/swagger_client/api/contract_abi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/dapp_controller_api.py` & `goplus-0.1.4/swagger_client/api/dapp_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/defi_controller_api.py` & `goplus-0.1.4/swagger_client/api/defi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/nft_controller_api.py` & `goplus-0.1.4/swagger_client/api/nft_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/token_controller_api.py` & `goplus-0.1.4/swagger_client/api/token_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/token_controller_v_1_api.py` & `goplus-0.1.4/swagger_client/api/token_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api/website_controller_api.py` & `goplus-0.1.4/swagger_client/api/website_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/api_client.py` & `goplus-0.1.4/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/configuration.py` & `goplus-0.1.4/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/__init__.py` & `goplus-0.1.4/swagger_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,11 +59,12 @@
 from swagger_client.models.response_wrapper_map_string_string import ResponseWrapperMapStringString
 from swagger_client.models.response_wrapper_parse_abi_data_response import ResponseWrapperParseAbiDataResponse
 from swagger_client.models.response_wrapper_phishing_site import ResponseWrapperPhishingSite
 from swagger_client.models.response_wrapper_phishing_site_result import ResponseWrapperPhishingSiteResult
 from swagger_client.models.response_wrapper_ta_token_security_response import ResponseWrapperTaTokenSecurityResponse
 from swagger_client.models.response_wrapper_token_security import ResponseWrapperTokenSecurity
 from swagger_client.models.response_wrapper_token_security_dex import ResponseWrapperTokenSecurityDex
+from swagger_client.models.response_wrapper_token_security_locked_detail import ResponseWrapperTokenSecurityLockedDetail
 from swagger_client.models.response_wrapper_token_security_lp_holders import ResponseWrapperTokenSecurityLpHolders
 from swagger_client.models.response_wrapper_token_security_result import ResponseWrapperTokenSecurityResult
 from swagger_client.models.response_wrapperobject import ResponseWrapperobject
 from swagger_client.models.ta_token_security_response import TaTokenSecurityResponse
```

### Comparing `goplus-0.1.3/swagger_client/models/abi_address_info.py` & `goplus-0.1.4/swagger_client/models/abi_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/abi_param_info.py` & `goplus-0.1.4/swagger_client/models/abi_param_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_address_info.py` & `goplus-0.1.4/swagger_client/models/approve_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_erc1155_result.py` & `goplus-0.1.4/swagger_client/models/approve_erc1155_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_nft1155_list_response.py` & `goplus-0.1.4/swagger_client/models/approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_nft_list_response.py` & `goplus-0.1.4/swagger_client/models/approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_result.py` & `goplus-0.1.4/swagger_client/models/approve_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_token_out_list_response.py` & `goplus-0.1.4/swagger_client/models/approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/approve_token_result.py` & `goplus-0.1.4/swagger_client/models/approve_token_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/audit_info.py` & `goplus-0.1.4/swagger_client/models/audit_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/contract_approve_response.py` & `goplus-0.1.4/swagger_client/models/contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/contracts.py` & `goplus-0.1.4/swagger_client/models/contracts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/contracts_security.py` & `goplus-0.1.4/swagger_client/models/contracts_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/dapp_contract_security_response.py` & `goplus-0.1.4/swagger_client/models/dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/get_access_token_request.py` & `goplus-0.1.4/swagger_client/models/get_access_token_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/get_access_token_response.py` & `goplus-0.1.4/swagger_client/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/get_defi_info_response.py` & `goplus-0.1.4/swagger_client/models/get_defi_info_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/get_defi_info_response_result.py` & `goplus-0.1.4/swagger_client/models/get_defi_info_response_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/get_defi_info_response_result_owner.py` & `goplus-0.1.4/swagger_client/models/get_defi_info_response_result_owner.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/json_object.py` & `goplus-0.1.4/swagger_client/models/json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/map_string_string.py` & `goplus-0.1.4/swagger_client/models/map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/parse_abi_data_request.py` & `goplus-0.1.4/swagger_client/models/parse_abi_data_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/parse_abi_data_response.py` & `goplus-0.1.4/swagger_client/models/parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_address_contract.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_address_contract.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_address_contract_result.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_address_contract_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_contract_approve_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_dapp_contract_security_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_access_token_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_json_object.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_nft_list_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_list_get_chains_list_result.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_list_json_object.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_list_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_map_string_string.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_parse_abi_data_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_phishing_site_result.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_ta_token_security_response.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_token_security.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_token_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_token_security_dex.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_dex.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_token_security_lp_holders.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_lp_holders.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'is_locked': 'int',
         'is_contract': 'int',
         'address': 'str',
         'balance': 'str',
-        'locked_detail': 'list[str]',
+        'locked_detail': 'list[ResponseWrapperTokenSecurityLockedDetail]',
         'tag': 'str',
         'percent': 'str'
     }
 
     attribute_map = {
         'is_locked': 'is_locked',
         'is_contract': 'is_contract',
@@ -164,29 +164,29 @@
 
         self._balance = balance
 
     @property
     def locked_detail(self):
         """Gets the locked_detail of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
-        It is an array, decribes lock position info of this holder, only shows when \"locked\": 1. This Array may contain multiple objects for multiple locking info. In every objetc, \"amount\" describes the number of token locked, \"end_time\" describes when the token will be unlocked, \"opt_time\" describes when the token was locked.(Notice:When \"locked\":0, or lock address is a black hole address,  \"locked_detail\" will be no return.)  # noqa: E501
+        It is an array, decribes lock position info of this holder, only shows when \"locked\": 1. This Array may contain multiple objects for multiple locking info. (Notice:When \"locked\":0, or lock address is a black hole address,  \"locked_detail\" will be no return.)  # noqa: E501
 
         :return: The locked_detail of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
-        :rtype: list[str]
+        :rtype: list[ResponseWrapperTokenSecurityLockedDetail]
         """
         return self._locked_detail
 
     @locked_detail.setter
     def locked_detail(self, locked_detail):
         """Sets the locked_detail of this ResponseWrapperTokenSecurityLpHolders.
 
-        It is an array, decribes lock position info of this holder, only shows when \"locked\": 1. This Array may contain multiple objects for multiple locking info. In every objetc, \"amount\" describes the number of token locked, \"end_time\" describes when the token will be unlocked, \"opt_time\" describes when the token was locked.(Notice:When \"locked\":0, or lock address is a black hole address,  \"locked_detail\" will be no return.)  # noqa: E501
+        It is an array, decribes lock position info of this holder, only shows when \"locked\": 1. This Array may contain multiple objects for multiple locking info. (Notice:When \"locked\":0, or lock address is a black hole address,  \"locked_detail\" will be no return.)  # noqa: E501
 
         :param locked_detail: The locked_detail of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
-        :type: list[str]
+        :type: list[ResponseWrapperTokenSecurityLockedDetail]
         """
 
         self._locked_detail = locked_detail
 
     @property
     def tag(self):
         """Gets the tag of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
```

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapper_token_security_result.py` & `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/response_wrapperobject.py` & `goplus-0.1.4/swagger_client/models/response_wrapperobject.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/models/ta_token_security_response.py` & `goplus-0.1.4/swagger_client/models/ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.3/swagger_client/rest.py` & `goplus-0.1.4/swagger_client/rest.py`

 * *Files identical despite different names*

