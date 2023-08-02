# Comparing `tmp/ethereum-etl-2.2.1.tar.gz` & `tmp/ethereum-etl-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ethereum-etl-2.2.1.tar", last modified: Tue May  2 13:02:01 2023, max compression
+gzip compressed data, was "dist/ethereum-etl-2.3.0.tar", last modified: Wed Aug  2 12:18:44 2023, max compression
```

## Comparing `ethereum-etl-2.2.1.tar` & `ethereum-etl-2.3.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/blockchainetl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/atomic_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/csv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/blockchainetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/base_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/composite_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/console_item_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/gcs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/kafka_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/multi_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/jobs/exporters/postgres_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/blockchainetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/streaming/postgres_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/streaming/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/streaming/streamer_adapter_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/blockchainetl/streaming/streaming_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereum_etl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/atomic_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_blocks_and_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_receipts_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/export_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/extract_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/extract_csv_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/extract_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/extract_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/extract_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/extract_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/filter_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/get_block_range_for_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/get_block_range_for_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/get_keccak_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/cli/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/csv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/geth_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/receipt_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/token_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/domain/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/enumeration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/enumeration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/enumeration/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/erc20_abi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/executors/batch_work_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/executors/bounded_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/executors/fail_safe_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/ipfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/ipfs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/ipfs/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_all_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_origin_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/export_traces_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/contracts_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/origin_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/tokens_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/exporters/traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/jobs/extract_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/json_rpc_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mainnet_daofork_state_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)   673817 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mainnet_genesis_alloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/block_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/contract_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/geth_trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/origin_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/receipt_log_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/receipt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/token_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/token_transfer_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/mappers/transaction_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/misc/retriable_value_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/providers/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/providers/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/providers/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/eth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/eth_special_trace_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/eth_token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/graph_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/origin_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/trace_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/service/trace_status_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/ethereumetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/eth_item_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/eth_item_timestamp_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/eth_streamer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/item_exporter_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/streaming/postgres_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/thread_local_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/ethereumetl/web3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/tests/ethereumetl/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/mock_batch_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/mock_ipfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/mock_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_origin_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/job/test_extract_token_transfers_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/tests/ethereumetl/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70321 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/service/test_eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/service/test_eth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/service/test_token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/ethereumetl/test_progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:02:01.000000 ethereum-etl-2.2.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 13:01:59.000000 ethereum-etl-2.2.1/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/blockchainetl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/atomic_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/csv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/blockchainetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/base_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/composite_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/console_item_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/composite_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/list_field_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/simple_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/gcs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/in_memory_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/kafka_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/kinesis_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/multi_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/jobs/exporters/postgres_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/blockchainetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/streaming/postgres_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/streaming/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/streaming/streamer_adapter_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/blockchainetl/streaming/streaming_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereum_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/atomic_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_blocks_and_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_receipts_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/export_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/extract_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/extract_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/extract_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/extract_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/extract_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/extract_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/filter_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/get_block_range_for_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/get_block_range_for_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/get_keccak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/cli/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/csv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/geth_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/receipt_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/token_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/domain/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/enumeration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/enumeration/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/erc20_abi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/executors/batch_work_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/executors/bounded_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/executors/fail_safe_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/ipfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/ipfs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/ipfs/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_all_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_origin_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/export_traces_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/contracts_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/geth_traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/origin_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/token_transfers_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/tokens_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/exporters/traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/jobs/extract_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/json_rpc_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mainnet_daofork_state_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   673817 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mainnet_genesis_alloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/block_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/contract_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/geth_trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/origin_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/receipt_log_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/receipt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/token_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/token_transfer_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/mappers/transaction_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/misc/retriable_value_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/providers/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/providers/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/providers/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/eth_special_trace_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/eth_token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/origin_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/trace_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/service/trace_status_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/ethereumetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/eth_item_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/eth_item_timestamp_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/eth_streamer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/item_exporter_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/streaming/postgres_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/thread_local_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/ethereumetl/web3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/tests/ethereumetl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/mock_batch_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/mock_ipfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/mock_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_origin_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/job/test_extract_token_transfers_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/tests/ethereumetl/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70321 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/service/test_eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/service/test_eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/service/test_token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/ethereumetl/test_progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:18:44.000000 ethereum-etl-2.3.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-02 12:18:43.000000 ethereum-etl-2.3.0/tests/resources/__init__.py
```

### Comparing `ethereum-etl-2.2.1/PKG-INFO` & `ethereum-etl-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereum-etl
-Version: 2.2.1
+Version: 2.3.0
 Summary: Tools for exporting Ethereum blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/ethereum-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/ethereum-etl/issues
 Project-URL: Chat, https://gitter.im/ethereum-etl/Lobby
