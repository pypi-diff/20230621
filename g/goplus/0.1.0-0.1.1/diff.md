# Comparing `tmp/goplus-0.1.0.tar.gz` & `tmp/goplus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goplus-0.1.0.tar", last modified: Wed May 10 06:13:28 2023, max compression
+gzip compressed data, was "goplus-0.1.1.tar", last modified: Wed Jun 21 02:44:53 2023, max compression
```

## Comparing `goplus-0.1.0.tar` & `goplus-0.1.1.tar`

### file list

```diff
@@ -1,113 +1,98 @@
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-05-10 06:13:28.728854 goplus-0.1.0/
--rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.0/LICENSE
--rw-r--r--   0 cong       (501) staff       (20)     3020 2023-05-10 06:13:28.728721 goplus-0.1.0/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     2562 2023-05-10 02:53:37.000000 goplus-0.1.0/README.md
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-05-10 06:13:28.712037 goplus-0.1.0/goplus/
--rw-r--r--   0 cong       (501) staff       (20)        0 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)       63 2023-05-10 06:10:18.000000 goplus-0.1.0/goplus/__version__.py
--rw-r--r--   0 cong       (501) staff       (20)      544 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/address.py
--rw-r--r--   0 cong       (501) staff       (20)     1636 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/approve.py
--rw-r--r--   0 cong       (501) staff       (20)      890 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/auth.py
--rw-r--r--   0 cong       (501) staff       (20)      248 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/base.py
--rw-r--r--   0 cong       (501) staff       (20)      273 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/chain.py
--rw-r--r--   0 cong       (501) staff       (20)      391 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/dapp.py
--rw-r--r--   0 cong       (501) staff       (20)      711 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/decode.py
--rw-r--r--   0 cong       (501) staff       (20)      504 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/errocode.py
--rw-r--r--   0 cong       (501) staff       (20)      501 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/nft.py
--rw-r--r--   0 cong       (501) staff       (20)      411 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)      862 2023-05-10 02:53:37.000000 goplus-0.1.0/goplus/token.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-05-10 06:13:28.712629 goplus-0.1.0/goplus.egg-info/
--rw-r--r--   0 cong       (501) staff       (20)     3020 2023-05-10 06:13:28.000000 goplus-0.1.0/goplus.egg-info/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     6520 2023-05-10 06:13:28.000000 goplus-0.1.0/goplus.egg-info/SOURCES.txt
--rw-r--r--   0 cong       (501) staff       (20)        1 2023-05-10 06:13:28.000000 goplus-0.1.0/goplus.egg-info/dependency_links.txt
--rw-r--r--   0 cong       (501) staff       (20)       67 2023-05-10 06:13:28.000000 goplus-0.1.0/goplus.egg-info/requires.txt
--rw-r--r--   0 cong       (501) staff       (20)       22 2023-05-10 06:13:28.000000 goplus-0.1.0/goplus.egg-info/top_level.txt
--rw-r--r--   0 cong       (501) staff       (20)       38 2023-05-10 06:13:28.728888 goplus-0.1.0/setup.cfg
--rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.0/setup.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-05-10 06:13:28.713736 goplus-0.1.0/swagger_client/
--rw-r--r--   0 cong       (501) staff       (20)     7105 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/__init__.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-05-10 06:13:28.715458 goplus-0.1.0/swagger_client/api/
--rw-r--r--   0 cong       (501) staff       (20)      692 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)    10993 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/approve_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)    15215 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/approve_controller_v_2_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4986 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/contract_abi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4476 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/dapp_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5934 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/nft_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4287 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/token_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    10368 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/token_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4836 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api/website_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    25089 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/api_client.py
--rw-r--r--   0 cong       (501) staff       (20)     8015 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/configuration.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-05-10 06:13:28.728551 goplus-0.1.0/swagger_client/models/
--rw-r--r--   0 cong       (501) staff       (20)     6348 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)     7941 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/abi_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     5541 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/abi_param_info.py
--rw-r--r--   0 cong       (501) staff       (20)    10432 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     7894 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_erc1155_result.py
--rw-r--r--   0 cong       (501) staff       (20)    10647 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)    10466 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     9652 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_result.py
--rw-r--r--   0 cong       (501) staff       (20)    11420 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     8753 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/approve_token_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4938 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/audit_info.py
--rw-r--r--   0 cong       (501) staff       (20)    15397 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)    11569 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/contracts.py
--rw-r--r--   0 cong       (501) staff       (20)     4473 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/contracts_security.py
--rw-r--r--   0 cong       (501) staff       (20)     9043 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5584 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/get_access_token_request.py
--rw-r--r--   0 cong       (501) staff       (20)     4149 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     2689 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     2709 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/mapstringstring.py
--rw-r--r--   0 cong       (501) staff       (20)     7481 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/parse_abi_data_request.py
--rw-r--r--   0 cong       (501) staff       (20)    10376 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4922 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5017 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4903 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4772 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5346 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfe_b2f246e4936a6968cc97141b.py
--rw-r--r--   0 cong       (501) staff       (20)    46790 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7548 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7596 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     8378 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     7516 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7692 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     5346 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c.py
--rw-r--r--   0 cong       (501) staff       (20)    46784 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7548 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7596 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     8378 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     7516 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7692 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     5137 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5061 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5156 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4833 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5516 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object4e98b9e2_fbdb43329976_a30066e02b73.py
--rw-r--r--   0 cong       (501) staff       (20)     4361 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object4e98b9e2fbdb43329976a30066e02b73_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5516 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object9524a1c652c545bf_b6c6898bfc3e93f3.py
--rw-r--r--   0 cong       (501) staff       (20)     4361 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object9524a1c652c545bfb6c6898bfc3e93f3_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4843 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstring.py
--rw-r--r--   0 cong       (501) staff       (20)     5441 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstring2a740de0_be5a4eb3_b6e4_a2cf0a2d8bf8.py
--rw-r--r--   0 cong       (501) staff       (20)     5223 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5441 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstring_a9a4024a_e50a4a3a_a475_dba457d7c10e.py
--rw-r--r--   0 cong       (501) staff       (20)     5223 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstringa9a4024ae50a4a3aa475dba457d7c10e_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4865 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4922 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5702 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response205696bc_fb354bc5_ab26_ddc7cd495fe2.py
--rw-r--r--   0 cong       (501) staff       (20)     5582 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_dex.py
--rw-r--r--   0 cong       (501) staff       (20)    11650 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)    78029 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5702 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8b_bfd0494baf55b849.py
--rw-r--r--   0 cong       (501) staff       (20)     5582 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8bbfd0494baf55b849_dex.py
--rw-r--r--   0 cong       (501) staff       (20)    11650 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8bbfd0494baf55b849_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)    78029 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8bbfd0494baf55b849_result.py
--rw-r--r--   0 cong       (501) staff       (20)    80798 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8bbfd0494baf55b849_result_contract_address.py
--rw-r--r--   0 cong       (501) staff       (20)     5918 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8bbfd0494baf55b849_result_contract_address_dex.py
--rw-r--r--   0 cong       (501) staff       (20)    12322 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response730b76cb88874c8bbfd0494baf55b849_result_contract_address_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)     4675 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapperobject.py
--rw-r--r--   0 cong       (501) staff       (20)     5270 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapperobject545a2cea_b58741b4_aae7_f3d73df91255.py
--rw-r--r--   0 cong       (501) staff       (20)    24627 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapperobject545a2ceab58741b4aae7f3d73df91255_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5270 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapperobject_f7b82021_fc934bb69009542c33e30a39.py
--rw-r--r--   0 cong       (501) staff       (20)    24627 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/response_wrapperobjectf7b82021fc934bb69009542c33e30a39_result.py
--rw-r--r--   0 cong       (501) staff       (20)     3199 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/models/ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)    13041 2023-05-10 02:42:24.000000 goplus-0.1.0/swagger_client/rest.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 02:44:53.976613 goplus-0.1.1/
+-rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.1/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)     3211 2023-06-21 02:44:53.976478 goplus-0.1.1/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     2733 2023-06-02 06:08:47.000000 goplus-0.1.1/README.md
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 02:44:53.963394 goplus-0.1.1/goplus/
+-rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)      654 2023-05-30 08:17:00.000000 goplus-0.1.1/goplus/__version__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/address.py
+-rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/approve.py
+-rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/auth.py
+-rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/base.py
+-rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/chain.py
+-rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/dapp.py
+-rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/decode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/errocode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/nft.py
+-rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/rug_pull.py
+-rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.1/goplus/token.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 02:44:53.964131 goplus-0.1.1/goplus.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)     3211 2023-06-21 02:44:53.000000 goplus-0.1.1/goplus.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     4082 2023-06-21 02:44:53.000000 goplus-0.1.1/goplus.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2023-06-21 02:44:53.000000 goplus-0.1.1/goplus.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)       67 2023-06-21 02:44:53.000000 goplus-0.1.1/goplus.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       22 2023-06-21 02:44:53.000000 goplus-0.1.1/goplus.egg-info/top_level.txt
+-rw-r--r--   0 cong       (501) staff       (20)       38 2023-06-21 02:44:53.976649 goplus-0.1.1/setup.cfg
+-rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.1/setup.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 02:44:53.965388 goplus-0.1.1/swagger_client/
+-rw-r--r--   0 cong       (501) staff       (20)     6306 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/__init__.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 02:44:53.967635 goplus-0.1.1/swagger_client/api/
+-rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.1/swagger_client/api/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)    10919 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/approve_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    15210 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/approve_controller_v_2_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4981 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/contract_abi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4471 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/dapp_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5548 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/api/defi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5833 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/nft_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/token_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    10150 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/token_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4726 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api/website_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/api_client.py
+-rw-r--r--   0 cong       (501) staff       (20)     8010 2023-05-30 08:59:54.000000 goplus-0.1.1/swagger_client/configuration.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-06-21 02:44:53.976299 goplus-0.1.1/swagger_client/models/
+-rw-r--r--   0 cong       (501) staff       (20)     5480 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/models/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/abi_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/abi_param_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_erc1155_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/approve_token_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/audit_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    15392 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/contracts.py
+-rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/contracts_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5579 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/get_access_token_request.py
+-rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4619 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/models/get_defi_info_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    12280 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/models/get_defi_info_response_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/models/get_defi_info_response_result_owner.py
+-rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/models/map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/parse_abi_data_request.py
+-rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_address_contract.py
+-rw-r--r--   0 cong       (501) staff       (20)    23058 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_address_contract_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5012 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4898 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4733 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    42552 2023-06-02 06:08:47.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
+-rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     4767 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     5132 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5056 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5151 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4960 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_list_get_chains_list.py
+-rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_list_get_chains_list_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_list_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     4838 2023-06-21 02:21:31.000000 goplus-0.1.1/swagger_client/models/response_wrapper_map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     4860 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4771 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_phishing_site_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4899 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_token_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_token_security_dex.py
+-rw-r--r--   0 cong       (501) staff       (20)    10301 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_token_security_lp_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)    70422 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapper_token_security_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4670 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/response_wrapperobject.py
+-rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/models/ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.1/swagger_client/rest.py
```

### Comparing `goplus-0.1.0/LICENSE` & `goplus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goplus-0.1.0/PKG-INFO` & `goplus-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.0
+Version: 0.1.1
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,97 +42,104 @@
 ```
 
 ### Token Security
 
 ```python
 from goplus.token import Token
 
-data = Token(access_token=None).token_security(chain_id="1", addresses=["0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"])
-print(data)
+Token(access_token=None).token_security(chain_id="1", addresses=["0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"])
+
+# set timeout seconds
+Token(access_token=None).token_security(chain_id="1", addresses=["0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"], **{"_request_timeout": 10})
+
 ```
 
 ### Address Security
 
 ```python
 from goplus.address import Address
 
-res = Address(access_token=None).address_security(address="0xc8b759860149542a98a3eb57c14aadf59d6d89b9")
-print(res)
+Address(access_token=None).address_security(address="0xc8b759860149542a98a3eb57c14aadf59d6d89b9")
+
 ```
 
 
 ### Approval Security API v1
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).approve_security_v1(chain_id="1", address="0x4639cd8cd52ec1cf2e496a606ce28d8afb1c792f")
-print(res)
+Approve(access_token=None).approve_security_v1(chain_id="1", address="0x4639cd8cd52ec1cf2e496a606ce28d8afb1c792f")
+
 ```
 
 
 ### Approval Security API v2
 
 #### Token Approval Security
 
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).token_approve_security(chain_id="56", address="0xd018e2b543a2669410537f96293590138cacedf3")
-print(res)
+Approve(access_token=None).token_approve_security(chain_id="56", address="0xd018e2b543a2669410537f96293590138cacedf3")
+
 ```
 
 #### ERC721 NFT Approval Security
 
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).erc721_approve_security(chain_id="1", address="0xd95dbdab08a9fed2d71ac9c3028aac40905d8cf3")
-print(res)
+Approve(access_token=None).erc721_approve_security(chain_id="1", address="0xd95dbdab08a9fed2d71ac9c3028aac40905d8cf3")
+
 ```
 
 #### ERC1155 NFT Approval Security
 
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).erc1155_approve_security(chain_id="56", address="0xb0dccbb9c4a65a94a41a0165aaea79c8b2fc54ce")
-print(res)
+Approve(access_token=None).erc1155_approve_security(chain_id="56", address="0xb0dccbb9c4a65a94a41a0165aaea79c8b2fc54ce")
 
 ```
 
 
 ### Signature Data Decode
 ```python
 from goplus.decode import Decode
 
-res = Decode(access_token=None).signature_data_decode(chain_id="1",
+Decode(access_token=None).signature_data_decode(chain_id="1",
                                                     address="0x4cc8aa0c6ffbe18534584da9b592aa438733ee66",
                                                     data="0xa0712d680000000000000000000000000000000000000000000000000000000062fee481")
-print(res)
 
 ```
 ### NFT Security
 ```python
 from goplus.nft import Nft
 
-res = Nft(access_token=None).nft_security(chain_id="1", address="0x82f5ef9ddc3d231962ba57a9c2ebb307dc8d26c2")
-print(res)
+Nft(access_token=None).nft_security(chain_id="1", address="0x82f5ef9ddc3d231962ba57a9c2ebb307dc8d26c2")
 
 ```
 
 ### dApp Security Info API
 ```python
 from goplus.dapp import Dapp
 
-res = Dapp(access_token=None).dapp_security(url="https://for.tube")
-print(res)
+Dapp(access_token=None).dapp_security(url="https://for.tube")
 
 ```
 
 ### Phishing Site Detection API
 ```python
 from goplus.phishing_site import PushingSite
 
-res = PushingSite(access_token=None).pushing_site_security(url="https://xn--cm-68s.cc/")
-print(res)
+PushingSite(access_token=None).pushing_site_security(url="https://xn--cm-68s.cc/")
 
 ```
+
+### Rug-pull Detection API
+```python
+from goplus.rug_pull import RugPull
+
+RugPull().rug_pull_security(chain_id="1", address="0x6B175474E89094C44Da98b954EedeAC495271d0F")
+```
+
+
```

### Comparing `goplus-0.1.0/README.md` & `goplus-0.1.1/goplus.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: goplus
+Version: 0.1.1
+Summary: GoPlus SDK
+Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
+Author: GoPlus
+Author-email: service@gopluslabs.io
+License: Apache License 2.0
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # GoPlus SDK  For Python
 
 ### Installation
 
 ```
 pip install goplus
 ```
@@ -25,97 +42,104 @@
 ```
 
 ### Token Security
 
 ```python
 from goplus.token import Token
 
-data = Token(access_token=None).token_security(chain_id="1", addresses=["0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"])
-print(data)
+Token(access_token=None).token_security(chain_id="1", addresses=["0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"])
+
+# set timeout seconds
+Token(access_token=None).token_security(chain_id="1", addresses=["0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"], **{"_request_timeout": 10})
+
 ```
 
 ### Address Security
 
 ```python
 from goplus.address import Address
 
-res = Address(access_token=None).address_security(address="0xc8b759860149542a98a3eb57c14aadf59d6d89b9")
-print(res)
+Address(access_token=None).address_security(address="0xc8b759860149542a98a3eb57c14aadf59d6d89b9")
+
 ```
 
 
 ### Approval Security API v1
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).approve_security_v1(chain_id="1", address="0x4639cd8cd52ec1cf2e496a606ce28d8afb1c792f")
-print(res)
+Approve(access_token=None).approve_security_v1(chain_id="1", address="0x4639cd8cd52ec1cf2e496a606ce28d8afb1c792f")
+
 ```
 
 
 ### Approval Security API v2
 
 #### Token Approval Security
 
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).token_approve_security(chain_id="56", address="0xd018e2b543a2669410537f96293590138cacedf3")
-print(res)
+Approve(access_token=None).token_approve_security(chain_id="56", address="0xd018e2b543a2669410537f96293590138cacedf3")
+
 ```
 
 #### ERC721 NFT Approval Security
 
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).erc721_approve_security(chain_id="1", address="0xd95dbdab08a9fed2d71ac9c3028aac40905d8cf3")
-print(res)
+Approve(access_token=None).erc721_approve_security(chain_id="1", address="0xd95dbdab08a9fed2d71ac9c3028aac40905d8cf3")
+
 ```
 
 #### ERC1155 NFT Approval Security
 
 ```python
 from goplus.approve import Approve
 
-res = Approve(access_token=None).erc1155_approve_security(chain_id="56", address="0xb0dccbb9c4a65a94a41a0165aaea79c8b2fc54ce")
-print(res)
+Approve(access_token=None).erc1155_approve_security(chain_id="56", address="0xb0dccbb9c4a65a94a41a0165aaea79c8b2fc54ce")
 
 ```
 
 
 ### Signature Data Decode
 ```python
 from goplus.decode import Decode
 
-res = Decode(access_token=None).signature_data_decode(chain_id="1",
+Decode(access_token=None).signature_data_decode(chain_id="1",
                                                     address="0x4cc8aa0c6ffbe18534584da9b592aa438733ee66",
                                                     data="0xa0712d680000000000000000000000000000000000000000000000000000000062fee481")
-print(res)
 
 ```
 ### NFT Security
 ```python
 from goplus.nft import Nft
 
-res = Nft(access_token=None).nft_security(chain_id="1", address="0x82f5ef9ddc3d231962ba57a9c2ebb307dc8d26c2")
-print(res)
+Nft(access_token=None).nft_security(chain_id="1", address="0x82f5ef9ddc3d231962ba57a9c2ebb307dc8d26c2")
 
 ```
 
 ### dApp Security Info API
 ```python
 from goplus.dapp import Dapp
 
-res = Dapp(access_token=None).dapp_security(url="https://for.tube")
-print(res)
+Dapp(access_token=None).dapp_security(url="https://for.tube")
 
 ```
 
 ### Phishing Site Detection API
 ```python
 from goplus.phishing_site import PushingSite
 
-res = PushingSite(access_token=None).pushing_site_security(url="https://xn--cm-68s.cc/")
-print(res)
+PushingSite(access_token=None).pushing_site_security(url="https://xn--cm-68s.cc/")
 
 ```
+
+### Rug-pull Detection API
+```python
+from goplus.rug_pull import RugPull
+
+RugPull().rug_pull_security(chain_id="1", address="0x6B175474E89094C44Da98b954EedeAC495271d0F")
+```
+
+
```

### Comparing `goplus-0.1.0/setup.py` & `goplus-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.0/swagger_client/__init__.py` & `goplus-0.1.1/swagger_client/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -15,14 +15,15 @@
 from __future__ import absolute_import
 
 # import apis into sdk package
 from swagger_client.api.approve_controller_v_1_api import ApproveControllerV1Api
 from swagger_client.api.approve_controller_v_2_api import ApproveControllerV2Api
 from swagger_client.api.contract_abi_controller_api import ContractAbiControllerApi
 from swagger_client.api.dapp_controller_api import DappControllerApi
+from swagger_client.api.defi_controller_api import DefiControllerApi
 from swagger_client.api.nft_controller_api import NftControllerApi
 from swagger_client.api.token_controller_api import TokenControllerApi
 from swagger_client.api.token_controller_v_1_api import TokenControllerV1Api
 from swagger_client.api.website_controller_api import WebsiteControllerApi
 # import ApiClient
 from swagger_client.api_client import ApiClient
 from swagger_client.configuration import Configuration
@@ -39,41 +40,44 @@
 from swagger_client.models.audit_info import AuditInfo
 from swagger_client.models.contract_approve_response import ContractApproveResponse
 from swagger_client.models.contracts import Contracts
 from swagger_client.models.contracts_security import ContractsSecurity
 from swagger_client.models.dapp_contract_security_response import DappContractSecurityResponse
 from swagger_client.models.get_access_token_request import GetAccessTokenRequest
 from swagger_client.models.get_access_token_response import GetAccessTokenResponse
+from swagger_client.models.get_defi_info_response import GetDefiInfoResponse
+from swagger_client.models.get_defi_info_response_result import GetDefiInfoResponseResult
+from swagger_client.models.get_defi_info_response_result_owner import GetDefiInfoResponseResultOwner
 from swagger_client.models.json_object import JSONObject
