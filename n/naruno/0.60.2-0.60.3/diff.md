# Comparing `tmp/naruno-0.60.2.tar.gz` & `tmp/naruno-0.60.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.60.2.tar", last modified: Tue Aug  1 14:28:23 2023, max compression
+gzip compressed data, was "naruno-0.60.3.tar", last modified: Wed Aug  2 15:08:28 2023, max compression
```

## Comparing `naruno-0.60.2.tar` & `naruno-0.60.3.tar`

### file list

```diff
@@ -1,304 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-lib-kot__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 14:28:12.000000 naruno-0.60.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-01 14:28:23.588044 naruno-0.60.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-08-01 14:28:12.000000 naruno-0.60.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.564043 naruno-0.60.2/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/apps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    29947 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/just_one_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.564043 naruno-0.60.2/naruno/gui/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.580044 naruno-0.60.2/naruno/gui/lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.580044 naruno-0.60.2/naruno/gui/lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.564043 naruno-0.60.2/naruno/gui/lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.580044 naruno-0.60.2/naruno/gui/lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/gui/lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/welcome_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/kot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:28:23.588044 naruno-0.60.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-01 14:28:12.000000 naruno-0.60.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-lib-kot__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 15:08:12.000000 naruno-0.60.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-02 15:08:28.646721 naruno-0.60.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-08-02 15:08:12.000000 naruno-0.60.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/apps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30414 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.586721 naruno-0.60.3/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    19173 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.594721 naruno-0.60.3/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.590721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.594721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.606721 naruno-0.60.3/naruno/gui/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.630721 naruno-0.60.3/naruno/gui/lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.634721 naruno-0.60.3/naruno/gui/lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.606721 naruno-0.60.3/naruno/gui/lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.634721 naruno-0.60.3/naruno/gui/lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.634721 naruno-0.60.3/naruno/gui/lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/welcome_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/kot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:08:28.646721 naruno-0.60.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-02 15:08:12.000000 naruno-0.60.3/setup.py
```

### Comparing `naruno-0.60.2/LICENCE-naruno-gui_lib__.md` & `naruno-0.60.3/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/LICENCE-naruno-lib-kot__.md` & `naruno-0.60.3/LICENCE-naruno-lib-kot__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/LICENCE-naruno-lib-mix__.md` & `naruno-0.60.3/LICENCE-naruno-lib-mix__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.60.3/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/LICENSE-others__.md` & `naruno-0.60.3/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/PKG-INFO` & `naruno-0.60.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.60.2
+Version: 0.60.3
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.60.2 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.3 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.60.2/README.md` & `naruno-0.60.3/README.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/account.py` & `naruno-0.60.3/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/commanders/delete_commander.py` & `naruno-0.60.3/naruno/accounts/commanders/delete_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/commanders/get_comnder.py` & `naruno-0.60.3/naruno/accounts/commanders/get_comnder.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/commanders/save_commander.py` & `naruno-0.60.3/naruno/accounts/commanders/save_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/get_accounts.py` & `naruno-0.60.3/naruno/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/get_balance.py` & `naruno-0.60.3/naruno/accounts/get_balance.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/get_sequence_number.py` & `naruno-0.60.3/naruno/accounts/get_sequence_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/accounts/save_accounts.py` & `naruno-0.60.3/naruno/accounts/save_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/api/buildozer/main.py` & `naruno-0.60.3/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/api/main.py` & `naruno-0.60.3/naruno/api/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/apps/checker.py` & `naruno-0.60.3/naruno/apps/checker.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/apps/remote_app.py` & `naruno-0.60.3/naruno/apps/remote_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,16 @@
         a_block = Block("Onur")
 
         if wait_amount is None:
             self.wait_amount = a_block.block_time * 4
         else:
             self.wait_amount = wait_amount
 
-        self.wait_amount_between_multiple_sendings = wait_amount_between_multiple_sendings
+        self.wait_amount_between_multiple_sendings = (
+            wait_amount_between_multiple_sendings)
 
         self.get_cache()
 
         self.sended_txs = []
 
         self.checking = checking
 
@@ -153,15 +154,16 @@
                 self.total_check = False if "true" in self.total_check else True
 
             self.original_wait_amoount = copy.copy(self.wait_amount)
 
             self.check_thread = (perpetualTimer(
                 self.original_wait_amoount, checker,
                 (self, )) if self.total_check else self.check_thread)
-            self.wait_amount = (self.wait_amount_between_multiple_sendings if self.total_check else self.wait_amount)
+            self.wait_amount = (self.wait_amount_between_multiple_sendings
+                                if self.total_check else self.wait_amount)
             success = True
         except:
             traceback.print_exc()
 
         logger.error("Network is not active") if not success else None
         self.close() if not success else None
         sys.exit() if not success else None
@@ -387,15 +389,14 @@
                 to_user,
                 system_length,
                 true_length,
                 force=force,
                 retrysecond=retrysecond,
             )
         else:
-
             data = json.dumps(data)
 
             request_body = {
                 "password": self.password,
                 "to_user": to_user,
                 "data": data,
             }
@@ -403,29 +404,31 @@
             alread_in_sended = False
             for tx in self.sended_txs:
                 if (tx[0] == action and tx[1] == app_data and tx[2] == to_user
                         and tx[3] == amount and tx[4] == force
                         and tx[5] == retrysecond and tx[6] == data):
                     alread_in_sended = True
             if not alread_in_sended:
-                self.sended_txs.append(
-                    [action, app_data, to_user, amount, force, retrysecond, data])
+                self.sended_txs.append([
+                    action, app_data, to_user, amount, force, retrysecond, data
+                ])
 
             if amount is not None:
                 request_body["amount"] = amount
 
             response = self.prepare_request("/send/",
                                             type="post",
                                             data=request_body)
 
             if "false" in response.text:
                 logger.error("Error on sending message")
                 if force:
                     logger.info("Trying to send again")
-                    return self.send_forcer(action, app_data, to_user, retrysecond)
+                    return self.send_forcer(action, app_data, to_user,
+                                            retrysecond)
                 return False
             else:
                 logger.info(
                     f"Message sent: app_name:{self.app_name} action:{action} data: {data} to: {to_user}"
                 )
                 time.sleep(1)
                 self.last_sended = time.time()
@@ -490,24 +493,26 @@
                         transactions[transaction]["transaction"])
                     if not transactions[transaction]["transaction"][
                             "data"] == "NP":
                         with contextlib.suppress(json.decoder.JSONDecodeError):
                             transactions[transaction]["transaction"][
                                 "data"] = json.loads(transactions[transaction]
                                                      ["transaction"]["data"])
-                        if not transactions[transaction]["transaction"][
-                                "data"]["app_data"].startswith("split-"):
-                            self.cache.append(
-                                transactions[transaction]["transaction"]
-                                ["signature"]) if not disable_caches else None
+                        with contextlib.suppress(TypeError):
+                            if not transactions[transaction]["transaction"][
+                                    "data"]["app_data"].startswith("split-"):
+                                self.cache.append(
+                                    transactions[transaction]["transaction"]
+                                    ["signature"]
+                                ) if not disable_caches else None
 
-                            SavetoMyTransaction(
-                                the_tx) if not get_all else None
-                            ValidateTransaction(
-                                the_tx) if not get_all else None
+                                SavetoMyTransaction(
+                                    the_tx) if not get_all else None
+                                ValidateTransaction(
+                                    the_tx) if not get_all else None
                     else:
                         SavetoMyTransaction(the_tx) if not get_all else None
                         ValidateTransaction(the_tx) if not get_all else None
                         self.cache.append(
                             transactions[transaction]["transaction"]
                             ["signature"]) if not disable_caches else None
                 elif transactions[transaction]["transaction"][
@@ -532,26 +537,27 @@
                             ["data"] == "NP"):
                             with contextlib.suppress(
                                     json.decoder.JSONDecodeError):
                                 transactions_sended[transaction][
                                     "transaction"]["data"] = json.loads(
                                         transactions_sended[transaction]
                                         ["transaction"]["data"])
-                            if not transactions_sended[transaction][
-                                    "transaction"]["data"][
-                                        "app_data"].startswith("split-"):
-                                self.cache.append(
-                                    transactions_sended[transaction]
-                                    ["transaction"]["signature"]
-                                ) if not disable_caches else None
+                            with contextlib.suppress(TypeError):
+                                if not transactions_sended[transaction][
+                                        "transaction"]["data"][
+                                            "app_data"].startswith("split-"):
+                                    self.cache.append(
+                                        transactions_sended[transaction]
+                                        ["transaction"]["signature"]
+                                    ) if not disable_caches else None
 