```

### Comparing `ethereum-etl-2.2.1/README.md` & `ethereum-etl-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/atomic_counter.py` & `ethereum-etl-2.3.0/blockchainetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/csv_utils.py` & `ethereum-etl-2.3.0/blockchainetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/exporters.py` & `ethereum-etl-2.3.0/blockchainetl/exporters.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/file_utils.py` & `ethereum-etl-2.3.0/blockchainetl/file_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/base_job.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/composite_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/composite_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/console_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/console_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/composite_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/list_field_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/simple_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/gcs_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/gcs_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/in_memory_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/kafka_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/kafka_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/kinesis_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/multi_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/multi_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/jobs/exporters/postgres_item_exporter.py` & `ethereum-etl-2.3.0/blockchainetl/jobs/exporters/postgres_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/streaming/__init__.py` & `ethereum-etl-2.3.0/blockchainetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/streaming/postgres_utils.py` & `ethereum-etl-2.3.0/blockchainetl/streaming/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/blockchainetl/streaming/streamer.py` & `ethereum-etl-2.3.0/blockchainetl/streaming/streamer.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereum_etl.egg-info/PKG-INFO` & `ethereum-etl-2.3.0/ethereum_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereum-etl
-Version: 2.2.1
+Version: 2.3.0
 Summary: Tools for exporting Ethereum blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/ethereum-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/ethereum-etl/issues
 Project-URL: Chat, https://gitter.im/ethereum-etl/Lobby
```

### Comparing `ethereum-etl-2.2.1/ethereum_etl.egg-info/SOURCES.txt` & `ethereum-etl-2.3.0/ethereum_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/__main__.py` & `ethereum-etl-2.3.0/ethereumetl/__main__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/atomic_counter.py` & `ethereum-etl-2.3.0/ethereumetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from ethereumetl.cli.get_block_range_for_date import get_block_range_for_date
 from ethereumetl.cli.get_block_range_for_timestamps import get_block_range_for_timestamps
 from ethereumetl.cli.get_keccak_hash import get_keccak_hash
 from ethereumetl.cli.stream import stream
 
 
 @click.group()
-@click.version_option(version='2.1.1')
+@click.version_option(version='2.3.0')
 @click.pass_context
 def cli(ctx):
     pass
 
 
 # export
 cli.add_command(export_all, "export_all")
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_all.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_all.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_blocks_and_transactions.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_blocks_and_transactions.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_contracts.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_contracts.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_geth_traces.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_geth_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_origin.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_receipts_and_logs.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_receipts_and_logs.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_token_transfers.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_token_transfers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_tokens.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_tokens.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/export_traces.py` & `ethereum-etl-2.3.0/ethereumetl/cli/export_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/extract_contracts.py` & `ethereum-etl-2.3.0/ethereumetl/cli/extract_contracts.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/extract_csv_column.py` & `ethereum-etl-2.3.0/ethereumetl/cli/extract_csv_column.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/extract_field.py` & `ethereum-etl-2.3.0/ethereumetl/cli/extract_field.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/extract_geth_traces.py` & `ethereum-etl-2.3.0/ethereumetl/cli/extract_geth_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/extract_token_transfers.py` & `ethereum-etl-2.3.0/ethereumetl/cli/extract_token_transfers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/extract_tokens.py` & `ethereum-etl-2.3.0/ethereumetl/cli/extract_tokens.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/filter_items.py` & `ethereum-etl-2.3.0/ethereumetl/cli/filter_items.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/get_block_range_for_date.py` & `ethereum-etl-2.3.0/ethereumetl/cli/get_block_range_for_date.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/get_block_range_for_timestamps.py` & `ethereum-etl-2.3.0/ethereumetl/cli/get_block_range_for_timestamps.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/get_keccak_hash.py` & `ethereum-etl-2.3.0/ethereumetl/cli/get_keccak_hash.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/cli/stream.py` & `ethereum-etl-2.3.0/ethereumetl/cli/stream.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/csv_utils.py` & `ethereum-etl-2.3.0/ethereumetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/block.py` & `ethereum-etl-2.3.0/ethereumetl/domain/block.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/contract.py` & `ethereum-etl-2.3.0/ethereumetl/domain/contract.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/geth_trace.py` & `ethereum-etl-2.3.0/ethereumetl/domain/geth_trace.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/origin.py` & `ethereum-etl-2.3.0/ethereumetl/domain/origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/receipt.py` & `ethereum-etl-2.3.0/ethereumetl/domain/receipt_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
-class EthReceipt(object):
+class EthReceiptLog(object):
     def __init__(self):