-from swagger_client.models.mapstringstring import Mapstringstring
+from swagger_client.models.map_string_string import MapStringString
 from swagger_client.models.parse_abi_data_request import ParseAbiDataRequest
 from swagger_client.models.parse_abi_data_response import ParseAbiDataResponse
+from swagger_client.models.response_wrapper_address_contract import ResponseWrapperAddressContract
+from swagger_client.models.response_wrapper_address_contract_result import ResponseWrapperAddressContractResult
 from swagger_client.models.response_wrapper_contract_approve_response import ResponseWrapperContractApproveResponse
 from swagger_client.models.response_wrapper_dapp_contract_security_response import ResponseWrapperDappContractSecurityResponse
 from swagger_client.models.response_wrapper_get_access_token_response import ResponseWrapperGetAccessTokenResponse
+from swagger_client.models.response_wrapper_get_nft_info import ResponseWrapperGetNftInfo
+from swagger_client.models.response_wrapper_get_nft_info_result import ResponseWrapperGetNftInfoResult
+from swagger_client.models.response_wrapper_get_nft_info_result_privileged_burn import ResponseWrapperGetNftInfoResultPrivilegedBurn
+from swagger_client.models.response_wrapper_get_nft_info_result_privileged_minting import ResponseWrapperGetNftInfoResultPrivilegedMinting
+from swagger_client.models.response_wrapper_get_nft_info_result_same_nfts import ResponseWrapperGetNftInfoResultSameNfts
+from swagger_client.models.response_wrapper_get_nft_info_result_self_destruct import ResponseWrapperGetNftInfoResultSelfDestruct
+from swagger_client.models.response_wrapper_get_nft_info_result_transfer_without_approval import ResponseWrapperGetNftInfoResultTransferWithoutApproval
 from swagger_client.models.response_wrapper_json_object import ResponseWrapperJSONObject
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResult
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_privileged_burn import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_privileged_minting import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_same_nfts import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSameNfts
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_self_destruct import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct
-from swagger_client.models.response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_transfer_without_approval import ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultTransferWithoutApproval
 from swagger_client.models.response_wrapper_list_approve_nft1155_list_response import ResponseWrapperListApproveNFT1155ListResponse
 from swagger_client.models.response_wrapper_list_approve_nft_list_response import ResponseWrapperListApproveNFTListResponse
 from swagger_client.models.response_wrapper_list_approve_token_out_list_response import ResponseWrapperListApproveTokenOutListResponse
+from swagger_client.models.response_wrapper_list_get_chains_list import ResponseWrapperListGetChainsList
+from swagger_client.models.response_wrapper_list_get_chains_list_result import ResponseWrapperListGetChainsListResult
 from swagger_client.models.response_wrapper_list_json_object import ResponseWrapperListJSONObject
-from swagger_client.models.response_wrapper_list_json_object9524a1c652c545bf_b6c6898bfc3e93f3 import ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3
-from swagger_client.models.response_wrapper_list_json_object9524a1c652c545bfb6c6898bfc3e93f3_result import ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result
-from swagger_client.models.response_wrapper_mapstringstring import ResponseWrapperMapstringstring
-from swagger_client.models.response_wrapper_mapstringstring2a740de0_be5a4eb3_b6e4_a2cf0a2d8bf8 import ResponseWrapperMapstringstring2a740de0Be5a4eb3B6e4A2cf0a2d8bf8
-from swagger_client.models.response_wrapper_mapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8_result import ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result
+from swagger_client.models.response_wrapper_map_string_string import ResponseWrapperMapStringString
 from swagger_client.models.response_wrapper_parse_abi_data_response import ResponseWrapperParseAbiDataResponse
+from swagger_client.models.response_wrapper_phishing_site import ResponseWrapperPhishingSite
+from swagger_client.models.response_wrapper_phishing_site_result import ResponseWrapperPhishingSiteResult
 from swagger_client.models.response_wrapper_ta_token_security_response import ResponseWrapperTaTokenSecurityResponse
-from swagger_client.models.response_wrapper_ta_token_security_response205696bc_fb354bc5_ab26_ddc7cd495fe2 import ResponseWrapperTaTokenSecurityResponse205696bcFb354bc5Ab26Ddc7cd495fe2
-from swagger_client.models.response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_dex import ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Dex
-from swagger_client.models.response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_lp_holders import ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders
-from swagger_client.models.response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_result import ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result
+from swagger_client.models.response_wrapper_token_security import ResponseWrapperTokenSecurity
+from swagger_client.models.response_wrapper_token_security_dex import ResponseWrapperTokenSecurityDex
+from swagger_client.models.response_wrapper_token_security_lp_holders import ResponseWrapperTokenSecurityLpHolders
+from swagger_client.models.response_wrapper_token_security_result import ResponseWrapperTokenSecurityResult
 from swagger_client.models.response_wrapperobject import ResponseWrapperobject
-from swagger_client.models.response_wrapperobject545a2cea_b58741b4_aae7_f3d73df91255 import ResponseWrapperobject545a2ceaB58741b4Aae7F3d73df91255
-from swagger_client.models.response_wrapperobject545a2ceab58741b4aae7f3d73df91255_result import ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result
 from swagger_client.models.ta_token_security_response import TaTokenSecurityResponse
```

### Comparing `goplus-0.1.0/swagger_client/api/__init__.py` & `goplus-0.1.1/swagger_client/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,11 +3,12 @@
 # flake8: noqa
 
 # import apis into api package
 from swagger_client.api.approve_controller_v_1_api import ApproveControllerV1Api
 from swagger_client.api.approve_controller_v_2_api import ApproveControllerV2Api
 from swagger_client.api.contract_abi_controller_api import ContractAbiControllerApi
 from swagger_client.api.dapp_controller_api import DappControllerApi
+from swagger_client.api.defi_controller_api import DefiControllerApi
 from swagger_client.api.nft_controller_api import NftControllerApi
 from swagger_client.api.token_controller_api import TokenControllerApi
 from swagger_client.api.token_controller_v_1_api import TokenControllerV1Api
 from swagger_client.api.website_controller_api import WebsiteControllerApi