-                                SavetoMyTransaction(
-                                    the_tx) if not get_all else None
-                                ValidateTransaction(
-                                    the_tx) if not get_all else None
+                                    SavetoMyTransaction(
+                                        the_tx) if not get_all else None
+                                    ValidateTransaction(
+                                        the_tx) if not get_all else None
                         else:
                             SavetoMyTransaction(
                                 the_tx) if not get_all else None
                             ValidateTransaction(
                                 the_tx) if not get_all else None
                             self.cache.append(
                                 transactions_sended[transaction]["transaction"]
@@ -578,29 +584,30 @@
                             with contextlib.suppress(
                                     json.decoder.JSONDecodeError):
                                 transactions_sended_not_validated[transaction][
                                     "transaction"]["data"] = json.loads(
                                         transactions_sended_not_validated[
                                             transaction]["transaction"]
                                         ["data"])
-                            if not transactions_sended_not_validated[
-                                    transaction]["transaction"]["data"][
-                                        "app_data"].startswith("split-"):
-                                self.cache.append(
-                                    transactions_sended_not_validated[
-                                        transaction]["transaction"]
-                                    ["signature"]
-                                ) if not disable_caches else None
+                            with contextlib.suppress(TypeError):
+                                if not transactions_sended_not_validated[
+                                        transaction]["transaction"]["data"][
+                                            "app_data"].startswith("split-"):
+                                    self.cache.append(
+                                        transactions_sended_not_validated[
+                                            transaction]["transaction"]
+                                        ["signature"]
+                                    ) if not disable_caches else None
 
-                                split_not_validated.append(
-                                    transactions_sended_not_validated[
-                                        transaction]["transaction"]
-                                    ["signature"])
-                                SavetoMyTransaction(
-                                    the_tx) if not get_all else None
+                                    split_not_validated.append(
+                                        transactions_sended_not_validated[
+                                            transaction]["transaction"]
+                                        ["signature"])
+                                    SavetoMyTransaction(
+                                        the_tx) if not get_all else None
                         else:
                             SavetoMyTransaction(
                                 the_tx) if not get_all else None
                             self.cache.append(
                                 transactions_sended_not_validated[transaction]
                                 ["transaction"]
                                 ["signature"]) if not disable_caches else None
```

### Comparing `naruno-0.60.2/naruno/blockchain/block/block_main.py` & `naruno-0.60.3/naruno/blockchain/block/block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/blocks_hash.py` & `naruno-0.60.3/naruno/blockchain/block/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.60.3/naruno/blockchain/block/change_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/create_block.py` & `naruno-0.60.3/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/get_block.py` & `naruno-0.60.3/naruno/blockchain/block/get_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.60.3/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.60.3/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/hash/accounts_hash.py` & `naruno-0.60.3/naruno/blockchain/block/hash/accounts_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.60.3/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.60.3/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.60.3/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/just_one_tx.py` & `naruno-0.60.3/naruno/blockchain/block/just_one_tx.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/max_data_size.py` & `naruno-0.60.3/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/max_tx_number.py` & `naruno-0.60.3/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/save_block.py` & `naruno-0.60.3/naruno/blockchain/block/save_block.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,290 +34,212 @@
 serial_testers = [
     "2844854d58334e66540097479439be65e0aa4efc",
     "7f53b1bb58032bc0212b8f1abc9fbb6510a16671",
     "8e0a8f580c43dd2b33d62afbfa514b3cbe262061",
     "0022b1a2c50249be6e760be4f3c2c0d9ed467fc3",
     "65abccda166c7f730376a0c15753942392b21d73",
     "c8ecc03e12e9b1975851ac4bac2159e2210c8402",
-
     "80df451fc2653ee4bb85230f2e9800f07527f778",
-
     "f51b88c59db9cac5e933ac8827bd7f10dc543ae3",
-
     "59bd07543a4aaf2e45a9b8b8f29e372de79d47ce",
-
     "7c697b908b77064d70ef4526a658eb9e2e5a9ee6",
-
     "5764cfd11addb37353c7e159a909e90f1de3c5e9",
-
     "e4ec7b50fe90c117ad37b41b01e5059c1c903ce0",
-
     "fd29f1d5b573796d4bd614c3c52738bbfcc5e340",
-
     "b01a9cdd81bad9cefc43733b5146c2a1b1b4dd6c",
-
     "c8dca04b72bc69b4e3ac3067f6d0174f2dcfe680",
-
     "755089190444e4af31aa4641c8d6e03254014b11",
-
     "68b777ebba65e8ab4af3d6bdb0837abc3ae177d9",
-
     "f641261d1527cade37371957afe04eb2d7e6b471",
-
     "7c7bf0510137fc29f09f2df2e38a45146567df7d",
-
     "1aa29b64943c955e2c1dfa5b734a5c617cdd4a8d",
-
     "d865a195c73d06313d72dcf3579d9920e4b4584b",
-
     "60d4357a85a2113467860455e5ccdb7b127a97dd",
-
     "bd679bd9bf83a00766cb0ae29ab0f9aae7f2d73e",
-
     "2b0d9405d9f8a6c658608dd2255528e0a12f4f16",
-
     "884aaa97c4121bbee5a3d79a312900c090bbbff5",
-
     "29b7ab3aeafedef1c3ad81323473ade7877ad698",
-
     "cc9ac91de747f657c1a2b6c9e071cf53833e357d",
-
     "52185af45f343636dcb2e88843a12e24aad3be9c",
-
     "73b02b4a4715c96eec46823b5fb1e1f401dcd1cb",
-
     "4b59062c6d3840a023fdc8aaa5c0a87f05aab62e",
-
     "8ed1aea1b9ebe2e4cfc9b9b03b53ac892bc63119",
-
     "6c9189efacd2c9b2bdbde200b5bae8cb022a9bd7",
-
     "ddf8a128b477f00167367f8d7e7816412c81feae",
-
     "58f9bda368fb61dcdc177af0daea1eb46b53ed5",
-
     "16bdffb8012f79c7818ee67054994fe128012cc4",
     "eae2c4f8ff12c10e0a3b0c8a5a677a2b9e50309e",
-
     "fcd23380b3ef500b205424c435837b8367e7e0a6",
     "1e65a85a0716c53fca521d7cbf9096d2f9a18ab4",
-
     "c010bb210da143a01d0d2ae914fd033c549e33c7",
-
     "1c8d4b723b67165847e3b11e3029748e6ebf5139",
-
     "b2345bda4ff22d0c51f27c4d470c63f63730ac77",
-
     "17008875dc5a6c9102a5c2aa1e03249d7f576237",
-
     "71fa49f318437ac5f3a72f6048f0f15dff974cce",
-
     "095fef5e67fad85a0cd40517d46316741f7b7e5c",
-
     "b1956275dadc0e91952b7991d692457c8699c73b",
     "d5a262b8719540b95e742838abf50a67c3972d82",
-
     "e493b8b92c3271af170064bcf42f706272bce631",
-
     "51a5563ecd11b49c19f2f11d3bb8ac1a0f75e4ea",
-
     "1243e02aa77ca080edd879b031fee5d2858ef248",
-
     "069f4682619925d4862c9597ac501c67b39e0608",
-
     "bdf78ffeed1cb2e37e2cd1e444ee6cf552b62e40",
-
     "6b31a60a3a73aa7b80b5a63fed63fcfdb85ee863",
-
     "a426fad6820c77d5d0c730c7f13bd1d668e17b45",
-
     "90f248e2d1143fd3995ebc2de856115d305ee46c",
-
     "6c3b4fd7a8f619194f13bacfb83bbeee91bf1ce0",
-
     "746c2ed9eae6210533854c217586b27330f80417",
-
     "329506e24ef995ec3e2759242ce52033a41be14a",
-
     "a02a508328575e913a09a9dd28a11145e62c9865",
-
     "9abb7a1219a20d6e55f8e4d5ae6ec0e89c2b4770",
-
     "1bb50e042ce653ec8501f47d712dc1ded0c6374a",
-
     "d3cbae4148f79953f5b86c8ab5c70282cbf398b7",
 
 
 
 
-
 ]
 individuals = [
+    "df78cbab1f97ec8115ad2d2a48f7e5cbbe754bb8",
     "55de207a538855b4da2d60325e8afadc3b3caa04",
-
-
     "86e9a2454e2d2bd12f56ef37e39d026608013e72",
-
-
     "2f58be5d152490affa05a7b0fd3cef8c195dae6d",
-
-
     "a26536e07f3c2a850fb2b63cbe99d84589674634",
-
-
     "0be5c9cd8bf68cafeec3a2d5d51678923780d3ff",
-
-
     "82d87a6bfd279d30ad4894912eae2efacd4d46d6",
-
-
     "f6e4955a8077ae5ed7d95014b41f22dcee6c0d76",
-
-
     "73672aafc1890fc18d9b88105380b396eca799a5",
-
-
     "83a15e056f98305418ee9ea26caf664c3d020040",
-
-
     "b1df8deda30d4f88cb905ecd57ed0fc7f2021d00",
-
-
     "ec29c2e01987796a3677da2e3a9b4a098b93b89a",
-
-
     "887af3d44bfe39005b4cc480c2b03a11c2fb8b63",
-
-
     "17d3d3e20bd84ddf6e3ed85fa693c12654f174eb",
-
-
     "1da75d769ab3604abc04763d20dc3f70bf1c69b8",
-
-
     "d7eee170a14b99e37a3e3fc6d375d1d28bddf62b",
-
-
     "d7f20b7990cc593e248f1d0dd31dd7a235a40d9a",
-
-
     "75f7e0e090834c959f6538b1a4c80f03be410bdd",
-
-
     "d37cb2c0df30965f2bc12cea040386e70e32402b",
-
-
     "0af54b3f47fc1577688e7c2c227672f610cad292",
-
-
     "96bb7bac1af450ea0c17300ea4f61b1cd0b88b6d",
-
-
     "709bf017a48d2f02bb5d5d8d205ccf39d8205b4a",
-
-
     "5b943d77a8b7e66aa60b98a2197f2197db4f464b",
-
-
     "bba1e2f5871c02b130416229c02dd54fc404cd21",
-
-
     "dcf715a42784bfedf009b515ada46c1946a3339b",
-
-
     "0af54b3f47fc1577688e7c2c227672f610cad292",
-
-
     "0af54b3f47fc1577688e7c2c227672f610cad292",
-
-
     "0af54b3f47fc1577688e7c2c227672f610cad292",
-
-
     "cbdeeab5577f6f8693e571494e61dc0f356d9d09",
-
-
     "09375da881e7d546b8520a7e39160fc05eb60ce1",
-
-
     "b3232a5ed1d57c339fb3a258be40c51e221b48af",
-
-
     "7be509d428fc848485683a599cc4bbd958bd6df3",
-
-
     "2b76e7031353e9cbf62e2d259b54b98673f997c9",
-
-
     "614deef9abde68a0dab39fe5ee9f9cb2f9e8773a",
-
-
     "44281e3b85497d41d8c99f3b8b66a3e88e354ca1",
-
-
     "5db89649f397be7d3787cfca2e9f39245ef5f8e1",
-
-
     "b3e6e03b6c3f6ea8989177d23a9a055e2a05659b",
-
-
     "bc512bab30167fe84c84208be8759bf9839d7815",
-
-
     "138c27b39d5789319aa9a0c00262cb5360d146d0",
-
-
     "0dbe3d640ee1632b222154197a23319870f3d12d",
-
-
     "4a1b3198530952ee851722b105770ef21c59e472",
-
-
     "541cb5cc142e94aed187f83ee0d91a1470db3023",
-
-
     "caefad8f89b701d8087945780ad24fe0f993ae2f",
-
-
     "8f571575a492ef27f0fe02916303ea867f50876d",
-
-
     "508c9565bac49d318eb5c67f6e6e0354acbc4edf",
-
-
     "c7b71bd5100d2081de69497776064589e98c4fe1",
-
-
     "c58b9d12474108867f4a0924f4c521119a57d62f",
-
-
     "0d435e7fb86a46f4849a4eb41f683ab322f03d6b",
-
-
     "2E6A70110890b7A46F7857E2866023043CeF4680",
-
-
     "078e6dd15b33411462d284baf4c901cfd828558c",
-
-
     "88b73c67bf3aab4764d627cc9aa1150c6ae97794",
+    "450305d3bb1a0fd7343824f136177220d436c046",
+    "e7b72ca5af68bc5b8ddd98e4187c68efcfbec5cd",
+    "b356e5edd49015dad8b69c607130588512380f24",
+    "6af5cba8cf348e92717ba1e08132e19220d2239d",
+    "78b830a53b4169f815da314d7dec8bbd935eab1e",
+    "d2bbee821194b41733a9aac650274690c11923c6",
+    "21d81b6bf3e4a6f693dfbcbeff5ba0af69130939",
+    "88f4a4ace0afb7621c6e33042bdc3674c37a5b87",
+    "f2e63a212a1d318f428a67eaac537a33bf9fa3ee",
+    "3e9ec4425b3d40bb0fbe630ce6353922fc58d174",
+    "899de6fc19d9e34beab208753fffb71fb4e4d52c",
+    "f2e63a212a1d318f428a67eaac537a33bf9fa3ee",
+    "c3dec99a1e27d739e25102e528a673dc9efd3217",
+    "d851fbd6e38c4e9f91be7768586765ce6cf1e3ac",
+    "37f7bfc9c0b7cf67a8cb8e3e757f3be00505df6f",
+    "ca5f6b56a4ddda561618b4a1460040ba2089d6d0",
+    "a517e581e265b6690ef1d58331f685df9276e7e4",
+    "f9ac49630d4e8319cb860e1492154585cc7603ce",
+    "1353f11e29fecd0f023ffbad20e13fbc8dbcc417",
+    "2cc4abe152c4b6a2a5108e76e2895656e82c33dc",
+    "c42e8c1d91de134c9e868877f495bbe2a2f0a2c3",
+    "9872f526e450a21782cc9db8b18867dc5a26b93a",
+    "73a4a4a4905bb4352633c49ec8641f0e6555c888",
+    "33e5a77ccef17133d0a87522cafca3c6cf9d4512",
+    "79948de58a4265e58199489176730ebe121c6faa",
+    "490fcf6651419d2a14d6f7ada52ac2bae51f9247",
+    "d2761b3f2a80e7c854a31088f5a4c48e0c30f630",
+    "198796aeb4b896d43a6b1bc82597349de6a231cc",
+    "078166eb3a997091b65f4fb25f9e434b9d13b7f3",
+    "97d46be7a5e281e7bb71ac8ef1ee0eeca716a8af",
+    "0e4004f212eb9b38443cdafa37d8a41aaa06da46",
+    "29dd1a158ab266ebae6f75e1a09c676f2fef0726",
+    "b5274cc8e238f855687d15efd1863d47aed38fdd",
+    "948812de96640a783dcb2696c9e04570382f24c3",
+    "1e43c76cdded5255f95a0ee0f886133c5cb953cf",
+    "813a3637cf67613b4755c0e849ea05b760f83c3a",
+    "2d9ac3d72feeafa2f86b4ffb57d4c8c33993d57",
+    "49b9529a5eb35188b9bcc938e8a9bc23052aa4cb",
+    "df7c8bd0bcee84959747547199f8f64af3c71af7",
+    "aaefe424bc7cf62c9ea20a8a111c56fdb7efa05b",
+    "ae431c1971be9d605c150f39454cbcdce0e7ec07",
+    "fe44fb36a82bc177794108d37e97b696ba982257",
+    "2b29e43956530c93be2c90022dfcc0dfff0c6419",
+    "7e8e4798ef5607834522712cf6ebf7f6625a2eed",
+    "fc94dc3d2ee57aea37dee8c6cc66fdef60bef519",
+    "d575221dffadf3d626c53d5e2caea06653d0c5b7",
+    "683b99fb0fc3a5c0e70f97ce16c8c803bb3cf828",
+    "99b9a4552a5484bce18d01dd6e165d497099b754",
+    "2ae08ace0c213cd17d08e9a97798137abaa4bf13",
+    "9039cc13c0fc89ee097fe9f608cf387da3971c8f",
+    "28e368a5cc6b4f3b7f09da5cf16bef1dc25c97b8",
+    "dc0fcf7851f565369c0c616e704ce0af6ecc61db",
+    "0944281ea3c0e5290d2d56547aec447fb823e3f2",
+    "82a347178b62a3203aef15cbad2e6c70a319ba46",
+    "c35a9acc440a980b136c5cf0b8a801b03a97e2f1",
+    "alb78e89d508ea358d32db79c20e444175551d7e",
+    "49b9529a5eb35188b9bcc938e8a9bc23052aa4cb",
+    "6256d81a0d280048c6907f20c2654b0ca027863c",
+    "c6618b1c64fac65fe58f8da8fc75f499b744f55e",
+    "cd02e3d2208b556d1115a2b8f62d2cc27af54389",
+    "ffc5219f0108bf02654f949f18037d68264c42bc",
+    "5ab039bdb7c6dfe57507834874f7494165a1f12b",
+    "af32b70e92506ed2128e0f58f233129d24dc1723",
+    "22974433614765cdc42fc94108dc0a0d5349bc73",
+    "2b0c8c2bc1c725056696c896425e8264fae2760f",
+    "0f5902f6285a9b7723c565d756e89f7a0ba9a3b3",
+    "a94976beb574e53bdc1e86a36f6415067123de86",
+    "9a46fd0899fcaf5fef9e7cd277b1bf1864827d24",
+    "cb9314ad3ecd2cff3f7aa1a1fc04f13c5b026270",
+    "f5647d2072bdfa89b6bd05e7051bf9e57bac5dd2",
+    "8029f657fe71de6c42491c9969f795b4be68fee7",
+    "05c19214daba9aacab274f0c89a93721919d80a1",
 
 
-    "450305d3bb1a0fd7343824f136177220d436c046",
 
 
-    "e7b72ca5af68bc5b8ddd98e4187c68efcfbec5cd",
 ]
 
-specials = ["e087a455c3b35d5022491b380e3e34d68df4ca6c"]
+specials = ["40a175793d9b7082157fd3e1632fc25c9f3f5234"]
 
 special_testers = [
     "d78101e2cb261efab28ee54a0e6d716820a1bab1",
     "40a175793d9b7082157fd3e1632fc25c9f3f5234",
-    "9febe30ed21991fdca2e84d1a42d594c1a02ab36"
+    "9febe30ed21991fdca2e84d1a42d594c1a02ab36",
+    "f687088eff5423f913f03b677f97a9c405f7549a",
+    "c923c646f2d73fcb8f626afacb1a0ade8d98954a"
     ]
 
 
 def SaveBlock(
     block: Block,
     custom_TEMP_BLOCK_PATH=None,
     custom_TEMP_ACCOUNTS_PATH=None,
@@ -344,18 +266,18 @@
         f"Block#{block.sequence_number + block.empty_block_number}:{block.empty_block_number}: {block.dump_json()}"
     )
 
     if block.first_time:
         accounts_list = [Account(block.creator, block.coin_amount)]
         baklava_test_net_users = []
 
-        baklava_test_net_users.extend([Account(i,(2 * block.minumum_transfer_amount) +block.transaction_fee * 100,) for i in serial_testers])
-        baklava_test_net_users.extend([Account(i,(2 * block.minumum_transfer_amount) +block.transaction_fee * 100,) for i in special_testers])
-        baklava_test_net_users.extend([Account(i,(2 * block.minumum_transfer_amount) +block.transaction_fee * 100,) for i in individuals])
-        baklava_test_net_users.extend([Account(i,(10 * block.minumum_transfer_amount) +block.transaction_fee * 100,) for i in specials])
+        baklava_test_net_users.extend([Account(i,(2 * block.minumum_transfer_amount) + block.transaction_fee * 100,) for i in serial_testers])
+        baklava_test_net_users.extend([Account(i,(2 * block.minumum_transfer_amount) + block.transaction_fee * 100,) for i in special_testers])
+        baklava_test_net_users.extend([Account(i,(2 * block.minumum_transfer_amount) + block.transaction_fee * 100,) for i in individuals])
+        baklava_test_net_users.extend([Account(i,(2000 * block.minumum_transfer_amount) + block.transaction_fee * 100,) for i in specials])
 
 
 
         if the_settings()["baklava_users"]:
             accounts_list.extend(baklava_test_net_users)
         SaveAccounts(
             accounts_list,
```

### Comparing `naruno-0.60.2/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.60.3/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/block/shares.py` & `naruno-0.60.3/naruno/blockchain/block/shares.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.60.3/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/cli/main.py` & `naruno-0.60.3/naruno/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 import time
 from getpass import getpass
 
 from naruno.accounts.get_balance import GetBalance
 from naruno.blockchain.block.create_block import CreateBlock
+from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.save_block import SaveBlock
 from naruno.config import MY_TRANSACTION_EXPORT_PATH
 from naruno.consensus.consensus_main import consensus_trigger
 from naruno.lib.backup.naruno_export import naruno_export
 from naruno.lib.backup.naruno_import import naruno_import
 from naruno.lib.export import export_the_transactions
@@ -152,38 +153,57 @@
 
         if choices_input == "cw":
             wallet_create(getpass("Password: "))
 
         if choices_input == "dw" and input("Are you sure ? (y or n): ") == "y":
             delete_current_wallet()
         if choices_input == "sc":
-            block = GetBlock()
+            if not the_settings()["baklava"]:
+                block = GetBlock()
+            else:
+                block = Block("baklava")
             send_tx = send(
                 getpass("Password: "),
                 input("Please write receiver adress: "),
                 amount=input("Coin Amount (ex. 1.0): "),
                 block=block,
             )
+
             if send_tx != False:
-                SavetoMyTransaction(send_tx, sended=True)
-                server.send_transaction(send_tx)
-                SaveBlock(block)
+                    SavetoMyTransaction(send_tx, sended=True)
+                    if not the_settings()["baklava"]:
+                        from naruno.node.server.server import server
+                        if server.Server is None:
+                            print("Please start the node server")
+                            return False
+                        server.send_transaction(send_tx)
+                        SaveBlock(block)
+
         if choices_input == "scd":
-            block = GetBlock()
+            if not the_settings()["baklava"]:
+                block = GetBlock()
+            else:
+                block = Block("baklava")
             send_tx = send(
                 getpass("Password: "),
                 input("Please write receiver adress: "),
                 amount=input("Coin Amount (ex. 1.0): "),
                 data=input("Data: "),
                 block=block,
             )
             if send_tx != False:
-                SavetoMyTransaction(send_tx, sended=True)
-                server.send_transaction(send_tx)
-                SaveBlock(block)
+                    SavetoMyTransaction(send_tx, sended=True)
+                    if not the_settings()["baklava"]:
+                        from naruno.node.server.server import server
+                        if server.Server is None:
+                            print("Please start the node server")
+                            return False
+                        server.send_transaction(send_tx)
+                        SaveBlock(block)
+
         if choices_input == "gb":
             print(GetBalance(wallet_import(-1, 0)))
         if choices_input == "help":
             show_menu()
         if choices_input == "ndstart":
             server(str(input("ip: ")), int(input("port: ")))
         if choices_input == "ndstop":
```

### Comparing `naruno-0.60.2/naruno/config.py` & `naruno-0.60.3/naruno/config.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/consensus_main.py` & `naruno-0.60.3/naruno/consensus/consensus_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/finished/finished_main.py` & `naruno-0.60.3/naruno/consensus/finished/finished_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/finished/transactions/transactions_main.py` & `naruno-0.60.3/naruno/consensus/finished/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.60.3/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.60.3/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.60.3/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/sync/send_block.py` & `naruno-0.60.3/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/sync/send_block_hash.py` & `naruno-0.60.3/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/consensus/sync/sync.py` & `naruno-0.60.3/naruno/consensus/sync/sync.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/POPPINS_LICENCE` & `naruno-0.60.3/naruno/gui/lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Black.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Bold.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Italic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Light.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Medium.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Regular.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Thin.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/images/logo.ico` & `naruno-0.60.3/naruno/gui/lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/images/logo.png` & `naruno-0.60.3/naruno/gui/lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/images/logo_sm_orb_fw.png` & `naruno-0.60.3/naruno/gui/lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/images/logo_w_bc.png` & `naruno-0.60.3/naruno/gui/lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/images/logo_win.ico` & `naruno-0.60.3/naruno/gui/lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/node_screen.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/node_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/operations_screen.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/operations_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/root_screen.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/root_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/settings_screen.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/settings_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/tabnavigation.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/tabnavigation.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/wallet_screen.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/wallet_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/baseclass/welcome_screen.py` & `naruno-0.60.3/naruno/gui/lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/node_screen.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/operations_screen.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/operations_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/root_screen.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/root_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/settings_screen.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/settings_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/tabnavigation.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/wallet_screen.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/lib/libs/kv/welcome_screen.kv` & `naruno-0.60.3/naruno/gui/lib/libs/kv/welcome_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/main.py` & `naruno-0.60.3/naruno/gui/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/gui/popup.py` & `naruno-0.60.3/naruno/gui/popup.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/backup/naruno_export.py` & `naruno-0.60.3/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/backup/naruno_import.py` & `naruno-0.60.3/naruno/lib/backup/naruno_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/clean_up.py` & `naruno-0.60.3/naruno/lib/clean_up.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/config_system.py` & `naruno-0.60.3/naruno/lib/config_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/encryption.py` & `naruno-0.60.3/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/export.py` & `naruno-0.60.3/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/kot.py` & `naruno-0.60.3/naruno/lib/kot.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/log.py` & `naruno-0.60.3/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/mix/merkle_root.py` & `naruno-0.60.3/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/mix/mixlib.py` & `naruno-0.60.3/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/notification.py` & `naruno-0.60.3/naruno/lib/notification.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.60.3/naruno/lib/performance_analyzers/accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/performance_analyzers/block.py` & `naruno-0.60.3/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.60.3/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.60.3/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.60.3/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.60.3/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/perpetualtimer.py` & `naruno-0.60.3/naruno/lib/perpetualtimer.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/qr.py` & `naruno-0.60.3/naruno/lib/qr.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/safety.py` & `naruno-0.60.3/naruno/lib/safety.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/settings_system.py` & `naruno-0.60.3/naruno/lib/settings_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/sign.py` & `naruno-0.60.3/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/status.py` & `naruno-0.60.3/naruno/lib/status.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/lib/verify.py` & `naruno-0.60.3/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/node/client/client.py` & `naruno-0.60.3/naruno/node/client/client.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/node/get_candidate_blocks.py` & `naruno-0.60.3/naruno/node/get_candidate_blocks.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/node/server/server.py` & `naruno-0.60.3/naruno/node/server/server.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/node/unl.py` & `naruno-0.60.3/naruno/node/unl.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/check/check_transaction.py` & `naruno-0.60.3/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/check/datas/check_datas.py` & `naruno-0.60.3/naruno/transactions/check/datas/check_datas.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/check/len/check_len.py` & `naruno-0.60.3/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/check/sign/check_sign.py` & `naruno-0.60.3/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/check/type/check_type.py` & `naruno-0.60.3/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/cleaner.py` & `naruno-0.60.3/naruno/transactions/cleaner.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/get_transaction.py` & `naruno-0.60.3/naruno/transactions/get_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.60.3/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/get_my_transaction.py` & `naruno-0.60.3/naruno/transactions/my_transactions/get_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.60.3/naruno/transactions/my_transactions/get_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/save_my_transaction.py` & `naruno-0.60.3/naruno/transactions/my_transactions/save_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.60.3/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.60.3/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/my_transactions/validate_transaction.py` & `naruno-0.60.3/naruno/transactions/my_transactions/validate_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/pending/delete_pending.py` & `naruno-0.60.3/naruno/transactions/pending/delete_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/pending/get_pending.py` & `naruno-0.60.3/naruno/transactions/pending/get_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/pending/save_pending.py` & `naruno-0.60.3/naruno/transactions/pending/save_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/pending_to_validating.py` & `naruno-0.60.3/naruno/transactions/pending_to_validating.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/print_transactions.py` & `naruno-0.60.3/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/process_the_transaction.py` & `naruno-0.60.3/naruno/transactions/process_the_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/send.py` & `naruno-0.60.3/naruno/transactions/send.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/transactions/transaction.py` & `naruno-0.60.3/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/delete_current_wallet.py` & `naruno-0.60.3/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/math.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/get_saved_wallet.py` & `naruno-0.60.3/naruno/wallet/get_saved_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/print_wallets.py` & `naruno-0.60.3/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/save_wallet_list.py` & `naruno-0.60.3/naruno/wallet/save_wallet_list.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/wallet_create.py` & `naruno-0.60.3/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/wallet_delete.py` & `naruno-0.60.3/naruno/wallet/wallet_delete.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/wallet_import.py` & `naruno-0.60.3/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno/wallet/wallet_selector.py` & `naruno-0.60.3/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/naruno.egg-info/PKG-INFO` & `naruno-0.60.3/naruno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.60.2
+Version: 0.60.3
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.60.2 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.3 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.60.2/naruno.egg-info/SOURCES.txt` & `naruno-0.60.3/naruno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naruno-0.60.2/setup.py` & `naruno-0.60.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.60.2",
+    version="0.60.3",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