+        self.log_index = None
         self.transaction_hash = None
         self.transaction_index = None
         self.block_hash = None
         self.block_number = None
-        self.cumulative_gas_used = None
-        self.gas_used = None
-        self.contract_address = None
-        self.logs = []
-        self.root = None
-        self.status = None
-        self.effective_gas_price = None
+        self.address = None
+        self.data = None
+        self.topics = []
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/receipt_log.py` & `ethereum-etl-2.3.0/ethereumetl/domain/token.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
-class EthReceiptLog(object):
+class EthToken(object):
     def __init__(self):
-        self.log_index = None
-        self.transaction_hash = None
-        self.transaction_index = None
-        self.block_hash = None
-        self.block_number = None
         self.address = None
-        self.data = None
-        self.topics = []
+        self.symbol = None
+        self.name = None
+        self.decimals = None
+        self.total_supply = None
+        self.block_number = None
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/token.py` & `ethereum-etl-2.3.0/ethereumetl/domain/token_transfer.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
-class EthToken(object):
+class EthTokenTransfer(object):
     def __init__(self):
-        self.address = None
-        self.symbol = None
-        self.name = None
-        self.decimals = None
-        self.total_supply = None
+        self.token_address = None
+        self.from_address = None
+        self.to_address = None
+        self.value = None
+        self.transaction_hash = None
+        self.log_index = None
         self.block_number = None
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/token_transfer.py` & `ethereum-etl-2.3.0/ethereumetl/misc/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,18 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-
-class EthTokenTransfer(object):
-    def __init__(self):
-        self.token_address = None
-        self.from_address = None
-        self.to_address = None
-        self.value = None
-        self.transaction_hash = None
-        self.log_index = None
-        self.block_number = None
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/trace.py` & `ethereum-etl-2.3.0/ethereumetl/domain/trace.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/domain/transaction.py` & `ethereum-etl-2.3.0/ethereumetl/domain/transaction.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/erc20_abi.py` & `ethereum-etl-2.3.0/ethereumetl/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/executors/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/executors/batch_work_executor.py` & `ethereum-etl-2.3.0/ethereumetl/executors/batch_work_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/executors/bounded_executor.py` & `ethereum-etl-2.3.0/ethereumetl/executors/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/executors/fail_safe_executor.py` & `ethereum-etl-2.3.0/ethereumetl/executors/fail_safe_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/exporters.py` & `ethereum-etl-2.3.0/ethereumetl/exporters.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/ipfs/client.py` & `ethereum-etl-2.3.0/ethereumetl/ipfs/client.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/ipfs/origin.py` & `ethereum-etl-2.3.0/ethereumetl/ipfs/origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_all_common.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_all_common.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_blocks_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_contracts_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_geth_traces_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_origin_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_origin_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_receipts_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_token_transfers_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_tokens_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/export_traces_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/export_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/contracts_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/contracts_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/geth_traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/origin_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/origin_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,20 @@
     'block_hash',
     'block_number',
     'cumulative_gas_used',
     'gas_used',
     'contract_address',
     'root',
     'status',