```

### Comparing `goplus-0.1.0/swagger_client/api/approve_controller_v_1_api.py` & `goplus-0.1.1/swagger_client/api/approve_controller_v_1_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -40,15 +40,15 @@
         >>> thread = api.address_contract_using_get1(address, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str address: address (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron.
-        :return: ResponseWrapperobject545a2ceaB58741b4Aae7F3d73df91255
+        :return: ResponseWrapperAddressContract
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.address_contract_using_get1_with_http_info(address, **kwargs)  # noqa: E501
         else:
@@ -63,15 +63,15 @@
         >>> thread = api.address_contract_using_get1_with_http_info(address, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str address: address (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron.
-        :return: ResponseWrapperobject545a2ceaB58741b4Aae7F3d73df91255
+        :return: ResponseWrapperAddressContract
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['address', 'authorization', 'chain_id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -121,15 +121,15 @@
             '/api/v1/address_security/{address}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ResponseWrapperobject545a2ceaB58741b4Aae7F3d73df91255',  # noqa: E501
+            response_type='ResponseWrapperAddressContract',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `goplus-0.1.0/swagger_client/api/approve_controller_v_2_api.py` & `goplus-0.1.1/swagger_client/api/approve_controller_v_2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/api/contract_abi_controller_api.py` & `goplus-0.1.1/swagger_client/api/contract_abi_controller_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/api/dapp_controller_api.py` & `goplus-0.1.1/swagger_client/api/dapp_controller_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/api/nft_controller_api.py` & `goplus-0.1.1/swagger_client/api/nft_controller_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -41,15 +41,15 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: Chain id, (eth: 1, bsc: 56, Polygon: 137, Avalanche: 43114) (required)
         :param str contract_addresses: NFT contract address (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str token_id: tokenId
-        :return: ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c
+        :return: ResponseWrapperGetNftInfo
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_nft_info_using_get1_with_http_info(chain_id, contract_addresses, **kwargs)  # noqa: E501
         else:
@@ -65,15 +65,15 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: Chain id, (eth: 1, bsc: 56, Polygon: 137, Avalanche: 43114) (required)
         :param str contract_addresses: NFT contract address (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str token_id: tokenId
-        :return: ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c
+        :return: ResponseWrapperGetNftInfo
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['chain_id', 'contract_addresses', 'authorization', 'token_id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -129,14 +129,14 @@
             '/api/v1/nft_security/{chain_id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c',  # noqa: E501
+            response_type='ResponseWrapperGetNftInfo',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `goplus-0.1.0/swagger_client/api/token_controller_api.py` & `goplus-0.1.1/swagger_client/api/token_controller_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/api/token_controller_v_1_api.py` & `goplus-0.1.1/swagger_client/api/token_controller_v_1_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -39,15 +39,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_chains_list_using_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str name: API name.
-        :return: ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3
+        :return: ResponseWrapperListGetChainsList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_chains_list_using_get_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -61,15 +61,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_chains_list_using_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str name: API name.
-        :return: ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3
+        :return: ResponseWrapperListGetChainsList
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['authorization', 'name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -113,15 +113,15 @@
             '/api/v1/supported_chains', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3',  # noqa: E501
+            response_type='ResponseWrapperListGetChainsList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -133,15 +133,15 @@
         >>> thread = api.token_security_using_get1(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron. (required)
         :param str contract_addresses: The contract address of tokens. (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
-        :return: ResponseWrapperTaTokenSecurityResponse205696bcFb354bc5Ab26Ddc7cd495fe2
+        :return: ResponseWrapperTokenSecurity
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.token_security_using_get1_with_http_info(chain_id, contract_addresses, **kwargs)  # noqa: E501
         else:
@@ -156,15 +156,15 @@
         >>> thread = api.token_security_using_get1_with_http_info(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron. (required)
         :param str contract_addresses: The contract address of tokens. (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
-        :return: ResponseWrapperTaTokenSecurityResponse205696bcFb354bc5Ab26Ddc7cd495fe2
+        :return: ResponseWrapperTokenSecurity
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['chain_id', 'contract_addresses', 'authorization']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -218,14 +218,14 @@
             '/api/v1/token_security/{chain_id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ResponseWrapperTaTokenSecurityResponse205696bcFb354bc5Ab26Ddc7cd495fe2',  # noqa: E501
+            response_type='ResponseWrapperTokenSecurity',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `goplus-0.1.0/swagger_client/api/website_controller_api.py` & `goplus-0.1.1/swagger_client/api/website_controller_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -39,15 +39,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.phishing_site_using_get(url, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str url: Url (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
-        :return: ResponseWrapperMapstringstring2a740de0Be5a4eb3B6e4A2cf0a2d8bf8
+        :return: ResponseWrapperPhishingSite
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.phishing_site_using_get_with_http_info(url, **kwargs)  # noqa: E501
         else:
@@ -61,15 +61,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.phishing_site_using_get_with_http_info(url, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str url: Url (required)
         :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
-        :return: ResponseWrapperMapstringstring2a740de0Be5a4eb3B6e4A2cf0a2d8bf8
+        :return: ResponseWrapperPhishingSite
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['url', 'authorization']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -117,14 +117,14 @@
             '/api/v1/phishing_site', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ResponseWrapperMapstringstring2a740de0Be5a4eb3B6e4A2cf0a2d8bf8',  # noqa: E501
+            response_type='ResponseWrapperPhishingSite',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `goplus-0.1.0/swagger_client/api_client.py` & `goplus-0.1.1/swagger_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/configuration.py` & `goplus-0.1.1/swagger_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/abi_address_info.py` & `goplus-0.1.1/swagger_client/models/abi_address_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/abi_param_info.py` & `goplus-0.1.1/swagger_client/models/abi_param_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_address_info.py` & `goplus-0.1.1/swagger_client/models/approve_address_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_erc1155_result.py` & `goplus-0.1.1/swagger_client/models/approve_erc1155_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_nft1155_list_response.py` & `goplus-0.1.1/swagger_client/models/approve_nft1155_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_nft_list_response.py` & `goplus-0.1.1/swagger_client/models/approve_nft_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_result.py` & `goplus-0.1.1/swagger_client/models/approve_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_token_out_list_response.py` & `goplus-0.1.1/swagger_client/models/approve_token_out_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/approve_token_result.py` & `goplus-0.1.1/swagger_client/models/approve_token_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/audit_info.py` & `goplus-0.1.1/swagger_client/models/audit_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/contract_approve_response.py` & `goplus-0.1.1/swagger_client/models/contract_approve_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/contracts.py` & `goplus-0.1.1/swagger_client/models/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/contracts_security.py` & `goplus-0.1.1/swagger_client/models/contracts_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/dapp_contract_security_response.py` & `goplus-0.1.1/swagger_client/models/dapp_contract_security_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/get_access_token_request.py` & `goplus-0.1.1/swagger_client/models/get_access_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/get_access_token_response.py` & `goplus-0.1.1/swagger_client/models/get_access_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/json_object.py` & `goplus-0.1.1/swagger_client/models/json_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/mapstringstring.py` & `goplus-0.1.1/swagger_client/models/map_string_string.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Mapstringstring(dict):
+class MapStringString(dict):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,15 +34,15 @@
 
     attribute_map = {
     }
     if hasattr(dict, "attribute_map"):
         attribute_map.update(dict.attribute_map)
 
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Mapstringstring - a model defined in Swagger"""  # noqa: E501
+        """MapStringString - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
         dict.__init__(self, *args, **kwargs)
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -59,15 +59,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Mapstringstring, dict):
+        if issubclass(MapStringString, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -75,15 +75,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Mapstringstring):
+        if not isinstance(other, MapStringString):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/parse_abi_data_request.py` & `goplus-0.1.1/swagger_client/models/parse_abi_data_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -27,38 +27,43 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'chain_id': 'str',
         'contract_address': 'str',
         'data': 'str',
+        'input': 'dict(str, object)',
         'signer': 'str',
         'transcation_type': 'str'
     }
 
     attribute_map = {
         'chain_id': 'chain_id',
         'contract_address': 'contract_address',
         'data': 'data',
+        'input': 'input',
         'signer': 'signer',
         'transcation_type': 'transcation_type'
     }
 
-    def __init__(self, chain_id=None, contract_address=None, data=None, signer=None, transcation_type=None):  # noqa: E501
+    def __init__(self, chain_id=None, contract_address=None, data=None, input=None, signer=None, transcation_type=None):  # noqa: E501
         """ParseAbiDataRequest - a model defined in Swagger"""  # noqa: E501
         self._chain_id = None
         self._contract_address = None
         self._data = None
+        self._input = None
         self._signer = None
         self._transcation_type = None
         self.discriminator = None
         self.chain_id = chain_id
         if contract_address is not None:
             self.contract_address = contract_address
         self.data = data
+        if input is not None:
+            self.input = input
         if signer is not None:
             self.signer = signer
         if transcation_type is not None:
             self.transcation_type = transcation_type
 
     @property
     def chain_id(self):
@@ -130,14 +135,37 @@
         """
         if data is None:
             raise ValueError("Invalid value for `data`, must not be `None`")  # noqa: E501
 
         self._data = data
 
     @property
+    def input(self):
+        """Gets the input of this ParseAbiDataRequest.  # noqa: E501
+
+        input info  # noqa: E501
+
+        :return: The input of this ParseAbiDataRequest.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._input
+
+    @input.setter
+    def input(self, input):
+        """Sets the input of this ParseAbiDataRequest.
+
+        input info  # noqa: E501
+
+        :param input: The input of this ParseAbiDataRequest.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._input = input
+
+    @property
     def signer(self):
         """Gets the signer of this ParseAbiDataRequest.  # noqa: E501
 
         Carrying the signer and contract address will help to decode more information.  # noqa: E501
 
         :return: The signer of this ParseAbiDataRequest.  # noqa: E501
         :rtype: str
@@ -172,15 +200,15 @@
         """Sets the transcation_type of this ParseAbiDataRequest.
 
         Transaction type  # noqa: E501
 
         :param transcation_type: The transcation_type of this ParseAbiDataRequest.  # noqa: E501
         :type: str
         """
-        allowed_values = ["COMMON", "ETH_SIGNTYPEDDATA_V4", "PERSONAL_SIGN", "ETH_SIGN"]  # noqa: E501
+        allowed_values = ["common", "eth_signTypedData_v4", "personal_sign", "eth_sign"]  # noqa: E501
         if transcation_type not in allowed_values:
             raise ValueError(
                 "Invalid value for `transcation_type` ({0}), must be one of {1}"  # noqa: E501
                 .format(transcation_type, allowed_values)
             )
 
         self._transcation_type = transcation_type
```

### Comparing `goplus-0.1.0/swagger_client/models/parse_abi_data_response.py` & `goplus-0.1.1/swagger_client/models/parse_abi_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_contract_approve_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_contract_approve_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_dapp_contract_security_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_dapp_contract_security_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_get_access_token_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_access_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
@@ -24,37 +24,58 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'result': 'GetAccessTokenResponse',
         'code': 'int',
-        'message': 'str',
-        'result': 'GetAccessTokenResponse'
+        'message': 'str'
     }
 
     attribute_map = {
+        'result': 'result',
         'code': 'code',
-        'message': 'message',
-        'result': 'result'
+        'message': 'message'
     }
 
-    def __init__(self, code=None, message=None, result=None):  # noqa: E501
+    def __init__(self, result=None, code=None, message=None):  # noqa: E501
         """ResponseWrapperGetAccessTokenResponse - a model defined in Swagger"""  # noqa: E501
+        self._result = None
         self._code = None
         self._message = None
-        self._result = None
         self.discriminator = None
+        if result is not None:
+            self.result = result
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
-        if result is not None:
-            self.result = result
+
+    @property
+    def result(self):
+        """Gets the result of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
+
+
+        :return: The result of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
+        :rtype: GetAccessTokenResponse
+        """
+        return self._result
+
+    @result.setter
+    def result(self, result):
+        """Sets the result of this ResponseWrapperGetAccessTokenResponse.
+
+
+        :param result: The result of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
+        :type: GetAccessTokenResponse
+        """
+
+        self._result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
@@ -94,35 +115,14 @@
 
         :param message: The message of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
-    @property
-    def result(self):
-        """Gets the result of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
-
-
-        :return: The result of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
-        :rtype: GetAccessTokenResponse
-        """
-        return self._result
-
-    @result.setter
-    def result(self, result):
-        """Sets the result of this ResponseWrapperGetAccessTokenResponse.
-
-
-        :param result: The result of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
-        :type: GetAccessTokenResponse
-        """
-
-        self._result = result
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_json_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfe_b2f246e4936a6968cc97141b.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b(object):
+class ResponseWrapperListApproveTokenOutListResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult'
+        'result': 'list[ApproveTokenOutListResponse]'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperListApproveTokenOutListResponse - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        """Gets the code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        :return: The code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.
+        """Sets the code of this ResponseWrapperListApproveTokenOutListResponse.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        :param code: The code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        """Gets the message of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        :return: The message of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.
+        """Sets the message of this ResponseWrapperListApproveTokenOutListResponse.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        :param message: The message of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
+        """Gets the result of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
 
+        Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
-        :rtype: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult
+        :return: The result of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        :rtype: list[ApproveTokenOutListResponse]
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.
+        """Sets the result of this ResponseWrapperListApproveTokenOutListResponse.
 
+        Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b.  # noqa: E501
-        :type: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult
+        :param result: The result of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        :type: list[ApproveTokenOutListResponse]
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -136,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b, dict):
+        if issubclass(ResponseWrapperListApproveTokenOutListResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject59da6cfeB2f246e4936a6968cc97141b):
+        if not isinstance(other, ResponseWrapperListApproveTokenOutListResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult(object):
+class ResponseWrapperGetNftInfoResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,35 +30,36 @@
     swagger_types = {
         'traded_volume_24h': 'float',
         'total_volume': 'float',
         'red_check_mark': 'int',
         'nft_proxy': 'int',
         'restricted_approval': 'int',
         'highest_price': 'float',
-        'transfer_without_approval': 'ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultTransferWithoutApproval',
+        'transfer_without_approval': 'ResponseWrapperGetNftInfoResultTransferWithoutApproval',
         'discord_url': 'str',
         'nft_open_source': 'int',
-        'privileged_minting': 'ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting',
-        'nft_owner_number': 'float',
+        'privileged_minting': 'ResponseWrapperGetNftInfoResultPrivilegedMinting',
+        'nft_owner_number': 'int',
         'trust_list': 'int',
         'token_id': 'str',
         'lowest_price_24h': 'float',
         'average_price_24h': 'float',
         'nft_erc': 'str',
         'creator_address': 'str',
         'medium_url': 'str',
         'malicious_nft_contract': 'int',
-        'privileged_burn': 'ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedBurn',
+        'privileged_burn': 'ResponseWrapperGetNftInfoResultPrivilegedBurn',
         'twitter_url': 'str',
         'nft_symbol': 'str',
         'nft_description': 'str',
-        'self_destruct': 'ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSelfDestruct',
+        'self_destruct': 'ResponseWrapperGetNftInfoResultSelfDestruct',
         'metadata_frozen': 'int',
+        'token_owner': 'str',
         'nft_verified': 'int',
-        'same_nfts': 'list[ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts]',
+        'same_nfts': 'list[ResponseWrapperGetNftInfoResultSameNfts]',
         'nft_items': 'int',
         'oversupply_minting': 'int',
         'nft_name': 'str',
         'website_url': 'str',
         'github_url': 'str',
         'telegram_url': 'str',
         'sales_24h': 'float',
@@ -87,28 +88,29 @@
         'malicious_nft_contract': 'malicious_nft_contract',
         'privileged_burn': 'privileged_burn',
         'twitter_url': 'twitter_url',
         'nft_symbol': 'nft_symbol',
         'nft_description': 'nft_description',
         'self_destruct': 'self_destruct',
         'metadata_frozen': 'metadata_frozen',
+        'token_owner': 'token_owner',
         'nft_verified': 'nft_verified',
         'same_nfts': 'same_nfts',
         'nft_items': 'nft_items',
         'oversupply_minting': 'oversupply_minting',
         'nft_name': 'nft_name',
         'website_url': 'website_url',
         'github_url': 'github_url',
         'telegram_url': 'telegram_url',
         'sales_24h': 'sales_24h',
         'create_block_number': 'create_block_number'
     }
 
-    def __init__(self, traded_volume_24h=None, total_volume=None, red_check_mark=None, nft_proxy=None, restricted_approval=None, highest_price=None, transfer_without_approval=None, discord_url=None, nft_open_source=None, privileged_minting=None, nft_owner_number=None, trust_list=None, token_id=None, lowest_price_24h=None, average_price_24h=None, nft_erc=None, creator_address=None, medium_url=None, malicious_nft_contract=None, privileged_burn=None, twitter_url=None, nft_symbol=None, nft_description=None, self_destruct=None, metadata_frozen=None, nft_verified=None, same_nfts=None, nft_items=None, oversupply_minting=None, nft_name=None, website_url=None, github_url=None, telegram_url=None, sales_24h=None, create_block_number=None):  # noqa: E501
-        """ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, traded_volume_24h=None, total_volume=None, red_check_mark=None, nft_proxy=None, restricted_approval=None, highest_price=None, transfer_without_approval=None, discord_url=None, nft_open_source=None, privileged_minting=None, nft_owner_number=None, trust_list=None, token_id=None, lowest_price_24h=None, average_price_24h=None, nft_erc=None, creator_address=None, medium_url=None, malicious_nft_contract=None, privileged_burn=None, twitter_url=None, nft_symbol=None, nft_description=None, self_destruct=None, metadata_frozen=None, token_owner=None, nft_verified=None, same_nfts=None, nft_items=None, oversupply_minting=None, nft_name=None, website_url=None, github_url=None, telegram_url=None, sales_24h=None, create_block_number=None):  # noqa: E501
+        """ResponseWrapperGetNftInfoResult - a model defined in Swagger"""  # noqa: E501
         self._traded_volume_24h = None
         self._total_volume = None
         self._red_check_mark = None
         self._nft_proxy = None
         self._restricted_approval = None
         self._highest_price = None
         self._transfer_without_approval = None
@@ -126,14 +128,15 @@
         self._malicious_nft_contract = None
         self._privileged_burn = None
         self._twitter_url = None
         self._nft_symbol = None
         self._nft_description = None
         self._self_destruct = None
         self._metadata_frozen = None
+        self._token_owner = None
         self._nft_verified = None
         self._same_nfts = None
         self._nft_items = None
         self._oversupply_minting = None
         self._nft_name = None
         self._website_url = None
         self._github_url = None
@@ -187,14 +190,16 @@
             self.nft_symbol = nft_symbol
         if nft_description is not None:
             self.nft_description = nft_description
         if self_destruct is not None:
             self.self_destruct = self_destruct
         if metadata_frozen is not None:
             self.metadata_frozen = metadata_frozen
+        if token_owner is not None:
+            self.token_owner = token_owner
         if nft_verified is not None:
             self.nft_verified = nft_verified
         if same_nfts is not None:
             self.same_nfts = same_nfts
         if nft_items is not None:
             self.nft_items = nft_items
         if oversupply_minting is not None:
@@ -210,804 +215,827 @@
         if sales_24h is not None:
             self.sales_24h = sales_24h
         if create_block_number is not None:
             self.create_block_number = create_block_number
 
     @property
     def traded_volume_24h(self):
-        """Gets the traded_volume_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the traded_volume_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the trading volume of the NFT in 24h.  # noqa: E501
 
-        :return: The traded_volume_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The traded_volume_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: float
         """
         return self._traded_volume_24h
 
     @traded_volume_24h.setter
     def traded_volume_24h(self, traded_volume_24h):
-        """Sets the traded_volume_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the traded_volume_24h of this ResponseWrapperGetNftInfoResult.
 
         It describes the trading volume of the NFT in 24h.  # noqa: E501
 
-        :param traded_volume_24h: The traded_volume_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param traded_volume_24h: The traded_volume_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: float
         """
 
         self._traded_volume_24h = traded_volume_24h
 
     @property
     def total_volume(self):
-        """Gets the total_volume of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the total_volume of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the total volume of the NFT.  # noqa: E501
 
-        :return: The total_volume of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The total_volume of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: float
         """
         return self._total_volume
 
     @total_volume.setter
     def total_volume(self, total_volume):
-        """Sets the total_volume of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the total_volume of this ResponseWrapperGetNftInfoResult.
 
         It describes the total volume of the NFT.  # noqa: E501
 
-        :param total_volume: The total_volume of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param total_volume: The total_volume of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: float
         """
 
         self._total_volume = total_volume
 
     @property
     def red_check_mark(self):
-        """Gets the red_check_mark of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the red_check_mark of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         red check mark  # noqa: E501
 
-        :return: The red_check_mark of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The red_check_mark of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._red_check_mark
 
     @red_check_mark.setter
     def red_check_mark(self, red_check_mark):
-        """Sets the red_check_mark of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the red_check_mark of this ResponseWrapperGetNftInfoResult.
 
         red check mark  # noqa: E501
 
-        :param red_check_mark: The red_check_mark of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param red_check_mark: The red_check_mark of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._red_check_mark = red_check_mark
 
     @property
     def nft_proxy(self):
-        """Gets the nft_proxy of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_proxy of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether this NFT contract has a proxy contract.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:(1) When \"is_open_source\": \"0\", it will return \"null\". (2) Most Proxy contracts are accompanied by modifiable implementation contracts, and implementation contracts may contain significant potential risk.)  # noqa: E501
 
-        :return: The nft_proxy of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_proxy of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._nft_proxy
 
     @nft_proxy.setter
     def nft_proxy(self, nft_proxy):
-        """Sets the nft_proxy of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_proxy of this ResponseWrapperGetNftInfoResult.
 
         It describes whether this NFT contract has a proxy contract.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:(1) When \"is_open_source\": \"0\", it will return \"null\". (2) Most Proxy contracts are accompanied by modifiable implementation contracts, and implementation contracts may contain significant potential risk.)  # noqa: E501
 
-        :param nft_proxy: The nft_proxy of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_proxy: The nft_proxy of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._nft_proxy = nft_proxy
 
     @property
     def restricted_approval(self):
-        """Gets the restricted_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the restricted_approval of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether the NFT contract can restrict the approval, resulting in NFT can not be traded on the NFT DEX. \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:If this risk exists, it means that users will not be able to trade the NFT on the exchange and only privileged users in the whitelist will be able to trade normally.)  # noqa: E501
 
-        :return: The restricted_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The restricted_approval of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._restricted_approval
 
     @restricted_approval.setter
     def restricted_approval(self, restricted_approval):
-        """Sets the restricted_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the restricted_approval of this ResponseWrapperGetNftInfoResult.
 
         It describes whether the NFT contract can restrict the approval, resulting in NFT can not be traded on the NFT DEX. \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:If this risk exists, it means that users will not be able to trade the NFT on the exchange and only privileged users in the whitelist will be able to trade normally.)  # noqa: E501
 
-        :param restricted_approval: The restricted_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param restricted_approval: The restricted_approval of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._restricted_approval = restricted_approval
 
     @property
     def highest_price(self):
-        """Gets the highest_price of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the highest_price of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the highest price of the NFT.  # noqa: E501
 
-        :return: The highest_price of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The highest_price of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: float
         """
         return self._highest_price
 
     @highest_price.setter
     def highest_price(self, highest_price):
-        """Sets the highest_price of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the highest_price of this ResponseWrapperGetNftInfoResult.
 
         It describes the highest price of the NFT.  # noqa: E501
 
-        :param highest_price: The highest_price of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param highest_price: The highest_price of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: float
         """
 
         self._highest_price = highest_price
 
     @property
     def transfer_without_approval(self):
-        """Gets the transfer_without_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the transfer_without_approval of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
 
-        :return: The transfer_without_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :rtype: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultTransferWithoutApproval
+        :return: The transfer_without_approval of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: ResponseWrapperGetNftInfoResultTransferWithoutApproval
         """
         return self._transfer_without_approval
 
     @transfer_without_approval.setter
     def transfer_without_approval(self, transfer_without_approval):
-        """Sets the transfer_without_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the transfer_without_approval of this ResponseWrapperGetNftInfoResult.
 
 
-        :param transfer_without_approval: The transfer_without_approval of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :type: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultTransferWithoutApproval
+        :param transfer_without_approval: The transfer_without_approval of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: ResponseWrapperGetNftInfoResultTransferWithoutApproval
         """
 
         self._transfer_without_approval = transfer_without_approval
 
     @property
     def discord_url(self):
-        """Gets the discord_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the discord_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the discord url of the NFT. Return “null” means there is no discord url or didn't find the discord url.  # noqa: E501
 
-        :return: The discord_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The discord_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._discord_url
 
     @discord_url.setter
     def discord_url(self, discord_url):
-        """Sets the discord_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the discord_url of this ResponseWrapperGetNftInfoResult.
 
         It describes the discord url of the NFT. Return “null” means there is no discord url or didn't find the discord url.  # noqa: E501
 
-        :param discord_url: The discord_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param discord_url: The discord_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._discord_url = discord_url
 
     @property
     def nft_open_source(self):
-        """Gets the nft_open_source of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_open_source of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether this contract is open source.  \"1\" means true;  \"0\" means false.(Notice:Un-open-sourced contracts may hide various unknown mechanisms and are extremely risky. When the contract is not open source, we will not be able to detect other risk items.)  # noqa: E501
 
-        :return: The nft_open_source of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_open_source of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._nft_open_source
 
     @nft_open_source.setter
     def nft_open_source(self, nft_open_source):
-        """Sets the nft_open_source of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_open_source of this ResponseWrapperGetNftInfoResult.
 
         It describes whether this contract is open source.  \"1\" means true;  \"0\" means false.(Notice:Un-open-sourced contracts may hide various unknown mechanisms and are extremely risky. When the contract is not open source, we will not be able to detect other risk items.)  # noqa: E501
 
-        :param nft_open_source: The nft_open_source of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_open_source: The nft_open_source of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._nft_open_source = nft_open_source
 
     @property
     def privileged_minting(self):
-        """Gets the privileged_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the privileged_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
 
-        :return: The privileged_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :rtype: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting
+        :return: The privileged_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: ResponseWrapperGetNftInfoResultPrivilegedMinting
         """
         return self._privileged_minting
 
     @privileged_minting.setter
     def privileged_minting(self, privileged_minting):
-        """Sets the privileged_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the privileged_minting of this ResponseWrapperGetNftInfoResult.
 
 
-        :param privileged_minting: The privileged_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :type: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting
+        :param privileged_minting: The privileged_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: ResponseWrapperGetNftInfoResultPrivilegedMinting
         """
 
         self._privileged_minting = privileged_minting
 
     @property
     def nft_owner_number(self):
-        """Gets the nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_owner_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the holders of the NFT.  # noqa: E501
 
-        :return: The nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :rtype: float
+        :return: The nft_owner_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: int
         """
         return self._nft_owner_number
 
     @nft_owner_number.setter
     def nft_owner_number(self, nft_owner_number):
-        """Sets the nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_owner_number of this ResponseWrapperGetNftInfoResult.
 
         It describes the holders of the NFT.  # noqa: E501
 
-        :param nft_owner_number: The nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :type: float
+        :param nft_owner_number: The nft_owner_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: int
         """
 
         self._nft_owner_number = nft_owner_number
 
     @property
     def trust_list(self):
-        """Gets the trust_list of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the trust_list of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether the NFT is a famous and trustworthy one. \"1\" means true;  Return \"null\" means no result.(Notice:(1) Only \"trust_list\": \"1\" means it is a famous and trustworthy NFT. (2) Return \"null\" doesn't mean it is risky.Th)  # noqa: E501
 
-        :return: The trust_list of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The trust_list of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._trust_list
 
     @trust_list.setter
     def trust_list(self, trust_list):
-        """Sets the trust_list of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the trust_list of this ResponseWrapperGetNftInfoResult.
 
         It describes whether the NFT is a famous and trustworthy one. \"1\" means true;  Return \"null\" means no result.(Notice:(1) Only \"trust_list\": \"1\" means it is a famous and trustworthy NFT. (2) Return \"null\" doesn't mean it is risky.Th)  # noqa: E501
 
-        :param trust_list: The trust_list of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param trust_list: The trust_list of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._trust_list = trust_list
 
     @property
     def token_id(self):
-        """Gets the token_id of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the token_id of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         token_id  # noqa: E501
 
-        :return: The token_id of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The token_id of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._token_id
 
     @token_id.setter
     def token_id(self, token_id):
-        """Sets the token_id of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the token_id of this ResponseWrapperGetNftInfoResult.
 
         token_id  # noqa: E501
 
-        :param token_id: The token_id of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param token_id: The token_id of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._token_id = token_id
 
     @property
     def lowest_price_24h(self):
-        """Gets the lowest_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the lowest_price_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the lowest price of the NFT in 24h.  # noqa: E501
 
-        :return: The lowest_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The lowest_price_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: float
         """
         return self._lowest_price_24h
 
     @lowest_price_24h.setter
     def lowest_price_24h(self, lowest_price_24h):
-        """Sets the lowest_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the lowest_price_24h of this ResponseWrapperGetNftInfoResult.
 
         It describes the lowest price of the NFT in 24h.  # noqa: E501
 
-        :param lowest_price_24h: The lowest_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param lowest_price_24h: The lowest_price_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: float
         """
 
         self._lowest_price_24h = lowest_price_24h
 
     @property
     def average_price_24h(self):
-        """Gets the average_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the average_price_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the average price of the NFT in 24h.  # noqa: E501
 
-        :return: The average_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The average_price_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: float
         """
         return self._average_price_24h
 
     @average_price_24h.setter
     def average_price_24h(self, average_price_24h):
-        """Sets the average_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the average_price_24h of this ResponseWrapperGetNftInfoResult.
 
         It describes the average price of the NFT in 24h.  # noqa: E501
 
-        :param average_price_24h: The average_price_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param average_price_24h: The average_price_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: float
         """
 
         self._average_price_24h = average_price_24h
 
     @property
     def nft_erc(self):
-        """Gets the nft_erc of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_erc of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the ERC protocol of the NFT. Example: \"nft_erc\": \"erc721\"  # noqa: E501
 
-        :return: The nft_erc of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_erc of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._nft_erc
 
     @nft_erc.setter
     def nft_erc(self, nft_erc):
-        """Sets the nft_erc of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_erc of this ResponseWrapperGetNftInfoResult.
 
         It describes the ERC protocol of the NFT. Example: \"nft_erc\": \"erc721\"  # noqa: E501
 
-        :param nft_erc: The nft_erc of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_erc: The nft_erc of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._nft_erc = nft_erc
 
     @property
     def creator_address(self):
-        """Gets the creator_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the creator_address of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the creator address of the NFT. Example: \"creator_address\": \"0x1ee0af784b96bb55ece98c9b15675726b0da1b6b\"; Return “null” means that we didn't find the creator address.  # noqa: E501
 
-        :return: The creator_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The creator_address of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._creator_address
 
     @creator_address.setter
     def creator_address(self, creator_address):
-        """Sets the creator_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the creator_address of this ResponseWrapperGetNftInfoResult.
 
         It describes the creator address of the NFT. Example: \"creator_address\": \"0x1ee0af784b96bb55ece98c9b15675726b0da1b6b\"; Return “null” means that we didn't find the creator address.  # noqa: E501
 
-        :param creator_address: The creator_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param creator_address: The creator_address of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._creator_address = creator_address
 
     @property
     def medium_url(self):
-        """Gets the medium_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the medium_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the medium url of the NFT. Return “null” means there is no medium url or didn't find the medium url.  # noqa: E501
 
-        :return: The medium_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The medium_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._medium_url
 
     @medium_url.setter
     def medium_url(self, medium_url):
-        """Sets the medium_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the medium_url of this ResponseWrapperGetNftInfoResult.
 
         It describes the medium url of the NFT. Return “null” means there is no medium url or didn't find the medium url.  # noqa: E501
 
-        :param medium_url: The medium_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param medium_url: The medium_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._medium_url = medium_url
 
     @property
     def malicious_nft_contract(self):
-        """Gets the malicious_nft_contract of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the malicious_nft_contract of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether this NFT has performed malicious behaviors. \"1\" means true; \"0\" means false.(Notice:Malicious behaviors include random additions, blacklist abuse, falsified transactions, and other high-risk behaviors. Interacting with NFTs flagged as Malicious may contain a high level of risk)  # noqa: E501
 
-        :return: The malicious_nft_contract of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The malicious_nft_contract of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._malicious_nft_contract
 
     @malicious_nft_contract.setter
     def malicious_nft_contract(self, malicious_nft_contract):
-        """Sets the malicious_nft_contract of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the malicious_nft_contract of this ResponseWrapperGetNftInfoResult.
 
         It describes whether this NFT has performed malicious behaviors. \"1\" means true; \"0\" means false.(Notice:Malicious behaviors include random additions, blacklist abuse, falsified transactions, and other high-risk behaviors. Interacting with NFTs flagged as Malicious may contain a high level of risk)  # noqa: E501
 
-        :param malicious_nft_contract: The malicious_nft_contract of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param malicious_nft_contract: The malicious_nft_contract of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._malicious_nft_contract = malicious_nft_contract
 
     @property
     def privileged_burn(self):
-        """Gets the privileged_burn of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the privileged_burn of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
 
-        :return: The privileged_burn of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :rtype: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedBurn
+        :return: The privileged_burn of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: ResponseWrapperGetNftInfoResultPrivilegedBurn
         """
         return self._privileged_burn
 
     @privileged_burn.setter
     def privileged_burn(self, privileged_burn):
-        """Sets the privileged_burn of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the privileged_burn of this ResponseWrapperGetNftInfoResult.
 
 
-        :param privileged_burn: The privileged_burn of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :type: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedBurn
+        :param privileged_burn: The privileged_burn of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: ResponseWrapperGetNftInfoResultPrivilegedBurn
         """
 
         self._privileged_burn = privileged_burn
 
     @property
     def twitter_url(self):
-        """Gets the twitter_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the twitter_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the twitter url of the NFT. Return “null” means there is no twitter url or didn't find the twitter url.  # noqa: E501
 
-        :return: The twitter_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The twitter_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._twitter_url
 
     @twitter_url.setter
     def twitter_url(self, twitter_url):
-        """Sets the twitter_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the twitter_url of this ResponseWrapperGetNftInfoResult.
 
         It describes the twitter url of the NFT. Return “null” means there is no twitter url or didn't find the twitter url.  # noqa: E501
 
-        :param twitter_url: The twitter_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param twitter_url: The twitter_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._twitter_url = twitter_url
 
     @property
     def nft_symbol(self):
-        """Gets the nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_symbol of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         nft_symbol  # noqa: E501
 
-        :return: The nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_symbol of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._nft_symbol
 
     @nft_symbol.setter
     def nft_symbol(self, nft_symbol):
-        """Sets the nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_symbol of this ResponseWrapperGetNftInfoResult.
 
         nft_symbol  # noqa: E501
 
-        :param nft_symbol: The nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_symbol: The nft_symbol of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._nft_symbol = nft_symbol
 
     @property
     def nft_description(self):
-        """Gets the nft_description of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_description of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the introduction of the NFT. Return “null” means there is no description of the NFT.  # noqa: E501
 
-        :return: The nft_description of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_description of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._nft_description
 
     @nft_description.setter
     def nft_description(self, nft_description):
-        """Sets the nft_description of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_description of this ResponseWrapperGetNftInfoResult.
 
         It describes the introduction of the NFT. Return “null” means there is no description of the NFT.  # noqa: E501
 
-        :param nft_description: The nft_description of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_description: The nft_description of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._nft_description = nft_description
 
     @property
     def self_destruct(self):
-        """Gets the self_destruct of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the self_destruct of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
 
-        :return: The self_destruct of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :rtype: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSelfDestruct
+        :return: The self_destruct of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: ResponseWrapperGetNftInfoResultSelfDestruct
         """
         return self._self_destruct
 
     @self_destruct.setter
     def self_destruct(self, self_destruct):
-        """Sets the self_destruct of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the self_destruct of this ResponseWrapperGetNftInfoResult.
 
 
-        :param self_destruct: The self_destruct of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :type: ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSelfDestruct
+        :param self_destruct: The self_destruct of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: ResponseWrapperGetNftInfoResultSelfDestruct
         """
 
         self._self_destruct = self_destruct
 
     @property
     def metadata_frozen(self):
-        """Gets the metadata_frozen of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the metadata_frozen of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         metadata_frozen  # noqa: E501
 
-        :return: The metadata_frozen of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The metadata_frozen of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._metadata_frozen
 
     @metadata_frozen.setter
     def metadata_frozen(self, metadata_frozen):
-        """Sets the metadata_frozen of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the metadata_frozen of this ResponseWrapperGetNftInfoResult.
 
         metadata_frozen  # noqa: E501
 
-        :param metadata_frozen: The metadata_frozen of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param metadata_frozen: The metadata_frozen of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._metadata_frozen = metadata_frozen
 
     @property
+    def token_owner(self):
+        """Gets the token_owner of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+
+        token_owner  # noqa: E501
+
+        :return: The token_owner of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._token_owner
+
+    @token_owner.setter
+    def token_owner(self, token_owner):
+        """Sets the token_owner of this ResponseWrapperGetNftInfoResult.
+
+        token_owner  # noqa: E501
+
+        :param token_owner: The token_owner of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: str
+        """
+
+        self._token_owner = token_owner
+
+    @property
     def nft_verified(self):
-        """Gets the nft_verified of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_verified of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether the NFT is verified. \"1\" means that the NFT is verified; \"0\" means that we did not find any information about whether the NFT is verified.  # noqa: E501
 
-        :return: The nft_verified of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_verified of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._nft_verified
 
     @nft_verified.setter
     def nft_verified(self, nft_verified):
-        """Sets the nft_verified of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_verified of this ResponseWrapperGetNftInfoResult.
 
         It describes whether the NFT is verified. \"1\" means that the NFT is verified; \"0\" means that we did not find any information about whether the NFT is verified.  # noqa: E501
 
-        :param nft_verified: The nft_verified of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_verified: The nft_verified of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._nft_verified = nft_verified
 
     @property
     def same_nfts(self):
-        """Gets the same_nfts of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the same_nfts of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the info of other NFTs with duplicate name and symbol.  # noqa: E501
 
-        :return: The same_nfts of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :rtype: list[ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts]
+        :return: The same_nfts of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :rtype: list[ResponseWrapperGetNftInfoResultSameNfts]
         """
         return self._same_nfts
 
     @same_nfts.setter
     def same_nfts(self, same_nfts):
-        """Sets the same_nfts of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the same_nfts of this ResponseWrapperGetNftInfoResult.
 
         It describes the info of other NFTs with duplicate name and symbol.  # noqa: E501
 
-        :param same_nfts: The same_nfts of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
-        :type: list[ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts]
+        :param same_nfts: The same_nfts of this ResponseWrapperGetNftInfoResult.  # noqa: E501
+        :type: list[ResponseWrapperGetNftInfoResultSameNfts]
         """
 
         self._same_nfts = same_nfts
 
     @property
     def nft_items(self):
-        """Gets the nft_items of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_items of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the numbers of the NFT.  # noqa: E501
 
-        :return: The nft_items of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_items of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._nft_items
 
     @nft_items.setter
     def nft_items(self, nft_items):
-        """Sets the nft_items of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_items of this ResponseWrapperGetNftInfoResult.
 
         It describes the numbers of the NFT.  # noqa: E501
 
-        :param nft_items: The nft_items of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_items: The nft_items of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._nft_items = nft_items
 
     @property
     def oversupply_minting(self):
-        """Gets the oversupply_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the oversupply_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes whether this NFT owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:Oversupply minting refers to the existence of a special mint method in the NFT contract — the owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.)  # noqa: E501
 
-        :return: The oversupply_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The oversupply_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._oversupply_minting
 
     @oversupply_minting.setter
     def oversupply_minting(self, oversupply_minting):
-        """Sets the oversupply_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the oversupply_minting of this ResponseWrapperGetNftInfoResult.
 
         It describes whether this NFT owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:Oversupply minting refers to the existence of a special mint method in the NFT contract — the owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.)  # noqa: E501
 
-        :param oversupply_minting: The oversupply_minting of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param oversupply_minting: The oversupply_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._oversupply_minting = oversupply_minting
 
     @property
     def nft_name(self):
-        """Gets the nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the nft_name of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         nft_name  # noqa: E501
 
-        :return: The nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The nft_name of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._nft_name
 
     @nft_name.setter
     def nft_name(self, nft_name):
-        """Sets the nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the nft_name of this ResponseWrapperGetNftInfoResult.
 
         nft_name  # noqa: E501
 
-        :param nft_name: The nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param nft_name: The nft_name of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._nft_name = nft_name
 
     @property
     def website_url(self):
-        """Gets the website_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the website_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the website url of the NFT. Return “null” means there is no website url or didn't find the website url.  # noqa: E501
 
-        :return: The website_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The website_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._website_url
 
     @website_url.setter
     def website_url(self, website_url):
-        """Sets the website_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the website_url of this ResponseWrapperGetNftInfoResult.
 
         It describes the website url of the NFT. Return “null” means there is no website url or didn't find the website url.  # noqa: E501
 
-        :param website_url: The website_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param website_url: The website_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._website_url = website_url
 
     @property
     def github_url(self):
-        """Gets the github_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the github_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the github url of the NFT. Return “null” means there is no github url or didn't find the github url.  # noqa: E501
 
-        :return: The github_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The github_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._github_url
 
     @github_url.setter
     def github_url(self, github_url):
-        """Sets the github_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the github_url of this ResponseWrapperGetNftInfoResult.
 
         It describes the github url of the NFT. Return “null” means there is no github url or didn't find the github url.  # noqa: E501
 
-        :param github_url: The github_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param github_url: The github_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._github_url = github_url
 
     @property
     def telegram_url(self):
-        """Gets the telegram_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the telegram_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the telegram url of the NFT. Return “null” means there is no telegram url or didn't find the telegram url.  # noqa: E501
 
-        :return: The telegram_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The telegram_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._telegram_url
 
     @telegram_url.setter
     def telegram_url(self, telegram_url):
-        """Sets the telegram_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the telegram_url of this ResponseWrapperGetNftInfoResult.
 
         It describes the telegram url of the NFT. Return “null” means there is no telegram url or didn't find the telegram url.  # noqa: E501
 
-        :param telegram_url: The telegram_url of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param telegram_url: The telegram_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._telegram_url = telegram_url
 
     @property
     def sales_24h(self):
-        """Gets the sales_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the sales_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the sales of the NFT in 24h.  # noqa: E501
 
-        :return: The sales_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The sales_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: float
         """
         return self._sales_24h
 
     @sales_24h.setter
     def sales_24h(self, sales_24h):
-        """Sets the sales_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the sales_24h of this ResponseWrapperGetNftInfoResult.
 
         It describes the sales of the NFT in 24h.  # noqa: E501
 
-        :param sales_24h: The sales_24h of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param sales_24h: The sales_24h of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: float
         """
 
         self._sales_24h = sales_24h
 
     @property
     def create_block_number(self):
-        """Gets the create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        """Gets the create_block_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
         It describes the number of blocks created for the NFT. Return “null” means that we didn't find the number of blocks created for the NFT.  # noqa: E501
 
-        :return: The create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :return: The create_block_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._create_block_number
 
     @create_block_number.setter
     def create_block_number(self, create_block_number):
-        """Sets the create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.
+        """Sets the create_block_number of this ResponseWrapperGetNftInfoResult.
 
         It describes the number of blocks created for the NFT. Return “null” means that we didn't find the number of blocks created for the NFT.  # noqa: E501
 
-        :param create_block_number: The create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult.  # noqa: E501
+        :param create_block_number: The create_block_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._create_block_number = create_block_number
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -1026,15 +1054,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult, dict):
+        if issubclass(ResponseWrapperGetNftInfoResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -1042,15 +1070,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResult):
+        if not isinstance(other, ResponseWrapperGetNftInfoResult):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_privileged_minting.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting(object):
+class ResponseWrapperGetNftInfoResultSelfDestruct(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,90 +36,90 @@
     attribute_map = {
         'owner_address': 'owner_address',
         'value': 'value',
         'owner_type': 'owner_type'
     }
 
     def __init__(self, owner_address=None, value=None, owner_type=None):  # noqa: E501
-        """ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperGetNftInfoResultSelfDestruct - a model defined in Swagger"""  # noqa: E501
         self._owner_address = None
         self._value = None
         self._owner_type = None
         self.discriminator = None
         if owner_address is not None:
             self.owner_address = owner_address
         if value is not None:
             self.value = value
         if owner_type is not None:
             self.owner_type = owner_type
 
     @property
     def owner_address(self):
-        """Gets the owner_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        """Gets the owner_address of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :return: The owner_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        :return: The owner_address of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
         :rtype: str
         """
         return self._owner_address
 
     @owner_address.setter
     def owner_address(self, owner_address):
-        """Sets the owner_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.
+        """Sets the owner_address of this ResponseWrapperGetNftInfoResultSelfDestruct.
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :param owner_address: The owner_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        :param owner_address: The owner_address of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
         :type: str
         """
 
         self._owner_address = owner_address
 
     @property
     def value(self):
-        """Gets the value of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        """Gets the value of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :return: The value of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        :return: The value of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
         :rtype: int
         """
         return self._value
 
     @value.setter
     def value(self, value):
-        """Sets the value of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.
+        """Sets the value of this ResponseWrapperGetNftInfoResultSelfDestruct.
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :param value: The value of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        :param value: The value of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
         :type: int
         """
 
         self._value = value
 
     @property
     def owner_type(self):
-        """Gets the owner_type of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        """Gets the owner_type of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :return: The owner_type of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        :return: The owner_type of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
         :rtype: str
         """
         return self._owner_type
 
     @owner_type.setter
     def owner_type(self, owner_type):
-        """Sets the owner_type of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.
+        """Sets the owner_type of this ResponseWrapperGetNftInfoResultSelfDestruct.
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :param owner_type: The owner_type of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting.  # noqa: E501
+        :param owner_type: The owner_type of this ResponseWrapperGetNftInfoResultSelfDestruct.  # noqa: E501
         :type: str
         """
 
         self._owner_type = owner_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting, dict):
+        if issubclass(ResponseWrapperGetNftInfoResultSelfDestruct, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultPrivilegedMinting):
+        if not isinstance(other, ResponseWrapperGetNftInfoResultSelfDestruct):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object59da6cfeb2f246e4936a6968cc97141b_result_same_nfts.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts(object):
+class ResponseWrapperGetNftInfoResultSameNfts(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -40,15 +40,15 @@
         'nft_name': 'nft_name',
         'nft_owner_number': 'nft_owner_number',
         'create_block_number': 'create_block_number',
         'nft_symbol': 'nft_symbol'
     }
 
     def __init__(self, nft_address=None, nft_name=None, nft_owner_number=None, create_block_number=None, nft_symbol=None):  # noqa: E501
-        """ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperGetNftInfoResultSameNfts - a model defined in Swagger"""  # noqa: E501
         self._nft_address = None
         self._nft_name = None
         self._nft_owner_number = None
         self._create_block_number = None
         self._nft_symbol = None
         self.discriminator = None
         if nft_address is not None:
@@ -60,122 +60,122 @@
         if create_block_number is not None:
             self.create_block_number = create_block_number
         if nft_symbol is not None:
             self.nft_symbol = nft_symbol
 
     @property
     def nft_address(self):
-        """Gets the nft_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        """Gets the nft_address of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
 
         It describes the address of the NFTs;  # noqa: E501
 
-        :return: The nft_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :return: The nft_address of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :rtype: str
         """
         return self._nft_address
 
     @nft_address.setter
     def nft_address(self, nft_address):
-        """Sets the nft_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.
+        """Sets the nft_address of this ResponseWrapperGetNftInfoResultSameNfts.
 
         It describes the address of the NFTs;  # noqa: E501
 
-        :param nft_address: The nft_address of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :param nft_address: The nft_address of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :type: str
         """
 
         self._nft_address = nft_address
 
     @property
     def nft_name(self):
-        """Gets the nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        """Gets the nft_name of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
 
         It describes the name of the NFT;  # noqa: E501
 
-        :return: The nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :return: The nft_name of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :rtype: str
         """
         return self._nft_name
 
     @nft_name.setter
     def nft_name(self, nft_name):
-        """Sets the nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.
+        """Sets the nft_name of this ResponseWrapperGetNftInfoResultSameNfts.
 
         It describes the name of the NFT;  # noqa: E501
 
-        :param nft_name: The nft_name of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :param nft_name: The nft_name of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :type: str
         """
 
         self._nft_name = nft_name
 
     @property
     def nft_owner_number(self):
-        """Gets the nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        """Gets the nft_owner_number of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
 
         It describes the holders of the NFT;  # noqa: E501
 
-        :return: The nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :return: The nft_owner_number of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :rtype: int
         """
         return self._nft_owner_number
 
     @nft_owner_number.setter
     def nft_owner_number(self, nft_owner_number):
-        """Sets the nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.
+        """Sets the nft_owner_number of this ResponseWrapperGetNftInfoResultSameNfts.
 
         It describes the holders of the NFT;  # noqa: E501
 
-        :param nft_owner_number: The nft_owner_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :param nft_owner_number: The nft_owner_number of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :type: int
         """
 
         self._nft_owner_number = nft_owner_number
 
     @property
     def create_block_number(self):
-        """Gets the create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        """Gets the create_block_number of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
 
         describes the number of blocks created for the NFT. Return \"null\" means no NFTs with duplicate name and symbol.  # noqa: E501
 
-        :return: The create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :return: The create_block_number of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :rtype: int
         """
         return self._create_block_number
 
     @create_block_number.setter
     def create_block_number(self, create_block_number):
-        """Sets the create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.
+        """Sets the create_block_number of this ResponseWrapperGetNftInfoResultSameNfts.
 
         describes the number of blocks created for the NFT. Return \"null\" means no NFTs with duplicate name and symbol.  # noqa: E501
 
-        :param create_block_number: The create_block_number of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :param create_block_number: The create_block_number of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :type: int
         """
 
         self._create_block_number = create_block_number
 
     @property
     def nft_symbol(self):
-        """Gets the nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        """Gets the nft_symbol of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
 
         It describes the symbol of the NFT;  # noqa: E501
 
-        :return: The nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :return: The nft_symbol of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :rtype: str
         """
         return self._nft_symbol
 
     @nft_symbol.setter
     def nft_symbol(self, nft_symbol):
-        """Sets the nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.
+        """Sets the nft_symbol of this ResponseWrapperGetNftInfoResultSameNfts.
 
         It describes the symbol of the NFT;  # noqa: E501
 
-        :param nft_symbol: The nft_symbol of this ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts.  # noqa: E501
+        :param nft_symbol: The nft_symbol of this ResponseWrapperGetNftInfoResultSameNfts.  # noqa: E501
         :type: str
         """
 
         self._nft_symbol = nft_symbol
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -194,15 +194,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts, dict):
+        if issubclass(ResponseWrapperGetNftInfoResultSameNfts, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -210,15 +210,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject59da6cfeb2f246e4936a6968cc97141bResultSameNfts):
+        if not isinstance(other, ResponseWrapperGetNftInfoResultSameNfts):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_token_security.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c(object):
+class ResponseWrapperTokenSecurity(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResult'
+        'result': 'dict(str, ResponseWrapperTokenSecurityResult)'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperTokenSecurity - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        """Gets the code of this ResponseWrapperTokenSecurity.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        :return: The code of this ResponseWrapperTokenSecurity.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.
+        """Sets the code of this ResponseWrapperTokenSecurity.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        :param code: The code of this ResponseWrapperTokenSecurity.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        """Gets the message of this ResponseWrapperTokenSecurity.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        :return: The message of this ResponseWrapperTokenSecurity.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.
+        """Sets the message of this ResponseWrapperTokenSecurity.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        :param message: The message of this ResponseWrapperTokenSecurity.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
+        """Gets the result of this ResponseWrapperTokenSecurity.  # noqa: E501
 
+        Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
-        :rtype: ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResult
+        :return: The result of this ResponseWrapperTokenSecurity.  # noqa: E501
+        :rtype: dict(str, ResponseWrapperTokenSecurityResult)
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.
+        """Sets the result of this ResponseWrapperTokenSecurity.
 
+        Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c.  # noqa: E501
-        :type: ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResult
+        :param result: The result of this ResponseWrapperTokenSecurity.  # noqa: E501
+        :type: dict(str, ResponseWrapperTokenSecurityResult)
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -136,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c, dict):
+        if issubclass(ResponseWrapperTokenSecurity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6c):
+        if not isinstance(other, ResponseWrapperTokenSecurity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_privileged_burn.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn(object):
+class ResponseWrapperGetNftInfoResultPrivilegedBurn(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,90 +36,90 @@
     attribute_map = {
         'owner_address': 'owner_address',
         'value': 'value',
         'owner_type': 'owner_type'
     }
 
     def __init__(self, owner_address=None, value=None, owner_type=None):  # noqa: E501
-        """ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperGetNftInfoResultPrivilegedBurn - a model defined in Swagger"""  # noqa: E501
         self._owner_address = None
         self._value = None
         self._owner_type = None
         self.discriminator = None
         if owner_address is not None:
             self.owner_address = owner_address
         if value is not None:
             self.value = value
         if owner_type is not None:
             self.owner_type = owner_type
 
     @property
     def owner_address(self):
-        """Gets the owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        """Gets the owner_address of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :return: The owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        :return: The owner_address of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
         :rtype: str
         """
         return self._owner_address
 
     @owner_address.setter
     def owner_address(self, owner_address):
-        """Sets the owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.
+        """Sets the owner_address of this ResponseWrapperGetNftInfoResultPrivilegedBurn.
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :param owner_address: The owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        :param owner_address: The owner_address of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
         :type: str
         """
 
         self._owner_address = owner_address
 
     @property
     def value(self):
-        """Gets the value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        """Gets the value of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :return: The value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        :return: The value of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
         :rtype: int
         """
         return self._value
 
     @value.setter
     def value(self, value):
-        """Sets the value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.
+        """Sets the value of this ResponseWrapperGetNftInfoResultPrivilegedBurn.
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :param value: The value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        :param value: The value of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
         :type: int
         """
 
         self._value = value
 
     @property
     def owner_type(self):
-        """Gets the owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        """Gets the owner_type of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :return: The owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        :return: The owner_type of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
         :rtype: str
         """
         return self._owner_type
 
     @owner_type.setter
     def owner_type(self, owner_type):
-        """Sets the owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.
+        """Sets the owner_type of this ResponseWrapperGetNftInfoResultPrivilegedBurn.
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :param owner_type: The owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn.  # noqa: E501
+        :param owner_type: The owner_type of this ResponseWrapperGetNftInfoResultPrivilegedBurn.  # noqa: E501
         :type: str
         """
 
         self._owner_type = owner_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn, dict):
+        if issubclass(ResponseWrapperGetNftInfoResultPrivilegedBurn, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedBurn):
+        if not isinstance(other, ResponseWrapperGetNftInfoResultPrivilegedBurn):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_privileged_minting.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting(object):
+class ResponseWrapperGetNftInfoResultPrivilegedMinting(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,90 +36,90 @@
     attribute_map = {
         'owner_address': 'owner_address',
         'value': 'value',
         'owner_type': 'owner_type'
     }
 
     def __init__(self, owner_address=None, value=None, owner_type=None):  # noqa: E501
-        """ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperGetNftInfoResultPrivilegedMinting - a model defined in Swagger"""  # noqa: E501
         self._owner_address = None
         self._value = None
         self._owner_type = None
         self.discriminator = None
         if owner_address is not None:
             self.owner_address = owner_address
         if value is not None:
             self.value = value
         if owner_type is not None:
             self.owner_type = owner_type
 
     @property
     def owner_address(self):
-        """Gets the owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        """Gets the owner_address of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :return: The owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        :return: The owner_address of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
         :rtype: str
         """
         return self._owner_address
 
     @owner_address.setter
     def owner_address(self, owner_address):
-        """Sets the owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.
+        """Sets the owner_address of this ResponseWrapperGetNftInfoResultPrivilegedMinting.
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :param owner_address: The owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        :param owner_address: The owner_address of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
         :type: str
         """
 
         self._owner_address = owner_address
 
     @property
     def value(self):
-        """Gets the value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        """Gets the value of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :return: The value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        :return: The value of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
         :rtype: int
         """
         return self._value
 
     @value.setter
     def value(self, value):
-        """Sets the value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.
+        """Sets the value of this ResponseWrapperGetNftInfoResultPrivilegedMinting.
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :param value: The value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        :param value: The value of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
         :type: int
         """
 
         self._value = value
 
     @property
     def owner_type(self):
-        """Gets the owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        """Gets the owner_type of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :return: The owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        :return: The owner_type of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
         :rtype: str
         """
         return self._owner_type
 
     @owner_type.setter
     def owner_type(self, owner_type):
-        """Sets the owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.
+        """Sets the owner_type of this ResponseWrapperGetNftInfoResultPrivilegedMinting.
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :param owner_type: The owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting.  # noqa: E501
+        :param owner_type: The owner_type of this ResponseWrapperGetNftInfoResultPrivilegedMinting.  # noqa: E501
         :type: str
         """
 
         self._owner_type = owner_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting, dict):
+        if issubclass(ResponseWrapperGetNftInfoResultPrivilegedMinting, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultPrivilegedMinting):
+        if not isinstance(other, ResponseWrapperGetNftInfoResultPrivilegedMinting):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_json_object5c459c547a184b1880671fad2eb60d6c_result_self_destruct.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct(object):
+class ResponseWrapperGetNftInfoResultTransferWithoutApproval(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,90 +36,90 @@
     attribute_map = {
         'owner_address': 'owner_address',
         'value': 'value',
         'owner_type': 'owner_type'
     }
 
     def __init__(self, owner_address=None, value=None, owner_type=None):  # noqa: E501
-        """ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperGetNftInfoResultTransferWithoutApproval - a model defined in Swagger"""  # noqa: E501
         self._owner_address = None
         self._value = None
         self._owner_type = None
         self.discriminator = None
         if owner_address is not None:
             self.owner_address = owner_address
         if value is not None:
             self.value = value
         if owner_type is not None:
             self.owner_type = owner_type
 
     @property
     def owner_address(self):
-        """Gets the owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        """Gets the owner_address of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :return: The owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        :return: The owner_address of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
         :rtype: str
         """
         return self._owner_address
 
     @owner_address.setter
     def owner_address(self, owner_address):
-        """Sets the owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.
+        """Sets the owner_address of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.
 
         Owner_address describes the owner address.  null: the owner address cannot be fetched.  # noqa: E501
 
-        :param owner_address: The owner_address of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        :param owner_address: The owner_address of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
         :type: str
         """
 
         self._owner_address = owner_address
 
     @property
     def value(self):
-        """Gets the value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        """Gets the value of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :return: The value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        :return: The value of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
         :rtype: int
         """
         return self._value
 
     @value.setter
     def value(self, value):
-        """Sets the value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.
+        """Sets the value of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.
 
         The \"value\" describes the status of the risk. null: the contract is not open source or there is a proxy, it is not possible to detect whether the risk exists. -1: the risk is detected but the ownership give up. If the detection of a code vulnerability, it can also be considered risk-free.  0: the risk is not detected.  1: the risk is detected, and the owner address is a common address (EOA), then it can be said that there is a clear risk.  2: The risk is detected, but the owner address is a contract address, the risk is not significant.  3: The risk is detected, but the owner address is not detectable / or an array.   # noqa: E501
 
-        :param value: The value of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        :param value: The value of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
         :type: int
         """
 
         self._value = value
 
     @property
     def owner_type(self):
-        """Gets the owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        """Gets the owner_type of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :return: The owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        :return: The owner_type of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
         :rtype: str
         """
         return self._owner_type
 
     @owner_type.setter
     def owner_type(self, owner_type):
-        """Sets the owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.
+        """Sets the owner_type of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.
 
         \"blackhole\" : the owner is a blackhole address. \"contract\" : the owner is a contract. \"eoa\" : the owner is a common address (eoa). \"multi-address\": the owner is an array/list. null: the address is not detected.  # noqa: E501
 
-        :param owner_type: The owner_type of this ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct.  # noqa: E501
+        :param owner_type: The owner_type of this ResponseWrapperGetNftInfoResultTransferWithoutApproval.  # noqa: E501
         :type: str
         """
 
         self._owner_type = owner_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct, dict):
+        if issubclass(ResponseWrapperGetNftInfoResultTransferWithoutApproval, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperJSONObject5c459c547a184b1880671fad2eb60d6cResultSelfDestruct):
+        if not isinstance(other, ResponseWrapperGetNftInfoResultTransferWithoutApproval):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_approve_nft_list_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_list_approve_nft_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_list_get_chains_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperListApproveTokenOutListResponse(object):
+class ResponseWrapperListGetChainsList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'list[ApproveTokenOutListResponse]'
+        'result': 'list[ResponseWrapperListGetChainsListResult]'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperListApproveTokenOutListResponse - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperListGetChainsList - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        """Gets the code of this ResponseWrapperListGetChainsList.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        :return: The code of this ResponseWrapperListGetChainsList.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperListApproveTokenOutListResponse.
+        """Sets the code of this ResponseWrapperListGetChainsList.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        :param code: The code of this ResponseWrapperListGetChainsList.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        """Gets the message of this ResponseWrapperListGetChainsList.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        :return: The message of this ResponseWrapperListGetChainsList.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperListApproveTokenOutListResponse.
+        """Sets the message of this ResponseWrapperListGetChainsList.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        :param message: The message of this ResponseWrapperListGetChainsList.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
+        """Gets the result of this ResponseWrapperListGetChainsList.  # noqa: E501
 
         Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
-        :rtype: list[ApproveTokenOutListResponse]
+        :return: The result of this ResponseWrapperListGetChainsList.  # noqa: E501
+        :rtype: list[ResponseWrapperListGetChainsListResult]
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperListApproveTokenOutListResponse.
+        """Sets the result of this ResponseWrapperListGetChainsList.
 
         Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
-        :type: list[ApproveTokenOutListResponse]
+        :param result: The result of this ResponseWrapperListGetChainsList.  # noqa: E501
+        :type: list[ResponseWrapperListGetChainsListResult]
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperListApproveTokenOutListResponse, dict):
+        if issubclass(ResponseWrapperListGetChainsList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperListApproveTokenOutListResponse):
+        if not isinstance(other, ResponseWrapperListGetChainsList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_list_json_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object4e98b9e2_fbdb43329976_a30066e02b73.py` & `goplus-0.1.1/swagger_client/models/response_wrapperobject.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73(object):
+class ResponseWrapperobject(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'list[ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result]'
+        'result': 'object'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73 - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperobject - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        """Gets the code of this ResponseWrapperobject.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        :return: The code of this ResponseWrapperobject.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.
+        """Sets the code of this ResponseWrapperobject.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        :param code: The code of this ResponseWrapperobject.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        """Gets the message of this ResponseWrapperobject.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        :return: The message of this ResponseWrapperobject.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.
+        """Sets the message of this ResponseWrapperobject.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        :param message: The message of this ResponseWrapperobject.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
+        """Gets the result of this ResponseWrapperobject.  # noqa: E501
 
         Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
-        :rtype: list[ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result]
+        :return: The result of this ResponseWrapperobject.  # noqa: E501
+        :rtype: object
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.
+        """Sets the result of this ResponseWrapperobject.
 
         Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73.  # noqa: E501
-        :type: list[ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result]
+        :param result: The result of this ResponseWrapperobject.  # noqa: E501
+        :type: object
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73, dict):
+        if issubclass(ResponseWrapperobject, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperListJSONObject4e98b9e2Fbdb43329976A30066e02b73):
+        if not isinstance(other, ResponseWrapperobject):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object4e98b9e2fbdb43329976a30066e02b73_result.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_token_security_dex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,127 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result(object):
+class ResponseWrapperTokenSecurityDex(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'name': 'str',
-        'id': 'str'
+        'liquidity': 'str',
+        'pair': 'str'
     }
 
     attribute_map = {
         'name': 'name',
-        'id': 'id'
+        'liquidity': 'liquidity',
+        'pair': 'pair'
     }
 
-    def __init__(self, name=None, id=None):  # noqa: E501
-        """ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, name=None, liquidity=None, pair=None):  # noqa: E501
+        """ResponseWrapperTokenSecurityDex - a model defined in Swagger"""  # noqa: E501
         self._name = None
-        self._id = None
+        self._liquidity = None
+        self._pair = None
         self.discriminator = None
         if name is not None:
             self.name = name
-        if id is not None:
-            self.id = id
+        if liquidity is not None:
+            self.liquidity = liquidity
+        if pair is not None:
+            self.pair = pair
 
     @property
     def name(self):
-        """Gets the name of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.  # noqa: E501
+        """Gets the name of this ResponseWrapperTokenSecurityDex.  # noqa: E501
 
-        chain name  # noqa: E501
 
-        :return: The name of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.  # noqa: E501
+        :return: The name of this ResponseWrapperTokenSecurityDex.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.
+        """Sets the name of this ResponseWrapperTokenSecurityDex.
 
-        chain name  # noqa: E501
 
-        :param name: The name of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.  # noqa: E501
+        :param name: The name of this ResponseWrapperTokenSecurityDex.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
-    def id(self):
-        """Gets the id of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.  # noqa: E501
+    def liquidity(self):
+        """Gets the liquidity of this ResponseWrapperTokenSecurityDex.  # noqa: E501
 
-        chain id  # noqa: E501
+        Liquidity is converted to USDT denomination.  # noqa: E501
 
-        :return: The id of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.  # noqa: E501
+        :return: The liquidity of this ResponseWrapperTokenSecurityDex.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._liquidity
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.
+    @liquidity.setter
+    def liquidity(self, liquidity):
+        """Sets the liquidity of this ResponseWrapperTokenSecurityDex.
 
-        chain id  # noqa: E501
+        Liquidity is converted to USDT denomination.  # noqa: E501
 
-        :param id: The id of this ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result.  # noqa: E501
+        :param liquidity: The liquidity of this ResponseWrapperTokenSecurityDex.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._liquidity = liquidity
+
+    @property
+    def pair(self):
+        """Gets the pair of this ResponseWrapperTokenSecurityDex.  # noqa: E501
+
+         It only counts when the token has a marketing pair with mainstream   # noqa: E501
+
+        :return: The pair of this ResponseWrapperTokenSecurityDex.  # noqa: E501
+        :rtype: str
+        """
+        return self._pair
+
+    @pair.setter
+    def pair(self, pair):
+        """Sets the pair of this ResponseWrapperTokenSecurityDex.
+
+         It only counts when the token has a marketing pair with mainstream   # noqa: E501
+
+        :param pair: The pair of this ResponseWrapperTokenSecurityDex.  # noqa: E501
+        :type: str
+        """
+
+        self._pair = pair
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result, dict):
+        if issubclass(ResponseWrapperTokenSecurityDex, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperListJSONObject4e98b9e2fbdb43329976a30066e02b73Result):
+        if not isinstance(other, ResponseWrapperTokenSecurityDex):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object9524a1c652c545bf_b6c6898bfc3e93f3.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_phishing_site.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,124 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3(object):
+class ResponseWrapperPhishingSite(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'list[ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result]'
+        'result': 'ResponseWrapperPhishingSiteResult'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3 - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperPhishingSite - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        """Gets the code of this ResponseWrapperPhishingSite.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        :return: The code of this ResponseWrapperPhishingSite.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.
+        """Sets the code of this ResponseWrapperPhishingSite.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        :param code: The code of this ResponseWrapperPhishingSite.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        """Gets the message of this ResponseWrapperPhishingSite.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        :return: The message of this ResponseWrapperPhishingSite.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.
+        """Sets the message of this ResponseWrapperPhishingSite.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        :param message: The message of this ResponseWrapperPhishingSite.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
+        """Gets the result of this ResponseWrapperPhishingSite.  # noqa: E501
 
-        Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
-        :rtype: list[ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result]
+        :return: The result of this ResponseWrapperPhishingSite.  # noqa: E501
+        :rtype: ResponseWrapperPhishingSiteResult
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.
+        """Sets the result of this ResponseWrapperPhishingSite.
 
-        Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3.  # noqa: E501
-        :type: list[ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result]
+        :param result: The result of this ResponseWrapperPhishingSite.  # noqa: E501
+        :type: ResponseWrapperPhishingSiteResult
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -138,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3, dict):
+        if issubclass(ResponseWrapperPhishingSite, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperListJSONObject9524a1c652c545bfB6c6898bfc3e93f3):
+        if not isinstance(other, ResponseWrapperPhishingSite):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_list_json_object9524a1c652c545bfb6c6898bfc3e93f3_result.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_ta_token_security_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,127 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result(object):
+class ResponseWrapperTaTokenSecurityResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'name': 'str',
-        'id': 'str'
+        'code': 'int',
+        'message': 'str',
+        'result': 'TaTokenSecurityResponse'
     }
 
     attribute_map = {
-        'name': 'name',
-        'id': 'id'
+        'code': 'code',
+        'message': 'message',
+        'result': 'result'
     }
 
-    def __init__(self, name=None, id=None):  # noqa: E501
-        """ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result - a model defined in Swagger"""  # noqa: E501
-        self._name = None
-        self._id = None
+    def __init__(self, code=None, message=None, result=None):  # noqa: E501
+        """ResponseWrapperTaTokenSecurityResponse - a model defined in Swagger"""  # noqa: E501
+        self._code = None
+        self._message = None
+        self._result = None
         self.discriminator = None
-        if name is not None:
-            self.name = name
-        if id is not None:
-            self.id = id
+        if code is not None:
+            self.code = code
+        if message is not None:
+            self.message = message
+        if result is not None:
+            self.result = result
 
     @property
-    def name(self):
-        """Gets the name of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.  # noqa: E501
+    def code(self):
+        """Gets the code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
 
-        chain name  # noqa: E501
+        Code 1：Success  # noqa: E501
 
-        :return: The name of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.  # noqa: E501
-        :rtype: str
+        :return: The code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :rtype: int
         """
-        return self._name
+        return self._code
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.
+    @code.setter
+    def code(self, code):
+        """Sets the code of this ResponseWrapperTaTokenSecurityResponse.
 
-        chain name  # noqa: E501
+        Code 1：Success  # noqa: E501
 
-        :param name: The name of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.  # noqa: E501
-        :type: str
+        :param code: The code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :type: int
         """
 
-        self._name = name
+        self._code = code
 
     @property
-    def id(self):
-        """Gets the id of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.  # noqa: E501
+    def message(self):
+        """Gets the message of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
 
-        chain id  # noqa: E501
+        Response message  # noqa: E501
 
-        :return: The id of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.  # noqa: E501
+        :return: The message of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._message
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.
+    @message.setter
+    def message(self, message):
+        """Sets the message of this ResponseWrapperTaTokenSecurityResponse.
 
-        chain id  # noqa: E501
+        Response message  # noqa: E501
 
-        :param id: The id of this ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result.  # noqa: E501
+        :param message: The message of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._message = message
+
+    @property
+    def result(self):
+        """Gets the result of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+
+
+        :return: The result of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :rtype: TaTokenSecurityResponse
+        """
+        return self._result
+
+    @result.setter
+    def result(self, result):
+        """Sets the result of this ResponseWrapperTaTokenSecurityResponse.
+
+
+        :param result: The result of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :type: TaTokenSecurityResponse
+        """
+
+        self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result, dict):
+        if issubclass(ResponseWrapperTaTokenSecurityResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperListJSONObject9524a1c652c545bfb6c6898bfc3e93f3Result):
+        if not isinstance(other, ResponseWrapperTaTokenSecurityResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstring.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_map_string_string.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperMapstringstring(object):
+class ResponseWrapperMapStringString(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,90 +36,90 @@
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperMapstringstring - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperMapStringString - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperMapstringstring.  # noqa: E501
+        """Gets the code of this ResponseWrapperMapStringString.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperMapstringstring.  # noqa: E501
+        :return: The code of this ResponseWrapperMapStringString.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperMapstringstring.
+        """Sets the code of this ResponseWrapperMapStringString.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperMapstringstring.  # noqa: E501
+        :param code: The code of this ResponseWrapperMapStringString.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperMapstringstring.  # noqa: E501
+        """Gets the message of this ResponseWrapperMapStringString.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperMapstringstring.  # noqa: E501
+        :return: The message of this ResponseWrapperMapStringString.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperMapstringstring.
+        """Sets the message of this ResponseWrapperMapStringString.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperMapstringstring.  # noqa: E501
+        :param message: The message of this ResponseWrapperMapStringString.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperMapstringstring.  # noqa: E501
+        """Gets the result of this ResponseWrapperMapStringString.  # noqa: E501
 
         Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperMapstringstring.  # noqa: E501
+        :return: The result of this ResponseWrapperMapStringString.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperMapstringstring.
+        """Sets the result of this ResponseWrapperMapStringString.
 
         Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperMapstringstring.  # noqa: E501
+        :param result: The result of this ResponseWrapperMapStringString.  # noqa: E501
         :type: dict(str, str)
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperMapstringstring, dict):
+        if issubclass(ResponseWrapperMapStringString, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperMapstringstring):
+        if not isinstance(other, ResponseWrapperMapStringString):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_mapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8_result.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_phishing_site_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result(object):
+class ResponseWrapperPhishingSiteResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,62 +34,62 @@
 
     attribute_map = {
         'website_contract_security': 'website_contract_security',
         'phishing_site': 'phishing_site'
     }
 
     def __init__(self, website_contract_security=None, phishing_site=None):  # noqa: E501
-        """ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperPhishingSiteResult - a model defined in Swagger"""  # noqa: E501
         self._website_contract_security = None
         self._phishing_site = None
         self.discriminator = None
         if website_contract_security is not None:
             self.website_contract_security = website_contract_security
         if phishing_site is not None:
             self.phishing_site = phishing_site
 
     @property
     def website_contract_security(self):
-        """Gets the website_contract_security of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.  # noqa: E501
+        """Gets the website_contract_security of this ResponseWrapperPhishingSiteResult.  # noqa: E501
 
 
-        :return: The website_contract_security of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.  # noqa: E501
+        :return: The website_contract_security of this ResponseWrapperPhishingSiteResult.  # noqa: E501
         :rtype: list[str]
         """
         return self._website_contract_security
 
     @website_contract_security.setter
     def website_contract_security(self, website_contract_security):
-        """Sets the website_contract_security of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.
+        """Sets the website_contract_security of this ResponseWrapperPhishingSiteResult.
 
 
-        :param website_contract_security: The website_contract_security of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.  # noqa: E501
+        :param website_contract_security: The website_contract_security of this ResponseWrapperPhishingSiteResult.  # noqa: E501
         :type: list[str]
         """
 
         self._website_contract_security = website_contract_security
 
     @property
     def phishing_site(self):
-        """Gets the phishing_site of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.  # noqa: E501
+        """Gets the phishing_site of this ResponseWrapperPhishingSiteResult.  # noqa: E501
 
         It means whether the website is a phishing site. \"1\" means true; \"0\" means that we have not found malicious behavior of this website.  # noqa: E501
 
-        :return: The phishing_site of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.  # noqa: E501
+        :return: The phishing_site of this ResponseWrapperPhishingSiteResult.  # noqa: E501
         :rtype: int
         """
         return self._phishing_site
 
     @phishing_site.setter
     def phishing_site(self, phishing_site):
-        """Sets the phishing_site of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.
+        """Sets the phishing_site of this ResponseWrapperPhishingSiteResult.
 
         It means whether the website is a phishing site. \"1\" means true; \"0\" means that we have not found malicious behavior of this website.  # noqa: E501
 
-        :param phishing_site: The phishing_site of this ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result.  # noqa: E501
+        :param phishing_site: The phishing_site of this ResponseWrapperPhishingSiteResult.  # noqa: E501
         :type: int
         """
 
         self._phishing_site = phishing_site
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result, dict):
+        if issubclass(ResponseWrapperPhishingSiteResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperMapstringstring2a740de0be5a4eb3b6e4a2cf0a2d8bf8Result):
+        if not isinstance(other, ResponseWrapperPhishingSiteResult):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_parse_abi_data_response.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_parse_abi_data_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response.py` & `goplus-0.1.1/swagger_client/models/get_defi_info_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperTaTokenSecurityResponse(object):
+class GetDefiInfoResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'TaTokenSecurityResponse'
+        'result': 'GetDefiInfoResponseResult'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperTaTokenSecurityResponse - a model defined in Swagger"""  # noqa: E501
+        """GetDefiInfoResponse - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        """Gets the code of this GetDefiInfoResponse.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :return: The code of this GetDefiInfoResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperTaTokenSecurityResponse.
+        """Sets the code of this GetDefiInfoResponse.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :param code: The code of this GetDefiInfoResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        """Gets the message of this GetDefiInfoResponse.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :return: The message of this GetDefiInfoResponse.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperTaTokenSecurityResponse.
+        """Sets the message of this GetDefiInfoResponse.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        :param message: The message of this GetDefiInfoResponse.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
+        """Gets the result of this GetDefiInfoResponse.  # noqa: E501
 
 
-        :return: The result of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
-        :rtype: TaTokenSecurityResponse
+        :return: The result of this GetDefiInfoResponse.  # noqa: E501
+        :rtype: GetDefiInfoResponseResult
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperTaTokenSecurityResponse.
+        """Sets the result of this GetDefiInfoResponse.
 
 
-        :param result: The result of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
-        :type: TaTokenSecurityResponse
+        :param result: The result of this GetDefiInfoResponse.  # noqa: E501
+        :type: GetDefiInfoResponseResult
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -136,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperTaTokenSecurityResponse, dict):
+        if issubclass(GetDefiInfoResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperTaTokenSecurityResponse):
+        if not isinstance(other, GetDefiInfoResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_lp_holders.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_token_security_lp_holders.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders(object):
+class ResponseWrapperTokenSecurityLpHolders(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -44,15 +44,15 @@
         'balance': 'balance',
         'locked_detail': 'locked_detail',
         'tag': 'tag',
         'percent': 'percent'
     }
 
     def __init__(self, is_locked=None, is_contract=None, address=None, balance=None, locked_detail=None, tag=None, percent=None):  # noqa: E501
-        """ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperTokenSecurityLpHolders - a model defined in Swagger"""  # noqa: E501
         self._is_locked = None
         self._is_contract = None
         self._address = None
         self._balance = None
         self._locked_detail = None
         self._tag = None
         self._percent = None
@@ -70,168 +70,168 @@
         if tag is not None:
             self.tag = tag
         if percent is not None:
             self.percent = percent
 
     @property
     def is_locked(self):
-        """Gets the is_locked of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the is_locked of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It describes whether the tokens owned by the holder are locked \"1\" means true; \"0\" means false;  (3) “tag” describes the address's public tag. Example:Burn (Notice:About \"locked\": We only support the token lock addresses or black hole addresses that we have included. )  # noqa: E501
 
-        :return: The is_locked of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The is_locked of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: int
         """
         return self._is_locked
 
     @is_locked.setter
     def is_locked(self, is_locked):
-        """Sets the is_locked of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the is_locked of this ResponseWrapperTokenSecurityLpHolders.
 
         It describes whether the tokens owned by the holder are locked \"1\" means true; \"0\" means false;  (3) “tag” describes the address's public tag. Example:Burn (Notice:About \"locked\": We only support the token lock addresses or black hole addresses that we have included. )  # noqa: E501
 
-        :param is_locked: The is_locked of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param is_locked: The is_locked of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: int
         """
 
         self._is_locked = is_locked
 
     @property
     def is_contract(self):
-        """Gets the is_contract of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the is_contract of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It describes whether the holder is a contract \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The is_contract of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The is_contract of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: int
         """
         return self._is_contract
 
     @is_contract.setter
     def is_contract(self, is_contract):
-        """Sets the is_contract of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the is_contract of this ResponseWrapperTokenSecurityLpHolders.
 
         It describes whether the holder is a contract \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param is_contract: The is_contract of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param is_contract: The is_contract of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: int
         """
 
         self._is_contract = is_contract
 
     @property
     def address(self):
-        """Gets the address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the address of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It describes the holder address;   # noqa: E501
 
-        :return: The address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The address of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: str
         """
         return self._address
 
     @address.setter
     def address(self, address):
-        """Sets the address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the address of this ResponseWrapperTokenSecurityLpHolders.
 
         It describes the holder address;   # noqa: E501
 
-        :param address: The address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param address: The address of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: str
         """
 
         self._address = address
 
     @property
     def balance(self):
-        """Gets the balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the balance of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It describes the balance of the holder.   # noqa: E501
 
-        :return: The balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The balance of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: str
         """
         return self._balance
 
     @balance.setter
     def balance(self, balance):
-        """Sets the balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the balance of this ResponseWrapperTokenSecurityLpHolders.
 
         It describes the balance of the holder.   # noqa: E501
 
-        :param balance: The balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param balance: The balance of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: str
         """
 
         self._balance = balance
 
     @property
     def locked_detail(self):
-        """Gets the locked_detail of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the locked_detail of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It is an array, decribes lock position info of this holder, only shows when \"locked\": 1. This Array may contain multiple objects for multiple locking info. In every objetc, \"amount\" describes the number of token locked, \"end_time\" describes when the token will be unlocked, \"opt_time\" describes when the token was locked.(Notice:When \"locked\":0, or lock address is a black hole address,  \"locked_detail\" will be no return.)  # noqa: E501
 
-        :return: The locked_detail of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The locked_detail of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: list[str]
         """
         return self._locked_detail
 
     @locked_detail.setter
     def locked_detail(self, locked_detail):
-        """Sets the locked_detail of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the locked_detail of this ResponseWrapperTokenSecurityLpHolders.
 
         It is an array, decribes lock position info of this holder, only shows when \"locked\": 1. This Array may contain multiple objects for multiple locking info. In every objetc, \"amount\" describes the number of token locked, \"end_time\" describes when the token will be unlocked, \"opt_time\" describes when the token was locked.(Notice:When \"locked\":0, or lock address is a black hole address,  \"locked_detail\" will be no return.)  # noqa: E501
 
-        :param locked_detail: The locked_detail of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param locked_detail: The locked_detail of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: list[str]
         """
 
         self._locked_detail = locked_detail
 
     @property
     def tag(self):
-        """Gets the tag of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the tag of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It describes the address's public tag. Example:Burn Address/Deployer;   # noqa: E501
 
-        :return: The tag of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The tag of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: str
         """
         return self._tag
 
     @tag.setter
     def tag(self, tag):
-        """Sets the tag of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the tag of this ResponseWrapperTokenSecurityLpHolders.
 
         It describes the address's public tag. Example:Burn Address/Deployer;   # noqa: E501
 
-        :param tag: The tag of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param tag: The tag of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: str
         """
 
         self._tag = tag
 
     @property
     def percent(self):
-        """Gets the percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        """Gets the percent of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
         It  describes the percentage of tokens held by this holder (Notice:About \"percent\": 1 means 100% here.)  # noqa: E501
 
-        :return: The percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :return: The percent of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: str
         """
         return self._percent
 
     @percent.setter
     def percent(self, percent):
-        """Sets the percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.
+        """Sets the percent of this ResponseWrapperTokenSecurityLpHolders.
 
         It  describes the percentage of tokens held by this holder (Notice:About \"percent\": 1 means 100% here.)  # noqa: E501
 
-        :param percent: The percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders.  # noqa: E501
+        :param percent: The percent of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: str
         """
 
         self._percent = percent
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -250,15 +250,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders, dict):
+        if issubclass(ResponseWrapperTokenSecurityLpHolders, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -266,15 +266,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders):
+        if not isinstance(other, ResponseWrapperTokenSecurityLpHolders):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapper_ta_token_security_response205696bcfb354bc5ab26ddc7cd495fe2_result.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_token_security_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result(object):
+class ResponseWrapperTokenSecurityResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'note': 'str',
         'lp_total_supply': 'str',
-        'lp_holders': 'list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders]',
+        'lp_holders': 'list[ResponseWrapperTokenSecurityLpHolders]',
         'is_airdrop_scam': 'str',
         'other_potential_risks': 'str',
         'transfer_pausable': 'str',
         'trading_cooldown': 'str',
         'hidden_owner': 'str',
         'selfdestruct': 'str',
         'owner_percent': 'str',
         'is_whitelisted': 'str',
         'holder_count': 'str',
         'trust_list': 'str',
         'is_honeypot': 'str',
-        'holders': 'list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders]',
-        'dex': 'list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Dex]',
+        'holders': 'list[ResponseWrapperTokenSecurityLpHolders]',
+        'dex': 'list[ResponseWrapperTokenSecurityDex]',
         'is_open_source': 'str',
         'sell_tax': 'str',
         'token_name': 'str',
         'creator_address': 'str',
         'creator_percent': 'str',
         'is_proxy': 'str',
         'creator_balance': 'str',
@@ -114,15 +114,15 @@
         'owner_change_balance': 'owner_change_balance',
         'cannot_buy': 'cannot_buy',
         'anti_whale_modifiable': 'anti_whale_modifiable',
         'token_symbol': 'token_symbol'
     }
 
     def __init__(self, note=None, lp_total_supply=None, lp_holders=None, is_airdrop_scam=None, other_potential_risks=None, transfer_pausable=None, trading_cooldown=None, hidden_owner=None, selfdestruct=None, owner_percent=None, is_whitelisted=None, holder_count=None, trust_list=None, is_honeypot=None, holders=None, dex=None, is_open_source=None, sell_tax=None, token_name=None, creator_address=None, creator_percent=None, is_proxy=None, creator_balance=None, is_in_dex=None, owner_balance=None, total_supply=None, is_true_token=None, can_take_back_ownership=None, is_blacklisted=None, owner_address=None, slippage_modifiable=None, buy_tax=None, external_call=None, cannot_sell_all=None, lp_holder_count=None, personal_slippage_modifiable=None, is_anti_whale=None, is_mintable=None, owner_change_balance=None, cannot_buy=None, anti_whale_modifiable=None, token_symbol=None):  # noqa: E501
-        """ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperTokenSecurityResult - a model defined in Swagger"""  # noqa: E501
         self._note = None
         self._lp_total_supply = None
         self._lp_holders = None
         self._is_airdrop_scam = None
         self._other_potential_risks = None
         self._transfer_pausable = None
         self._trading_cooldown = None
@@ -245,973 +245,973 @@
         if anti_whale_modifiable is not None:
             self.anti_whale_modifiable = anti_whale_modifiable
         if token_symbol is not None:
             self.token_symbol = token_symbol
 
     @property
     def note(self):
-        """Gets the note of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the note of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has other things investors need to know.  Example:  \"note”: “Contract owner is a multisign contract.”(Notice:(1) If we haven't found any other thing which is valuable yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
-        :return: The note of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The note of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._note
 
     @note.setter
     def note(self, note):
-        """Sets the note of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the note of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has other things investors need to know.  Example:  \"note”: “Contract owner is a multisign contract.”(Notice:(1) If we haven't found any other thing which is valuable yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
-        :param note: The note of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param note: The note of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._note = note
 
     @property
     def lp_total_supply(self):
-        """Gets the lp_total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the lp_total_supply of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the supply number of the LP token. Example:\"lp_total_supply\": \"100000000\". No return means no LP.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) It is LP token number, NOT token number)  # noqa: E501
 
-        :return: The lp_total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The lp_total_supply of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._lp_total_supply
 
     @lp_total_supply.setter
     def lp_total_supply(self, lp_total_supply):
-        """Sets the lp_total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the lp_total_supply of this ResponseWrapperTokenSecurityResult.
 
         It describes the supply number of the LP token. Example:\"lp_total_supply\": \"100000000\". No return means no LP.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) It is LP token number, NOT token number)  # noqa: E501
 
-        :param lp_total_supply: The lp_total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param lp_total_supply: The lp_total_supply of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._lp_total_supply = lp_total_supply
 
     @property
     def lp_holders(self):
-        """Gets the lp_holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the lp_holders of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         Top10 LP token holders info(Notice:When \"is_in_dex\": \"0\", there will be no return. )  # noqa: E501
 
-        :return: The lp_holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
-        :rtype: list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders]
+        :return: The lp_holders of this ResponseWrapperTokenSecurityResult.  # noqa: E501
+        :rtype: list[ResponseWrapperTokenSecurityLpHolders]
         """
         return self._lp_holders
 
     @lp_holders.setter
     def lp_holders(self, lp_holders):
-        """Sets the lp_holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the lp_holders of this ResponseWrapperTokenSecurityResult.
 
         Top10 LP token holders info(Notice:When \"is_in_dex\": \"0\", there will be no return. )  # noqa: E501
 
-        :param lp_holders: The lp_holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
-        :type: list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders]
+        :param lp_holders: The lp_holders of this ResponseWrapperTokenSecurityResult.  # noqa: E501
+        :type: list[ResponseWrapperTokenSecurityLpHolders]
         """
 
         self._lp_holders = lp_holders
 
     @property
     def is_airdrop_scam(self):
-        """Gets the is_airdrop_scam of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_airdrop_scam of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the token is an airdrop scam. \"1\" means true; \"0\" means false; None means no result (Because We did not find conclusive information on whether token is an airdrop scam).(Notice:Only \"is_airdrop_scam\": \"1\" means it is an airdrop scam.)  # noqa: E501
 
-        :return: The is_airdrop_scam of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_airdrop_scam of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_airdrop_scam
 
     @is_airdrop_scam.setter
     def is_airdrop_scam(self, is_airdrop_scam):
-        """Sets the is_airdrop_scam of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_airdrop_scam of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the token is an airdrop scam. \"1\" means true; \"0\" means false; None means no result (Because We did not find conclusive information on whether token is an airdrop scam).(Notice:Only \"is_airdrop_scam\": \"1\" means it is an airdrop scam.)  # noqa: E501
 
-        :param is_airdrop_scam: The is_airdrop_scam of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_airdrop_scam: The is_airdrop_scam of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_airdrop_scam = is_airdrop_scam
 
     @property
     def other_potential_risks(self):
-        """Gets the other_potential_risks of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the other_potential_risks of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has other potential risks. Example: “other_potential_risks”: “Owner can set different transaction taxes for each user, which can trigger serious losses.”(Notice:(1) If we haven't found any other potential risk yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
-        :return: The other_potential_risks of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The other_potential_risks of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._other_potential_risks
 
     @other_potential_risks.setter
     def other_potential_risks(self, other_potential_risks):
-        """Sets the other_potential_risks of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the other_potential_risks of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has other potential risks. Example: “other_potential_risks”: “Owner can set different transaction taxes for each user, which can trigger serious losses.”(Notice:(1) If we haven't found any other potential risk yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
-        :param other_potential_risks: The other_potential_risks of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param other_potential_risks: The other_potential_risks of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._other_potential_risks = other_potential_risks
 
     @property
     def transfer_pausable(self):
-        """Gets the transfer_pausable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the transfer_pausable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether trading can be pausable by token contract. \"1\" means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) This feature means that the contract owner will be able to suspend trading at any time, after that anyone will not be able to sell, except those who have special authority.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :return: The transfer_pausable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The transfer_pausable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._transfer_pausable
 
     @transfer_pausable.setter
     def transfer_pausable(self, transfer_pausable):
-        """Sets the transfer_pausable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the transfer_pausable of this ResponseWrapperTokenSecurityResult.
 
         It describes whether trading can be pausable by token contract. \"1\" means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) This feature means that the contract owner will be able to suspend trading at any time, after that anyone will not be able to sell, except those who have special authority.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :param transfer_pausable: The transfer_pausable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param transfer_pausable: The transfer_pausable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._transfer_pausable = transfer_pausable
 
     @property
     def trading_cooldown(self):
-        """Gets the trading_cooldown of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the trading_cooldown of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has trading-cool-down mechanism which can limits the minimum time between two transactions. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return. (2) Sometimes, when \"is_proxy\": \"1\", there will be no return. )  # noqa: E501
 
-        :return: The trading_cooldown of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The trading_cooldown of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._trading_cooldown
 
     @trading_cooldown.setter
     def trading_cooldown(self, trading_cooldown):
-        """Sets the trading_cooldown of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the trading_cooldown of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has trading-cool-down mechanism which can limits the minimum time between two transactions. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return. (2) Sometimes, when \"is_proxy\": \"1\", there will be no return. )  # noqa: E501
 
-        :param trading_cooldown: The trading_cooldown of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param trading_cooldown: The trading_cooldown of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._trading_cooldown = trading_cooldown
 
     @property
     def hidden_owner(self):
-        """Gets the hidden_owner of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the hidden_owner of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has hidden owners. For contract with a hidden owner, developer can still manipulate the contract even if the ownership has been abandoned. “1” means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hidden owner is often used by developers to hide ownership and is often accompanied by malicious functionality. When the hidden owner exists, it is assumed that ownership has not been abandoned.)  # noqa: E501
 
-        :return: The hidden_owner of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The hidden_owner of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._hidden_owner
 
     @hidden_owner.setter
     def hidden_owner(self, hidden_owner):
-        """Sets the hidden_owner of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the hidden_owner of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has hidden owners. For contract with a hidden owner, developer can still manipulate the contract even if the ownership has been abandoned. “1” means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hidden owner is often used by developers to hide ownership and is often accompanied by malicious functionality. When the hidden owner exists, it is assumed that ownership has not been abandoned.)  # noqa: E501
 
-        :param hidden_owner: The hidden_owner of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param hidden_owner: The hidden_owner of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._hidden_owner = hidden_owner
 
     @property
     def selfdestruct(self):
-        """Gets the selfdestruct of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the selfdestruct of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether this contract can self destruct. \"1\" means true;  \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) When the self-destruct function is triggered, this contract will be destroyed, all functions will be unavailable, and all related assets will be erased.)  # noqa: E501
 
-        :return: The selfdestruct of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The selfdestruct of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._selfdestruct
 
     @selfdestruct.setter
     def selfdestruct(self, selfdestruct):
-        """Sets the selfdestruct of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the selfdestruct of this ResponseWrapperTokenSecurityResult.
 
         It describes whether this contract can self destruct. \"1\" means true;  \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) When the self-destruct function is triggered, this contract will be destroyed, all functions will be unavailable, and all related assets will be erased.)  # noqa: E501
 
-        :param selfdestruct: The selfdestruct of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param selfdestruct: The selfdestruct of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._selfdestruct = selfdestruct
 
     @property
     def owner_percent(self):
-        """Gets the owner_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the owner_percent of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the percentage of tokens held by the contract owner.  Example:\"owner_balance\": \"0.1\".  No return or return empty means there is no ownership or can't find ownership.(Notice:(1) 1 means 100% here. (2) When \"owner_address\" returns empty, or no return, there will be no return.)  # noqa: E501
 
-        :return: The owner_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The owner_percent of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._owner_percent
 
     @owner_percent.setter
     def owner_percent(self, owner_percent):
-        """Sets the owner_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the owner_percent of this ResponseWrapperTokenSecurityResult.
 
         It describes the percentage of tokens held by the contract owner.  Example:\"owner_balance\": \"0.1\".  No return or return empty means there is no ownership or can't find ownership.(Notice:(1) 1 means 100% here. (2) When \"owner_address\" returns empty, or no return, there will be no return.)  # noqa: E501
 
-        :param owner_percent: The owner_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param owner_percent: The owner_percent of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._owner_percent = owner_percent
 
     @property
     def is_whitelisted(self):
-        """Gets the is_whitelisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_whitelisted of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the whitelist function is not included in the contract. If there is a whitelist, some addresses may not be able to trade normally. \"1\" means true; \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Whitelisting is mostly used to allow specific addresses to make early transactions, tax-free, and not affected by transaction suspension. (4) For contracts without an owner (or the owner is a black hole address), the whitelist will not be able to get updated. However, the existing whitelist is still in effect.)  # noqa: E501
 
-        :return: The is_whitelisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_whitelisted of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_whitelisted
 
     @is_whitelisted.setter
     def is_whitelisted(self, is_whitelisted):
-        """Sets the is_whitelisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_whitelisted of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the whitelist function is not included in the contract. If there is a whitelist, some addresses may not be able to trade normally. \"1\" means true; \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Whitelisting is mostly used to allow specific addresses to make early transactions, tax-free, and not affected by transaction suspension. (4) For contracts without an owner (or the owner is a black hole address), the whitelist will not be able to get updated. However, the existing whitelist is still in effect.)  # noqa: E501
 
-        :param is_whitelisted: The is_whitelisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_whitelisted: The is_whitelisted of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_whitelisted = is_whitelisted
 
     @property
     def holder_count(self):
-        """Gets the holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the holder_count of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the number of token holders. Example:\"holder_count\": \"4342\"  # noqa: E501
 
-        :return: The holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The holder_count of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._holder_count
 
     @holder_count.setter
     def holder_count(self, holder_count):
-        """Sets the holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the holder_count of this ResponseWrapperTokenSecurityResult.
 
         It describes the number of token holders. Example:\"holder_count\": \"4342\"  # noqa: E501
 
-        :param holder_count: The holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param holder_count: The holder_count of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._holder_count = holder_count
 
     @property
     def trust_list(self):
-        """Gets the trust_list of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the trust_list of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the token is a famous and trustworthy one. \"1\" means true; No return no result (Because We did not find conclusive information on whether token is a airdrop scam).(Notice:(1) Only \"trust_list\": \"1\" means it is a famous and trustworthy token.  (2) No return doesn't mean it is risky.)  # noqa: E501
 
-        :return: The trust_list of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The trust_list of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._trust_list
 
     @trust_list.setter
     def trust_list(self, trust_list):
-        """Sets the trust_list of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the trust_list of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the token is a famous and trustworthy one. \"1\" means true; No return no result (Because We did not find conclusive information on whether token is a airdrop scam).(Notice:(1) Only \"trust_list\": \"1\" means it is a famous and trustworthy token.  (2) No return doesn't mean it is risky.)  # noqa: E501
 
-        :param trust_list: The trust_list of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param trust_list: The trust_list of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._trust_list = trust_list
 
     @property
     def is_honeypot(self):
-        """Gets the is_honeypot of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_honeypot of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the token is a honeypot. \"HoneyPot\" means that the token maybe cannot be sold because of the token contract's function, Or the token contains malicious code.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hight risk, definitely scam.)  # noqa: E501
 
-        :return: The is_honeypot of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_honeypot of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_honeypot
 
     @is_honeypot.setter
     def is_honeypot(self, is_honeypot):
-        """Sets the is_honeypot of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_honeypot of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the token is a honeypot. \"HoneyPot\" means that the token maybe cannot be sold because of the token contract's function, Or the token contains malicious code.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hight risk, definitely scam.)  # noqa: E501
 
-        :param is_honeypot: The is_honeypot of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_honeypot: The is_honeypot of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_honeypot = is_honeypot
 
     @property
     def holders(self):
-        """Gets the holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the holders of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         Top10 holders info  # noqa: E501
 
-        :return: The holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
-        :rtype: list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders]
+        :return: The holders of this ResponseWrapperTokenSecurityResult.  # noqa: E501
+        :rtype: list[ResponseWrapperTokenSecurityLpHolders]
         """
         return self._holders
 
     @holders.setter
     def holders(self, holders):
-        """Sets the holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the holders of this ResponseWrapperTokenSecurityResult.
 
         Top10 holders info  # noqa: E501
 
-        :param holders: The holders of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
-        :type: list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2LpHolders]
+        :param holders: The holders of this ResponseWrapperTokenSecurityResult.  # noqa: E501
+        :type: list[ResponseWrapperTokenSecurityLpHolders]
         """
 
         self._holders = holders
 
     @property
     def dex(self):
-        """Gets the dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the dex of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes Dex information of where the token that can be traded.(Notice:When \"is_in_dex\": \"0\", there will be empty array. )  # noqa: E501
 
-        :return: The dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
-        :rtype: list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Dex]
+        :return: The dex of this ResponseWrapperTokenSecurityResult.  # noqa: E501
+        :rtype: list[ResponseWrapperTokenSecurityDex]
         """
         return self._dex
 
     @dex.setter
     def dex(self, dex):
-        """Sets the dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the dex of this ResponseWrapperTokenSecurityResult.
 
         It describes Dex information of where the token that can be traded.(Notice:When \"is_in_dex\": \"0\", there will be empty array. )  # noqa: E501
 
-        :param dex: The dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
-        :type: list[ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Dex]
+        :param dex: The dex of this ResponseWrapperTokenSecurityResult.  # noqa: E501
+        :type: list[ResponseWrapperTokenSecurityDex]
         """
 
         self._dex = dex
 
     @property
     def is_open_source(self):
-        """Gets the is_open_source of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_open_source of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether this contract is open source.  \"1\" means true;  \"0\" means false.(Notice:Un-open-sourced contracts may hide various unknown mechanisms and are extremely risky. When the contract is not open source, we will not be able to detect other risk items.)  # noqa: E501
 
-        :return: The is_open_source of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_open_source of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_open_source
 
     @is_open_source.setter
     def is_open_source(self, is_open_source):
-        """Sets the is_open_source of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_open_source of this ResponseWrapperTokenSecurityResult.
 
         It describes whether this contract is open source.  \"1\" means true;  \"0\" means false.(Notice:Un-open-sourced contracts may hide various unknown mechanisms and are extremely risky. When the contract is not open source, we will not be able to detect other risk items.)  # noqa: E501
 
-        :param is_open_source: The is_open_source of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_open_source: The is_open_source of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_open_source = is_open_source
 
     @property
     def sell_tax(self):
-        """Gets the sell_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the sell_tax of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the tax when selling the token.  Example: \"sell_tax\": 0.1%.  No return means unknown.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) Sell tax will cause the actual value received when selling a token to be less than expected, and too much buy tax may lead to large losses. (3) When \"sell_tax\": \"1\", it means sell-tax is 100% or this token cannot be sold. (4) Sometimes token's  trading-cool-down mechanism would affect our sandbox system. When \"trading_cooldown\": \"1\", \"sell_tax\" may return \"1\".)  # noqa: E501
 
-        :return: The sell_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The sell_tax of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._sell_tax
 
     @sell_tax.setter
     def sell_tax(self, sell_tax):
-        """Sets the sell_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the sell_tax of this ResponseWrapperTokenSecurityResult.
 
         It describes the tax when selling the token.  Example: \"sell_tax\": 0.1%.  No return means unknown.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) Sell tax will cause the actual value received when selling a token to be less than expected, and too much buy tax may lead to large losses. (3) When \"sell_tax\": \"1\", it means sell-tax is 100% or this token cannot be sold. (4) Sometimes token's  trading-cool-down mechanism would affect our sandbox system. When \"trading_cooldown\": \"1\", \"sell_tax\" may return \"1\".)  # noqa: E501
 
-        :param sell_tax: The sell_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param sell_tax: The sell_tax of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._sell_tax = sell_tax
 
     @property
     def token_name(self):
-        """Gets the token_name of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the token_name of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         Token Name  # noqa: E501
 
-        :return: The token_name of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The token_name of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._token_name
 
     @token_name.setter
     def token_name(self, token_name):
-        """Sets the token_name of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the token_name of this ResponseWrapperTokenSecurityResult.
 
         Token Name  # noqa: E501
 
-        :param token_name: The token_name of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param token_name: The token_name of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._token_name = token_name
 
     @property
     def creator_address(self):
-        """Gets the creator_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the creator_address of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes this contract's owner address.  Example: \"creator_address\": \"0x744aF9cBb7606BB040f6FBf1c0a0B0dcBA6385E5\";  # noqa: E501
 
-        :return: The creator_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The creator_address of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._creator_address
 
     @creator_address.setter
     def creator_address(self, creator_address):
-        """Sets the creator_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the creator_address of this ResponseWrapperTokenSecurityResult.
 
         It describes this contract's owner address.  Example: \"creator_address\": \"0x744aF9cBb7606BB040f6FBf1c0a0B0dcBA6385E5\";  # noqa: E501
 
-        :param creator_address: The creator_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param creator_address: The creator_address of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._creator_address = creator_address
 
     @property
     def creator_percent(self):
-        """Gets the creator_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the creator_percent of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the percentage of tokens held by the contract owner. Example:\"owner_balance\": 0.1.(Notice:1 means 100% here.)  # noqa: E501
 
-        :return: The creator_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The creator_percent of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._creator_percent
 
     @creator_percent.setter
     def creator_percent(self, creator_percent):
-        """Sets the creator_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the creator_percent of this ResponseWrapperTokenSecurityResult.
 
         It describes the percentage of tokens held by the contract owner. Example:\"owner_balance\": 0.1.(Notice:1 means 100% here.)  # noqa: E501
 
-        :param creator_percent: The creator_percent of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param creator_percent: The creator_percent of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._creator_percent = creator_percent
 
     @property
     def is_proxy(self):
-        """Gets the is_proxy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_proxy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether this contract has a proxy contract.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Most Proxy contracts are accompanied by modifiable implementation contracts, and implementation contracts may contain significant potential risk. When the contract is a Proxy, we will stop detecting other risk items.)  # noqa: E501
 
-        :return: The is_proxy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_proxy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_proxy
 
     @is_proxy.setter
     def is_proxy(self, is_proxy):
-        """Sets the is_proxy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_proxy of this ResponseWrapperTokenSecurityResult.
 
         It describes whether this contract has a proxy contract.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Most Proxy contracts are accompanied by modifiable implementation contracts, and implementation contracts may contain significant potential risk. When the contract is a Proxy, we will stop detecting other risk items.)  # noqa: E501
 
-        :param is_proxy: The is_proxy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_proxy: The is_proxy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_proxy = is_proxy
 
     @property
     def creator_balance(self):
-        """Gets the creator_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the creator_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the balance of the contract owner.  Example:\"owner_balance\": 100000000.  # noqa: E501
 
-        :return: The creator_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The creator_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._creator_balance
 
     @creator_balance.setter
     def creator_balance(self, creator_balance):
-        """Sets the creator_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the creator_balance of this ResponseWrapperTokenSecurityResult.
 
         It describes the balance of the contract owner.  Example:\"owner_balance\": 100000000.  # noqa: E501
 
-        :param creator_balance: The creator_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param creator_balance: The creator_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._creator_balance = creator_balance
 
     @property
     def is_in_dex(self):
-        """Gets the is_in_dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_in_dex of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the token can be traded on the main Dex. \"1\" means true; \"0\" means false(Notice:It only counts when the token has a marketing pair with mainstream coins/tokens.)  # noqa: E501
 
-        :return: The is_in_dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_in_dex of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_in_dex
 
     @is_in_dex.setter
     def is_in_dex(self, is_in_dex):
-        """Sets the is_in_dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_in_dex of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the token can be traded on the main Dex. \"1\" means true; \"0\" means false(Notice:It only counts when the token has a marketing pair with mainstream coins/tokens.)  # noqa: E501
 
-        :param is_in_dex: The is_in_dex of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_in_dex: The is_in_dex of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_in_dex = is_in_dex
 
     @property
     def owner_balance(self):
-        """Gets the owner_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the owner_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the balance of the contract owner.  Example: \"owner_balance\": \"100000000\".  No return or return empty means there is no ownership or can't find ownership.(Notice:When \"owner_address\" returns empty, or no return, there will be no return.)  # noqa: E501
 
-        :return: The owner_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The owner_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._owner_balance
 
     @owner_balance.setter
     def owner_balance(self, owner_balance):
-        """Sets the owner_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the owner_balance of this ResponseWrapperTokenSecurityResult.
 
         It describes the balance of the contract owner.  Example: \"owner_balance\": \"100000000\".  No return or return empty means there is no ownership or can't find ownership.(Notice:When \"owner_address\" returns empty, or no return, there will be no return.)  # noqa: E501
 
-        :param owner_balance: The owner_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param owner_balance: The owner_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._owner_balance = owner_balance
 
     @property
     def total_supply(self):
-        """Gets the total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the total_supply of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the supply number of the token. Example:\"total_supply\": 100000000  # noqa: E501
 
-        :return: The total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The total_supply of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._total_supply
 
     @total_supply.setter
     def total_supply(self, total_supply):
-        """Sets the total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the total_supply of this ResponseWrapperTokenSecurityResult.
 
         It describes the supply number of the token. Example:\"total_supply\": 100000000  # noqa: E501
 
-        :param total_supply: The total_supply of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param total_supply: The total_supply of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._total_supply = total_supply
 
     @property
     def is_true_token(self):
-        """Gets the is_true_token of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_true_token of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the token is true or fake. \"1\" means true token; \"0\" means fake token; None means no result (Because we did not find decisive information about the truth or falsity)(Notice:Only \"is_true_token\": \"0\" means it is a fake token.)  # noqa: E501
 
-        :return: The is_true_token of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_true_token of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_true_token
 
     @is_true_token.setter
     def is_true_token(self, is_true_token):
-        """Sets the is_true_token of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_true_token of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the token is true or fake. \"1\" means true token; \"0\" means fake token; None means no result (Because we did not find decisive information about the truth or falsity)(Notice:Only \"is_true_token\": \"0\" means it is a fake token.)  # noqa: E501
 
-        :param is_true_token: The is_true_token of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_true_token: The is_true_token of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_true_token = is_true_token
 
     @property
     def can_take_back_ownership(self):
-        """Gets the can_take_back_ownership of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the can_take_back_ownership of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether this contract has the function to take back ownership.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Ownership is mostly used to adjust the parameters and status of the contract, such as minting, modification of slippage, suspension of trading, setting blacklsit, etc.  When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, these functions will most likely be disabled.)  # noqa: E501
 
-        :return: The can_take_back_ownership of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The can_take_back_ownership of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._can_take_back_ownership
 
     @can_take_back_ownership.setter
     def can_take_back_ownership(self, can_take_back_ownership):
-        """Sets the can_take_back_ownership of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the can_take_back_ownership of this ResponseWrapperTokenSecurityResult.
 
         It describes whether this contract has the function to take back ownership.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Ownership is mostly used to adjust the parameters and status of the contract, such as minting, modification of slippage, suspension of trading, setting blacklsit, etc.  When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, these functions will most likely be disabled.)  # noqa: E501
 
-        :param can_take_back_ownership: The can_take_back_ownership of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param can_take_back_ownership: The can_take_back_ownership of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._can_take_back_ownership = can_take_back_ownership
 
     @property
     def is_blacklisted(self):
-        """Gets the is_blacklisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_blacklisted of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the blacklist function is not included in the contract. If there is a blacklist, some addresses may not be able to trade normally. \"1\" means true; \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\",  there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) The contract owner may add any address into the blacklist, and the token holder in blacklist will not be able to trade. Abuse of the blacklist function will lead to great risks.  (4) For contracts without an owner (or the owner is a black hole address), the blacklist will not be able to get updated. However, the existing blacklist is still in effect.)  # noqa: E501
 
-        :return: The is_blacklisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_blacklisted of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_blacklisted
 
     @is_blacklisted.setter
     def is_blacklisted(self, is_blacklisted):
-        """Sets the is_blacklisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_blacklisted of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the blacklist function is not included in the contract. If there is a blacklist, some addresses may not be able to trade normally. \"1\" means true; \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\",  there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) The contract owner may add any address into the blacklist, and the token holder in blacklist will not be able to trade. Abuse of the blacklist function will lead to great risks.  (4) For contracts without an owner (or the owner is a black hole address), the blacklist will not be able to get updated. However, the existing blacklist is still in effect.)  # noqa: E501
 
-        :param is_blacklisted: The is_blacklisted of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_blacklisted: The is_blacklisted of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_blacklisted = is_blacklisted
 
     @property
     def owner_address(self):
-        """Gets the owner_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the owner_address of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes this contract's owner address.  Example: \"owner_address\": \"0x744aF9cBb7606BB040f6FBf1c0a0B0dcBA6385E5\";  No return means unknown; Return empty means there is no ownership or can't find ownership.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Ownership is mostly used to adjust the parameters and status of the contract, such as minting, modification of slippage, suspension of trading, setting blacklist, etc.  When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, these functions will most likely be disabled.)  # noqa: E501
 
-        :return: The owner_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The owner_address of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._owner_address
 
     @owner_address.setter
     def owner_address(self, owner_address):
-        """Sets the owner_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the owner_address of this ResponseWrapperTokenSecurityResult.
 
         It describes this contract's owner address.  Example: \"owner_address\": \"0x744aF9cBb7606BB040f6FBf1c0a0B0dcBA6385E5\";  No return means unknown; Return empty means there is no ownership or can't find ownership.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Ownership is mostly used to adjust the parameters and status of the contract, such as minting, modification of slippage, suspension of trading, setting blacklist, etc.  When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, these functions will most likely be disabled.)  # noqa: E501
 
-        :param owner_address: The owner_address of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param owner_address: The owner_address of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._owner_address = owner_address
 
     @property
     def slippage_modifiable(self):
-        """Gets the slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the slippage_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the trading tax can be modifiable by token contract. \"1\" means true; \"0\" means false; No return means unknown.(Notice:(1) When When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Token with modifiable tax means that the contract owner can modify the buy tax or sell tax of the token. This may cause some losses, especially since some contracts have unlimited modifiable tax rates, which would make the token untradeable.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :return: The slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The slippage_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._slippage_modifiable
 
     @slippage_modifiable.setter
     def slippage_modifiable(self, slippage_modifiable):
-        """Sets the slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the slippage_modifiable of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the trading tax can be modifiable by token contract. \"1\" means true; \"0\" means false; No return means unknown.(Notice:(1) When When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Token with modifiable tax means that the contract owner can modify the buy tax or sell tax of the token. This may cause some losses, especially since some contracts have unlimited modifiable tax rates, which would make the token untradeable.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :param slippage_modifiable: The slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param slippage_modifiable: The slippage_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._slippage_modifiable = slippage_modifiable
 
     @property
     def buy_tax(self):
-        """Gets the buy_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the buy_tax of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the tax when buying the token.  Example: \"buy_tax\": 0.1%.  No return means unknown.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) Buy tax will cause the actual value received when buying a token to be less than expected, and too much buy tax may lead to heavy losses. (3) When \"buy_tax\": \"1\", it means buy tax is 100% or cannot buy. (4) Sometimes token's anti-bot mechanism would affect our sandbox system, leading to \"cannoy_buy\": \"1\",  causing the display of \"buy_tax\": \"1\". (5)Some of the token is deisgned not for sale, leading to \"cannot_buy\":1, causing the display of \"buy_tax\": \"1\".)  # noqa: E501
 
-        :return: The buy_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The buy_tax of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._buy_tax
 
     @buy_tax.setter
     def buy_tax(self, buy_tax):
-        """Sets the buy_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the buy_tax of this ResponseWrapperTokenSecurityResult.
 
         It describes the tax when buying the token.  Example: \"buy_tax\": 0.1%.  No return means unknown.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) Buy tax will cause the actual value received when buying a token to be less than expected, and too much buy tax may lead to heavy losses. (3) When \"buy_tax\": \"1\", it means buy tax is 100% or cannot buy. (4) Sometimes token's anti-bot mechanism would affect our sandbox system, leading to \"cannoy_buy\": \"1\",  causing the display of \"buy_tax\": \"1\". (5)Some of the token is deisgned not for sale, leading to \"cannot_buy\":1, causing the display of \"buy_tax\": \"1\".)  # noqa: E501
 
-        :param buy_tax: The buy_tax of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param buy_tax: The buy_tax of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._buy_tax = buy_tax
 
     @property
     def external_call(self):
-        """Gets the external_call of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the external_call of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract would call functions of other contracts when primary methods are executed. \"1\" means true;  \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) External call would cause the implementation of this contract to be highly dependent on other external contracts, which may be a potential risk.)  # noqa: E501
 
-        :return: The external_call of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The external_call of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._external_call
 
     @external_call.setter
     def external_call(self, external_call):
-        """Sets the external_call of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the external_call of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract would call functions of other contracts when primary methods are executed. \"1\" means true;  \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) External call would cause the implementation of this contract to be highly dependent on other external contracts, which may be a potential risk.)  # noqa: E501
 
-        :param external_call: The external_call of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param external_call: The external_call of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._external_call = external_call
 
     @property
     def cannot_sell_all(self):
-        """Gets the cannot_sell_all of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the cannot_sell_all of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has the function restricting token holder selling all the token.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) This feature means that you will not be able to sell all your tokens in a single sale. Sometimes you need to leave a certain percentage of the token, e.g. 10%, sometimes you need to leave a fixed number of token, such as 10 token. (3) When \"buy_tax\": \"1\", there will be no return.)  # noqa: E501
 
-        :return: The cannot_sell_all of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The cannot_sell_all of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._cannot_sell_all
 
     @cannot_sell_all.setter
     def cannot_sell_all(self, cannot_sell_all):
-        """Sets the cannot_sell_all of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the cannot_sell_all of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has the function restricting token holder selling all the token.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_in_dex\": \"0\", there will be no return.  (2) This feature means that you will not be able to sell all your tokens in a single sale. Sometimes you need to leave a certain percentage of the token, e.g. 10%, sometimes you need to leave a fixed number of token, such as 10 token. (3) When \"buy_tax\": \"1\", there will be no return.)  # noqa: E501
 
-        :param cannot_sell_all: The cannot_sell_all of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param cannot_sell_all: The cannot_sell_all of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._cannot_sell_all = cannot_sell_all
 
     @property
     def lp_holder_count(self):
-        """Gets the lp_holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the lp_holder_count of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes the number of LP token holders. Example:\"lp_holder_count\": \"4342\". No return means no LP.(Notice:When \"is_in_dex\": \"0\", there will be no return.)  # noqa: E501
 
-        :return: The lp_holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The lp_holder_count of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._lp_holder_count
 
     @lp_holder_count.setter
     def lp_holder_count(self, lp_holder_count):
-        """Sets the lp_holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the lp_holder_count of this ResponseWrapperTokenSecurityResult.
 
         It describes the number of LP token holders. Example:\"lp_holder_count\": \"4342\". No return means no LP.(Notice:When \"is_in_dex\": \"0\", there will be no return.)  # noqa: E501
 
-        :param lp_holder_count: The lp_holder_count of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param lp_holder_count: The lp_holder_count of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._lp_holder_count = lp_holder_count
 
     @property
     def personal_slippage_modifiable(self):
-        """Gets the personal_slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the personal_slippage_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the owner can set a different tax rate for every assigned address. \"1\" means ture; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\",  there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) The contract owner may set a very outrageous tax rate for assigned address to block it from trading. Abuse of this funtcion will lead to great risks.  (4) For contracts without an owner (or the owner is a black hole address), this function would not able to be used. However, the existing tax rate would be still in effect.)  # noqa: E501
 