-    'effective_gas_price'
+    'effective_gas_price',
+    'l1_fee',
+    'l1_gas_used',
+    'l1_gas_price',
+    'l1_fee_scalar'
+    
 ]
 
 LOG_FIELDS_TO_EXPORT = [
     'log_index',
     'transaction_hash',
     'transaction_index',
     'block_hash',
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/token_transfers_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/tokens_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/tokens_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/exporters/traces_item_exporter.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/exporters/traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/extract_contracts_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/extract_geth_traces_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/extract_token_transfers_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/jobs/extract_tokens_job.py` & `ethereum-etl-2.3.0/ethereumetl/jobs/extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/json_rpc_requests.py` & `ethereum-etl-2.3.0/ethereumetl/json_rpc_requests.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mainnet_daofork_state_changes.py` & `ethereum-etl-2.3.0/ethereumetl/mainnet_daofork_state_changes.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mainnet_genesis_alloc.py` & `ethereum-etl-2.3.0/ethereumetl/mainnet_genesis_alloc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/block_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/block_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/contract_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/contract_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/geth_trace_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/geth_trace_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/origin_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/origin_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/receipt_log_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/receipt_log_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/token_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/token_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/token_transfer_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/token_transfer_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/trace_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/trace_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/mappers/transaction_mapper.py` & `ethereum-etl-2.3.0/ethereumetl/mappers/transaction_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/misc/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/providers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/misc_utils.py` & `ethereum-etl-2.3.0/ethereumetl/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/progress_logger.py` & `ethereum-etl-2.3.0/ethereumetl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/providers/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/providers/auto.py` & `ethereum-etl-2.3.0/ethereumetl/providers/auto.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/providers/ipc.py` & `ethereum-etl-2.3.0/ethereumetl/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/providers/rpc.py` & `ethereum-etl-2.3.0/ethereumetl/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/__init__.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/eth_contract_service.py` & `ethereum-etl-2.3.0/ethereumetl/service/eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/eth_service.py` & `ethereum-etl-2.3.0/ethereumetl/service/eth_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         end_datetime = datetime.combine(date, datetime.max.time().replace(tzinfo=timezone.utc))
         return self.get_block_range_for_timestamps(start_datetime.timestamp(), end_datetime.timestamp())
 
     def get_block_range_for_timestamps(self, start_timestamp, end_timestamp):
         start_timestamp = int(start_timestamp)
         end_timestamp = int(end_timestamp)
         if start_timestamp > end_timestamp:
-            raise ValueError('start_timestamp must be greater or equal to end_timestamp')
+            raise ValueError('start_timestamp must be lesser than end_timestamp')
 
         try:
             start_block_bounds = self._graph_operations.get_bounds_for_y_coordinate(start_timestamp)
         except OutOfBoundsError:
             start_block_bounds = (0, 0)
 
         try:
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/eth_special_trace_service.py` & `ethereum-etl-2.3.0/ethereumetl/service/eth_special_trace_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/eth_token_service.py` & `ethereum-etl-2.3.0/ethereumetl/service/eth_token_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/graph_operations.py` & `ethereum-etl-2.3.0/ethereumetl/service/graph_operations.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/origin_extractor.py` & `ethereum-etl-2.3.0/ethereumetl/service/origin_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/token_transfer_extractor.py` & `ethereum-etl-2.3.0/ethereumetl/service/token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/trace_id_calculator.py` & `ethereum-etl-2.3.0/ethereumetl/service/trace_id_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/service/trace_status_calculator.py` & `ethereum-etl-2.3.0/ethereumetl/service/trace_status_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/__init__.py` & `ethereum-etl-2.3.0/tests/ethereumetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/enrich.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/enrich.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,20 @@
         ],
         right_fields=[
             ('cumulative_gas_used', 'receipt_cumulative_gas_used'),
             ('gas_used', 'receipt_gas_used'),
             ('contract_address', 'receipt_contract_address'),
             ('root', 'receipt_root'),
             ('status', 'receipt_status'),
-            ('effective_gas_price', 'receipt_effective_gas_price')
+            ('effective_gas_price', 'receipt_effective_gas_price'),
+            ('l1_fee', 'receipt_l1_fee'),
+            ('l1_gas_used', 'receipt_l1_gas_used'),
+            ('l1_gas_price', 'receipt_l1_gas_price'),
+            ('l1_fee_scalar', 'receipt_l1_fee_scalar')
+
         ]))
 
     if len(result) != len(transactions):
         raise ValueError('The number of transactions is wrong ' + str(result))
 
     return result
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/eth_item_id_calculator.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/eth_item_id_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/eth_item_timestamp_calculator.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/eth_item_timestamp_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/eth_streamer_adapter.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/eth_streamer_adapter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/item_exporter_creator.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/item_exporter_creator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/streaming/postgres_tables.py` & `ethereum-etl-2.3.0/ethereumetl/streaming/postgres_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from sqlalchemy import Table, Column, Integer, BigInteger, Boolean, String, Numeric, \
-    MetaData, PrimaryKeyConstraint, VARCHAR, TIMESTAMP
+    MetaData, PrimaryKeyConstraint, VARCHAR, TIMESTAMP, Float
 from sqlalchemy.dialects.postgresql import ARRAY
 
 metadata = MetaData()
 
 # SQL schema is here https://github.com/blockchain-etl/ethereum-etl-postgres/tree/master/schema
 
 BLOCKS = Table(
@@ -70,14 +70,18 @@
     Column('block_timestamp', TIMESTAMP),
     Column('block_number', BigInteger),
     Column('block_hash', String),
     Column('max_fee_per_gas', BigInteger),
     Column('max_priority_fee_per_gas', BigInteger),
     Column('transaction_type', BigInteger),
     Column('receipt_effective_gas_price', BigInteger),
+    Column('receipt_l1_fee', BigInteger),
+    Column('receipt_l1_gas_used', BigInteger),
+    Column('receipt_l1_gas_price', BigInteger),
+    Column('receipt_l1_fee_scalar', Float),
 )
 
 LOGS = Table(
     'logs', metadata,
     Column('log_index', BigInteger, primary_key=True),
     Column('transaction_hash', String, primary_key=True),
     Column('transaction_index', BigInteger),
```

### Comparing `ethereum-etl-2.2.1/ethereumetl/thread_local_proxy.py` & `ethereum-etl-2.3.0/ethereumetl/thread_local_proxy.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/utils.py` & `ethereum-etl-2.3.0/ethereumetl/utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/ethereumetl/web3_utils.py` & `ethereum-etl-2.3.0/ethereumetl/web3_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/setup.py` & `ethereum-etl-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 long_description = read('README.md') if os.path.isfile("README.md") else ""
 
 setup(
     name='ethereum-etl',
-    version='2.2.1',
+    version='2.3.0',
     author='Evgeny Medvedev',
     author_email='evge.medvedev@gmail.com',
     description='Tools for exporting Ethereum blockchain data to CSV or JSON',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blockchain-etl/ethereum-etl',
     packages=find_packages(exclude=['schemas', 'tests']),
@@ -34,14 +34,15 @@
         'web3>=5.29,<6',
         'eth-utils==1.10',
         'eth-abi>=2.2.0,<3.0.0',
         # TODO: This has to be removed when "ModuleNotFoundError: No module named 'eth_utils.toolz'" is fixed at eth-abi
         'python-dateutil>=2.8.0,<3',
         'click>=8.0.4,<9',
         'ethereum-dasm==0.1.4',
+        'urllib3<2',
         'base58',
         'requests'
     ],
     extras_require={
         'streaming': [
             'timeout-decorator==0.4.1',
             'google-cloud-pubsub==2.13.0',
```

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/__init__.py` & `ethereum-etl-2.3.0/tests/ethereumetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/__init__.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/helpers.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/helpers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/mock_batch_web3_provider.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/mock_batch_web3_provider.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/mock_web3_provider.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/mock_web3_provider.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_blocks_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_contracts_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_geth_traces_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_origin_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_origin_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_receipts_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_token_transfers_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_tokens_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_export_traces_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_export_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_extract_geth_traces_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/job/test_extract_token_transfers_job.py` & `ethereum-etl-2.3.0/tests/ethereumetl/job/test_extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/service/test_eth_contract_service.py` & `ethereum-etl-2.3.0/tests/ethereumetl/service/test_eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/service/test_eth_service.py` & `ethereum-etl-2.3.0/tests/ethereumetl/service/test_eth_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/service/test_token_transfer_extractor.py` & `ethereum-etl-2.3.0/tests/ethereumetl/service/test_token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/ethereumetl/test_progress_logger.py` & `ethereum-etl-2.3.0/tests/ethereumetl/test_progress_logger.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.2.1/tests/resources/__init__.py` & `ethereum-etl-2.3.0/tests/resources/__init__.py`

 * *Files identical despite different names*