-        :return: The personal_slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The personal_slippage_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._personal_slippage_modifiable
 
     @personal_slippage_modifiable.setter
     def personal_slippage_modifiable(self, personal_slippage_modifiable):
-        """Sets the personal_slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the personal_slippage_modifiable of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the owner can set a different tax rate for every assigned address. \"1\" means ture; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\",  there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) The contract owner may set a very outrageous tax rate for assigned address to block it from trading. Abuse of this funtcion will lead to great risks.  (4) For contracts without an owner (or the owner is a black hole address), this function would not able to be used. However, the existing tax rate would be still in effect.)  # noqa: E501
 
-        :param personal_slippage_modifiable: The personal_slippage_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param personal_slippage_modifiable: The personal_slippage_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._personal_slippage_modifiable = personal_slippage_modifiable
 
     @property
     def is_anti_whale(self):
-        """Gets the is_anti_whale of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_anti_whale of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has the function to limit the maximum amount of transactions or the maximum token position that for single address.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return. (2) Sometimes, when \"is_proxy\": \"1\", there will be no return. )  # noqa: E501
 
-        :return: The is_anti_whale of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_anti_whale of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_anti_whale
 
     @is_anti_whale.setter
     def is_anti_whale(self, is_anti_whale):
-        """Sets the is_anti_whale of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_anti_whale of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has the function to limit the maximum amount of transactions or the maximum token position that for single address.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return. (2) Sometimes, when \"is_proxy\": \"1\", there will be no return. )  # noqa: E501
 
-        :param is_anti_whale: The is_anti_whale of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_anti_whale: The is_anti_whale of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_anti_whale = is_anti_whale
 
     @property
     def is_mintable(self):
-        """Gets the is_mintable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the is_mintable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether this contract has the function to mint tokens.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Mint function will directly trigger a massive sell-off, causing the coin price to plummet. It is extremely risky.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :return: The is_mintable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The is_mintable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._is_mintable
 
     @is_mintable.setter
     def is_mintable(self, is_mintable):
-        """Sets the is_mintable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the is_mintable of this ResponseWrapperTokenSecurityResult.
 
         It describes whether this contract has the function to mint tokens.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Mint function will directly trigger a massive sell-off, causing the coin price to plummet. It is extremely risky.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :param is_mintable: The is_mintable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param is_mintable: The is_mintable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._is_mintable = is_mintable
 
     @property
     def owner_change_balance(self):
-        """Gets the owner_change_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the owner_change_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract owner has the authority to change the balance of any token holder.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Token with this feature means that the owner can modify anyone's balance, resulting in an asset straight to zero or a massive minting and sell-off.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :return: The owner_change_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The owner_change_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._owner_change_balance
 
     @owner_change_balance.setter
     def owner_change_balance(self, owner_change_balance):
-        """Sets the owner_change_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the owner_change_balance of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract owner has the authority to change the balance of any token holder.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Token with this feature means that the owner can modify anyone's balance, resulting in an asset straight to zero or a massive minting and sell-off.  (4) This function generally relies on ownership. When the contract does not have an owner (or if the owner is a black hole address) and the owner cannot be retrieved, this function will most likely be disabled.)  # noqa: E501
 
-        :param owner_change_balance: The owner_change_balance of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param owner_change_balance: The owner_change_balance of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._owner_change_balance = owner_change_balance
 
     @property
     def cannot_buy(self):
-        """Gets the cannot_buy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the cannot_buy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It deiscribes whether the Token can be bought. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) Generally, \"cannot_buy\": \"1\" would be found in Reward Tokens. Such Tokens are issued as rewards for some on-chain applications and cannot be bought directly by users. (2) Sometimes token's anti-bot mechanism would affect our sandbox system, causing the display of \"buy_tax\": \"1\". (3) When “cannot_buy”: \"1\", our sandbox system might be bloked, causing the display of \"buy_tax\": \"1\" and \"sell_tax\": \"1\")  # noqa: E501
 
-        :return: The cannot_buy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The cannot_buy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._cannot_buy
 
     @cannot_buy.setter
     def cannot_buy(self, cannot_buy):
-        """Sets the cannot_buy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the cannot_buy of this ResponseWrapperTokenSecurityResult.
 
         It deiscribes whether the Token can be bought. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) Generally, \"cannot_buy\": \"1\" would be found in Reward Tokens. Such Tokens are issued as rewards for some on-chain applications and cannot be bought directly by users. (2) Sometimes token's anti-bot mechanism would affect our sandbox system, causing the display of \"buy_tax\": \"1\". (3) When “cannot_buy”: \"1\", our sandbox system might be bloked, causing the display of \"buy_tax\": \"1\" and \"sell_tax\": \"1\")  # noqa: E501
 
-        :param cannot_buy: The cannot_buy of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param cannot_buy: The cannot_buy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._cannot_buy = cannot_buy
 
     @property
     def anti_whale_modifiable(self):
-        """Gets the anti_whale_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the anti_whale_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         It describes whether the contract has the function to modify the maximum amount of transactions or the maximum token position.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return. (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3)When the anti whale value is set to a very small value, all tradinge would fail.)  # noqa: E501
 
-        :return: The anti_whale_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The anti_whale_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._anti_whale_modifiable
 
     @anti_whale_modifiable.setter
     def anti_whale_modifiable(self, anti_whale_modifiable):
-        """Sets the anti_whale_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the anti_whale_modifiable of this ResponseWrapperTokenSecurityResult.
 
         It describes whether the contract has the function to modify the maximum amount of transactions or the maximum token position.  \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return. (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3)When the anti whale value is set to a very small value, all tradinge would fail.)  # noqa: E501
 
-        :param anti_whale_modifiable: The anti_whale_modifiable of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param anti_whale_modifiable: The anti_whale_modifiable of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._anti_whale_modifiable = anti_whale_modifiable
 
     @property
     def token_symbol(self):
-        """Gets the token_symbol of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        """Gets the token_symbol of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
         Token Symbol  # noqa: E501
 
-        :return: The token_symbol of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :return: The token_symbol of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._token_symbol
 
     @token_symbol.setter
     def token_symbol(self, token_symbol):
-        """Sets the token_symbol of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.
+        """Sets the token_symbol of this ResponseWrapperTokenSecurityResult.
 
         Token Symbol  # noqa: E501
 
-        :param token_symbol: The token_symbol of this ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result.  # noqa: E501
+        :param token_symbol: The token_symbol of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._token_symbol = token_symbol
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -1230,15 +1230,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result, dict):
+        if issubclass(ResponseWrapperTokenSecurityResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -1246,15 +1246,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperTaTokenSecurityResponse205696bcfb354bc5ab26ddc7cd495fe2Result):
+        if not isinstance(other, ResponseWrapperTokenSecurityResult):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapperobject.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_get_nft_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,124 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperobject(object):
+class ResponseWrapperGetNftInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'code': 'int',
         'message': 'str',
-        'result': 'object'
+        'result': 'ResponseWrapperGetNftInfoResult'
     }
 
     attribute_map = {
         'code': 'code',
         'message': 'message',
         'result': 'result'
     }
 
     def __init__(self, code=None, message=None, result=None):  # noqa: E501
-        """ResponseWrapperobject - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperGetNftInfo - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self._result = None
         self.discriminator = None
         if code is not None:
             self.code = code
         if message is not None:
             self.message = message
         if result is not None:
             self.result = result
 
     @property
     def code(self):
-        """Gets the code of this ResponseWrapperobject.  # noqa: E501
+        """Gets the code of this ResponseWrapperGetNftInfo.  # noqa: E501
 
         Code 1：Success  # noqa: E501
 
-        :return: The code of this ResponseWrapperobject.  # noqa: E501
+        :return: The code of this ResponseWrapperGetNftInfo.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ResponseWrapperobject.
+        """Sets the code of this ResponseWrapperGetNftInfo.
 
         Code 1：Success  # noqa: E501
 
-        :param code: The code of this ResponseWrapperobject.  # noqa: E501
+        :param code: The code of this ResponseWrapperGetNftInfo.  # noqa: E501
         :type: int
         """
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ResponseWrapperobject.  # noqa: E501
+        """Gets the message of this ResponseWrapperGetNftInfo.  # noqa: E501
 
         Response message  # noqa: E501
 
-        :return: The message of this ResponseWrapperobject.  # noqa: E501
+        :return: The message of this ResponseWrapperGetNftInfo.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ResponseWrapperobject.
+        """Sets the message of this ResponseWrapperGetNftInfo.
 
         Response message  # noqa: E501
 
-        :param message: The message of this ResponseWrapperobject.  # noqa: E501
+        :param message: The message of this ResponseWrapperGetNftInfo.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def result(self):
-        """Gets the result of this ResponseWrapperobject.  # noqa: E501
+        """Gets the result of this ResponseWrapperGetNftInfo.  # noqa: E501
 
-        Response result  # noqa: E501
 
-        :return: The result of this ResponseWrapperobject.  # noqa: E501
-        :rtype: object
+        :return: The result of this ResponseWrapperGetNftInfo.  # noqa: E501
+        :rtype: ResponseWrapperGetNftInfoResult
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this ResponseWrapperobject.
+        """Sets the result of this ResponseWrapperGetNftInfo.
 
-        Response result  # noqa: E501
 
-        :param result: The result of this ResponseWrapperobject.  # noqa: E501
-        :type: object
+        :param result: The result of this ResponseWrapperGetNftInfo.  # noqa: E501
+        :type: ResponseWrapperGetNftInfoResult
         """
 
         self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -138,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperobject, dict):
+        if issubclass(ResponseWrapperGetNftInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperobject):
+        if not isinstance(other, ResponseWrapperGetNftInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/response_wrapperobject545a2ceab58741b4aae7f3d73df91255_result.py` & `goplus-0.1.1/swagger_client/models/response_wrapper_address_contract_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result(object):
+class ResponseWrapperAddressContractResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -62,15 +62,15 @@
         'sanctioned': 'sanctioned',
         'malicious_mining_activities': 'malicious_mining_activities',
         'mixer': 'mixer',
         'honeypot_related_address': 'honeypot_related_address'
     }
 
     def __init__(self, cybercrime=None, money_laundering=None, number_of_malicious_contracts_created=None, financial_crime=None, darkweb_transactions=None, phishing_activities=None, contract_address=None, fake_kyc=None, blacklist_doubt=None, data_source=None, stealing_attack=None, blackmail_activities=None, sanctioned=None, malicious_mining_activities=None, mixer=None, honeypot_related_address=None):  # noqa: E501
-        """ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result - a model defined in Swagger"""  # noqa: E501
+        """ResponseWrapperAddressContractResult - a model defined in Swagger"""  # noqa: E501
         self._cybercrime = None
         self._money_laundering = None
         self._number_of_malicious_contracts_created = None
         self._financial_crime = None
         self._darkweb_transactions = None
         self._phishing_activities = None
         self._contract_address = None
@@ -115,375 +115,375 @@
         if mixer is not None:
             self.mixer = mixer
         if honeypot_related_address is not None:
             self.honeypot_related_address = honeypot_related_address
 
     @property
     def cybercrime(self):
-        """Gets the cybercrime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the cybercrime of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in cybercrime. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The cybercrime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The cybercrime of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._cybercrime
 
     @cybercrime.setter
     def cybercrime(self, cybercrime):
-        """Sets the cybercrime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the cybercrime of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is involved in cybercrime. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param cybercrime: The cybercrime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param cybercrime: The cybercrime of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._cybercrime = cybercrime
 
     @property
     def money_laundering(self):
-        """Gets the money_laundering of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the money_laundering of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in money laundering. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The money_laundering of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The money_laundering of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._money_laundering
 
     @money_laundering.setter
     def money_laundering(self, money_laundering):
-        """Sets the money_laundering of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the money_laundering of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is involved in money laundering. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param money_laundering: The money_laundering of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param money_laundering: The money_laundering of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._money_laundering = money_laundering
 
     @property
     def number_of_malicious_contracts_created(self):
-        """Gets the number_of_malicious_contracts_created of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the number_of_malicious_contracts_created of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         This parameter describes how many malicious contracts have been created by this address.  # noqa: E501
 
-        :return: The number_of_malicious_contracts_created of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The number_of_malicious_contracts_created of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._number_of_malicious_contracts_created
 
     @number_of_malicious_contracts_created.setter
     def number_of_malicious_contracts_created(self, number_of_malicious_contracts_created):
-        """Sets the number_of_malicious_contracts_created of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the number_of_malicious_contracts_created of this ResponseWrapperAddressContractResult.
 
         This parameter describes how many malicious contracts have been created by this address.  # noqa: E501
 
-        :param number_of_malicious_contracts_created: The number_of_malicious_contracts_created of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param number_of_malicious_contracts_created: The number_of_malicious_contracts_created of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._number_of_malicious_contracts_created = number_of_malicious_contracts_created
 
     @property
     def financial_crime(self):
-        """Gets the financial_crime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the financial_crime of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in financial crime. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The financial_crime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The financial_crime of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._financial_crime
 
     @financial_crime.setter
     def financial_crime(self, financial_crime):
-        """Sets the financial_crime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the financial_crime of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is involved in financial crime. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param financial_crime: The financial_crime of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param financial_crime: The financial_crime of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._financial_crime = financial_crime
 
     @property
     def darkweb_transactions(self):
-        """Gets the darkweb_transactions of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the darkweb_transactions of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in darkweb transactions. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The darkweb_transactions of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The darkweb_transactions of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._darkweb_transactions
 
     @darkweb_transactions.setter
     def darkweb_transactions(self, darkweb_transactions):
-        """Sets the darkweb_transactions of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the darkweb_transactions of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is involved in darkweb transactions. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param darkweb_transactions: The darkweb_transactions of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param darkweb_transactions: The darkweb_transactions of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._darkweb_transactions = darkweb_transactions
 
     @property
     def phishing_activities(self):
-        """Gets the phishing_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the phishing_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address has implemented phishing activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The phishing_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The phishing_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._phishing_activities
 
     @phishing_activities.setter
     def phishing_activities(self, phishing_activities):
-        """Sets the phishing_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the phishing_activities of this ResponseWrapperAddressContractResult.
 
         It describes whether this address has implemented phishing activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param phishing_activities: The phishing_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param phishing_activities: The phishing_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._phishing_activities = phishing_activities
 
     @property
     def contract_address(self):
-        """Gets the contract_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the contract_address of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is a contract address. \"1\" means true; \"0\" means false.(Notice:If only the address is sent to the API and not the chain id, the \"contract_address\" will not be returned (This is because there are cases where the same address is a contract in one public chain but not in other public chains.) Determining the contract address is achieved by calling a third-party blockchain browser interface. Since it takes time for the browser interface to return, the field may be empty on the first request. Solution: the second call around 5s can return whether the address is the value of the contract normally.)  # noqa: E501
 
-        :return: The contract_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The contract_address of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._contract_address
 
     @contract_address.setter
     def contract_address(self, contract_address):
-        """Sets the contract_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the contract_address of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is a contract address. \"1\" means true; \"0\" means false.(Notice:If only the address is sent to the API and not the chain id, the \"contract_address\" will not be returned (This is because there are cases where the same address is a contract in one public chain but not in other public chains.) Determining the contract address is achieved by calling a third-party blockchain browser interface. Since it takes time for the browser interface to return, the field may be empty on the first request. Solution: the second call around 5s can return whether the address is the value of the contract normally.)  # noqa: E501
 
-        :param contract_address: The contract_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param contract_address: The contract_address of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._contract_address = contract_address
 
     @property
     def fake_kyc(self):
-        """Gets the fake_kyc of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the fake_kyc of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in fake KYC. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The fake_kyc of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The fake_kyc of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._fake_kyc
 
     @fake_kyc.setter
     def fake_kyc(self, fake_kyc):
-        """Sets the fake_kyc of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the fake_kyc of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is involved in fake KYC. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param fake_kyc: The fake_kyc of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param fake_kyc: The fake_kyc of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._fake_kyc = fake_kyc
 
     @property
     def blacklist_doubt(self):
-        """Gets the blacklist_doubt of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the blacklist_doubt of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is suspected of malicious behavior. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The blacklist_doubt of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The blacklist_doubt of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._blacklist_doubt
 
     @blacklist_doubt.setter
     def blacklist_doubt(self, blacklist_doubt):
-        """Sets the blacklist_doubt of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the blacklist_doubt of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is suspected of malicious behavior. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param blacklist_doubt: The blacklist_doubt of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param blacklist_doubt: The blacklist_doubt of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._blacklist_doubt = blacklist_doubt
 
     @property
     def data_source(self):
-        """Gets the data_source of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes the data source for this address information. For example：GoPlus/SlowMist  # noqa: E501
 
-        :return: The data_source of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._data_source
 
     @data_source.setter
     def data_source(self, data_source):
-        """Sets the data_source of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the data_source of this ResponseWrapperAddressContractResult.
 
         It describes the data source for this address information. For example：GoPlus/SlowMist  # noqa: E501
 
-        :param data_source: The data_source of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param data_source: The data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._data_source = data_source
 
     @property
     def stealing_attack(self):
-        """Gets the stealing_attack of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the stealing_attack of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address has implemented stealing attacks. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The stealing_attack of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The stealing_attack of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._stealing_attack
 
     @stealing_attack.setter
     def stealing_attack(self, stealing_attack):
-        """Sets the stealing_attack of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the stealing_attack of this ResponseWrapperAddressContractResult.
 
         It describes whether this address has implemented stealing attacks. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param stealing_attack: The stealing_attack of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param stealing_attack: The stealing_attack of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._stealing_attack = stealing_attack
 
     @property
     def blackmail_activities(self):
-        """Gets the blackmail_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the blackmail_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address has implemented blackmail activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The blackmail_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The blackmail_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._blackmail_activities
 
     @blackmail_activities.setter
     def blackmail_activities(self, blackmail_activities):
-        """Sets the blackmail_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the blackmail_activities of this ResponseWrapperAddressContractResult.
 
         It describes whether this address has implemented blackmail activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param blackmail_activities: The blackmail_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param blackmail_activities: The blackmail_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._blackmail_activities = blackmail_activities
 
     @property
     def sanctioned(self):
-        """Gets the sanctioned of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the sanctioned of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is coin sanctioned address. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The sanctioned of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The sanctioned of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._sanctioned
 
     @sanctioned.setter
     def sanctioned(self, sanctioned):
-        """Sets the sanctioned of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the sanctioned of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is coin sanctioned address. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param sanctioned: The sanctioned of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param sanctioned: The sanctioned of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._sanctioned = sanctioned
 
     @property
     def malicious_mining_activities(self):
-        """Gets the malicious_mining_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the malicious_mining_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in malicious mining activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :return: The malicious_mining_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The malicious_mining_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._malicious_mining_activities
 
     @malicious_mining_activities.setter
     def malicious_mining_activities(self, malicious_mining_activities):
-        """Sets the malicious_mining_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the malicious_mining_activities of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is involved in malicious mining activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
-        :param malicious_mining_activities: The malicious_mining_activities of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param malicious_mining_activities: The malicious_mining_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._malicious_mining_activities = malicious_mining_activities
 
     @property
     def mixer(self):
-        """Gets the mixer of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the mixer of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is coin mixer address. \"1\" means true; \"0\" means false.(Notice:Interacting with coin mixer may result in your address being added to the risk list of third-party institutions.)  # noqa: E501
 
-        :return: The mixer of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The mixer of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._mixer
 
     @mixer.setter
     def mixer(self, mixer):
-        """Sets the mixer of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the mixer of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is coin mixer address. \"1\" means true; \"0\" means false.(Notice:Interacting with coin mixer may result in your address being added to the risk list of third-party institutions.)  # noqa: E501
 
-        :param mixer: The mixer of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param mixer: The mixer of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._mixer = mixer
 
     @property
     def honeypot_related_address(self):
-        """Gets the honeypot_related_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        """Gets the honeypot_related_address of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is related to honeypot tokens or has created scam tokens. \"1\" means true; \"0\" means false.(Notice:Addresses related to honeypot mean the creators or owners of the honeypot tokens. This is a dangerous address if the address is ralated to honeypot tokens.)  # noqa: E501
 
-        :return: The honeypot_related_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :return: The honeypot_related_address of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._honeypot_related_address
 
     @honeypot_related_address.setter
     def honeypot_related_address(self, honeypot_related_address):
-        """Sets the honeypot_related_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.
+        """Sets the honeypot_related_address of this ResponseWrapperAddressContractResult.
 
         It describes whether this address is related to honeypot tokens or has created scam tokens. \"1\" means true; \"0\" means false.(Notice:Addresses related to honeypot mean the creators or owners of the honeypot tokens. This is a dangerous address if the address is ralated to honeypot tokens.)  # noqa: E501
 
-        :param honeypot_related_address: The honeypot_related_address of this ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result.  # noqa: E501
+        :param honeypot_related_address: The honeypot_related_address of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._honeypot_related_address = honeypot_related_address
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -502,15 +502,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result, dict):
+        if issubclass(ResponseWrapperAddressContractResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -518,15 +518,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResponseWrapperobject545a2ceab58741b4aae7f3d73df91255Result):
+        if not isinstance(other, ResponseWrapperAddressContractResult):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `goplus-0.1.0/swagger_client/models/ta_token_security_response.py` & `goplus-0.1.1/swagger_client/models/ta_token_security_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

### Comparing `goplus-0.1.0/swagger_client/rest.py` & `goplus-0.1.1/swagger_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    GoPlus Security API Documentation
+    GoPlus Security API Document
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
```

