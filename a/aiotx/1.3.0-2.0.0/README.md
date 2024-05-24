# Comparing `tmp/aiotx-1.3.0.tar.gz` & `tmp/aiotx-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-1.3.0.tar", last modified: Wed May 22 20:04:49 2024, max compression
+gzip compressed data, was "aiotx-2.0.0.tar", last modified: Thu May 23 05:12:57 2024, max compression
```

## Comparing `aiotx-1.3.0.tar` & `aiotx-2.0.0.tar`

### file list

```diff
@@ -1,162 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.662374 aiotx-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/mysql_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-22 20:04:43.000000 aiotx-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-22 20:04:43.000000 aiotx-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-22 20:04:43.000000 aiotx-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-22 20:04:43.000000 aiotx-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-22 20:04:43.000000 aiotx-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-22 20:04:49.662374 aiotx-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-22 20:04:43.000000 aiotx-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/_utxo_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/utils/bep20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/utils/erc20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.662374 aiotx-1.3.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.606374 aiotx-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/docs/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.606374 aiotx-1.3.0/docs/clients/evm_client/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_contract_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_contract_decimals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_gas_price.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_last_block.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_transaction_count.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/send_token.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.606374 aiotx-1.3.0/docs/clients/tron_client/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/docs/clients/utxo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/estimate_smart_fee.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/from_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_last_block_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/import_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/send_bulk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/to_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/monitoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/eth_block_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/ltc_block_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 20:04:43.000000 aiotx-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 20:04:43.000000 aiotx-1.3.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-22 20:04:43.000000 aiotx-1.3.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 20:04:49.662374 aiotx-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-22 20:04:43.000000 aiotx-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.614374 aiotx-1.3.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.626374 aiotx-1.3.0/tests/fixtures/cassettes/btc/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 10852371 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 21958019 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.654374 aiotx-1.3.0/tests/fixtures/cassettes/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/fixtures/cassettes/ltc/
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42576 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34448 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/networks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/tests/test_evm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_evm/test_bsc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_evm/test_eth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/test_eth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/test_eth_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/test_eth_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/tests/test_utxo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_utxo/test_btc/
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_utxo/test_ltc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_ltc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.206153 aiotx-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.142153 aiotx-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.146153 aiotx-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 05:12:51.000000 aiotx-2.0.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-23 05:12:51.000000 aiotx-2.0.0/.github/workflows/mysql_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 05:12:51.000000 aiotx-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-23 05:12:51.000000 aiotx-2.0.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 05:12:51.000000 aiotx-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-23 05:12:51.000000 aiotx-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-23 05:12:51.000000 aiotx-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-23 05:12:51.000000 aiotx-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 05:12:51.000000 aiotx-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 05:12:51.000000 aiotx-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-23 05:12:57.206153 aiotx-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-23 05:12:51.000000 aiotx-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.146153 aiotx-2.0.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.150153 aiotx-2.0.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/clients/_utxo_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.150153 aiotx-2.0.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.150153 aiotx-2.0.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-23 05:12:51.000000 aiotx-2.0.0/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.206153 aiotx-2.0.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-23 05:12:57.000000 aiotx-2.0.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-23 05:12:57.000000 aiotx-2.0.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:12:57.000000 aiotx-2.0.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 05:12:57.000000 aiotx-2.0.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 05:12:57.000000 aiotx-2.0.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.150153 aiotx-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.142153 aiotx-2.0.0/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.150153 aiotx-2.0.0/docs/clients/evm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_contract_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_contract_decimals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/send_token.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/evm_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.154153 aiotx-2.0.0/docs/clients/tron_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/tron_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/tron_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/tron_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/tron_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.154153 aiotx-2.0.0/docs/clients/utxo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/estimate_smart_fee.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/from_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/get_last_block_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/import_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/send_bulk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/clients/utxo_client/to_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-23 05:12:51.000000 aiotx-2.0.0/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.154153 aiotx-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-23 05:12:51.000000 aiotx-2.0.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 05:12:51.000000 aiotx-2.0.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-23 05:12:51.000000 aiotx-2.0.0/examples/eth_block_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 05:12:51.000000 aiotx-2.0.0/examples/ltc_block_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 05:12:51.000000 aiotx-2.0.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-23 05:12:51.000000 aiotx-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 05:12:51.000000 aiotx-2.0.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.154153 aiotx-2.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-23 05:12:51.000000 aiotx-2.0.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 05:12:57.210152 aiotx-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-23 05:12:51.000000 aiotx-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.154153 aiotx-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.154153 aiotx-2.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.142153 aiotx-2.0.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.158153 aiotx-2.0.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_chain_id.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.170153 aiotx-2.0.0/tests/fixtures/cassettes/btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/btc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 10852371 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 21958019 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.202153 aiotx-2.0.0/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_chain_id.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.202153 aiotx-2.0.0/tests/fixtures/cassettes/ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42576 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34448 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/fixtures/networks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.142153 aiotx-2.0.0/tests/test_evm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.206153 aiotx-2.0.0/tests/test_evm/test_bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_bsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_bsc/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.206153 aiotx-2.0.0/tests/test_evm/test_eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_eth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_eth/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_eth/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_evm/test_eth/test_eth_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.146153 aiotx-2.0.0/tests/test_utxo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.206153 aiotx-2.0.0/tests/test_utxo/test_btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_utxo/test_btc/test_btc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_utxo/test_btc/test_btc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:57.206153 aiotx-2.0.0/tests/test_utxo/test_ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_utxo/test_ltc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_utxo/test_ltc/test_ltc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 05:12:51.000000 aiotx-2.0.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
```

### Comparing `aiotx-1.3.0/.github/workflows/lint-check.yml` & `aiotx-2.0.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/.github/workflows/mysql_test.yml` & `aiotx-2.0.0/.github/workflows/mysql_test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/.github/workflows/python-publish.yml` & `aiotx-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/.github/workflows/static.yml` & `aiotx-2.0.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/.github/workflows/test.yml` & `aiotx-2.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/.gitignore` & `aiotx-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/CHANGELOG.md` & `aiotx-2.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [2.0.0]
+- BREAKING change - EVM chain ID parameter removed from client definition
+
 ## [1.3.0]
 - Pulling block only if they are in network to stop printing a lot of errors
 
 ## [1.2.5]
 - Pin the version of main packages and code changes for new eth_account 
 
 ## [1.2.4]
```

### Comparing `aiotx-1.3.0/CODE_OF_CONDUCT.md` & `aiotx-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/CONTRIBUTING.md` & `aiotx-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/LICENSE` & `aiotx-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/PKG-INFO` & `aiotx-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.3.0
+Version: 2.0.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
@@ -105,15 +105,15 @@
 ```
 
 Sending Tokens (Ethereum):
 ```python
 from aiotx.clients import AioTxETHClient
 
 async def main():
-    eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+    eth_client = AioTxETHClient("NODE_URL")
     
     private_key = "YOUR_PRIVATE_KEY"
     to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
     token_address = "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984"  # Example token address (Uniswap)
     amount = eth_client.to_wei(10, "ether")  # Sending 10 tokens
     
     tx_hash = await eth_client.send_token(private_key, to_address, token_address, amount)
@@ -123,15 +123,15 @@
 ```
 
 Sending Native Currency (Ethereum):
 ```python
 from aiotx.clients import AioTxETHClient
 
 async def main():
-    eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+    eth_client = AioTxETHClient("NODE_URL")
     
     private_key = "YOUR_PRIVATE_KEY"
     to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
     amount = eth_client.to_wei(0.5, "ether")  # Sending 0.5 ETH
     
     tx_hash = await eth_client.send(private_key, to_address, amount)
     print(f"Transaction Hash: {tx_hash}")
```

### Comparing `aiotx-1.3.0/README.md` & `aiotx-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ```
 
 Sending Tokens (Ethereum):
 ```python
 from aiotx.clients import AioTxETHClient
 
 async def main():
-    eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+    eth_client = AioTxETHClient("NODE_URL")
     
     private_key = "YOUR_PRIVATE_KEY"
     to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
     token_address = "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984"  # Example token address (Uniswap)
     amount = eth_client.to_wei(10, "ether")  # Sending 10 tokens
     
     tx_hash = await eth_client.send_token(private_key, to_address, token_address, amount)
@@ -76,15 +76,15 @@
 ```
 
 Sending Native Currency (Ethereum):
 ```python
 from aiotx.clients import AioTxETHClient
 
 async def main():
-    eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+    eth_client = AioTxETHClient("NODE_URL")
     
     private_key = "YOUR_PRIVATE_KEY"
     to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
     amount = eth_client.to_wei(0.5, "ether")  # Sending 0.5 ETH
     
     tx_hash = await eth_client.send(private_key, to_address, amount)
     print(f"Transaction Hash: {tx_hash}")
```

### Comparing `aiotx-1.3.0/aiotx/clients/__init__.py` & `aiotx-2.0.0/aiotx/clients/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import pkg_resources
 
 from ._evm_base_client import AioTxEVMClient
 from ._utxo_base_client import AioTxUTXOClient
 
 
 class AioTxBSCClient(AioTxEVMClient):
-    def __init__(self, node_url, chain_id):
-        super().__init__(node_url, chain_id)
+    def __init__(self, node_url):
+        super().__init__(node_url)
         bep20_abi_json = pkg_resources.resource_string('aiotx.utils', 'bep20_abi.json')
         self._bep20_abi = json.loads(bep20_abi_json)
 
     def _get_abi_entries(self):
         return [entry for entry in self._bep20_abi]
 
 
 class AioTxETHClient(AioTxEVMClient):
-    def __init__(self, node_url, chain_id):
-        super().__init__(node_url, chain_id)
+    def __init__(self, node_url):
+        super().__init__(node_url)
         erc20_abi_json = pkg_resources.resource_string('aiotx.utils', 'erc20_abi.json')
         self._erc20_abi = json.loads(erc20_abi_json)
 
     def _get_abi_entries(self):
         return [entry for entry in self._erc20_abi]
```

### Comparing `aiotx-1.3.0/aiotx/clients/_base_client.py` & `aiotx-2.0.0/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/aiotx/clients/_evm_base_client.py` & `aiotx-2.0.0/aiotx/clients/_evm_base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     VMExecutionError,
     WrongPrivateKey,
 )
 from aiotx.types import BlockParam
 
 
 class AioTxEVMClient(AioTxClient):
-    def __init__(self, node_url, chain_id):
+    def __init__(self, node_url):
         super().__init__(node_url)
-        self.chain_id = chain_id
+        self.chain_id = None
         self.monitor = EvmMonitor(self)
         self._monitoring_task = None
 
     def generate_address(self):
         private_key_bytes = secrets.token_hex(32)
         private_key = "0x" + private_key_bytes
         acct = Account.from_key(private_key)
@@ -176,14 +176,16 @@
     ) -> str:
         if gas_price is None:
             gas_price = await self.get_gas_price()
 
         from_address = self.get_address_from_private_key(private_key)
         if nonce is None:
             nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
+        if self.chain_id is None:
+            self.chain_id = await self.get_chain_id()
         transaction = {
             "nonce": nonce,
             "gasPrice": gas_price,
             "gas": gas_limit,
             "to": to_checksum_address(to_address),
             "value": amount,
             "data": b"",
@@ -206,14 +208,16 @@
         gas_limit: int = 100000,
     ) -> str:
         from_address = self.get_address_from_private_key(private_key)
         if nonce is None:
             nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
         if gas_price is None:
             gas_price = await self.get_gas_price()
+        if self.chain_id is None:
+            self.chain_id = await self.get_chain_id()
         function_signature = "transfer(address,uint256)"
         function_selector = keccak(function_signature.encode("utf-8"))[:4].hex()
         transfer_data = encode(["address", "uint256"], [to_checksum_address(to_address), amount])
         data = "0x" + function_selector + transfer_data.hex()
 
         transaction = {
             "nonce": nonce,
@@ -227,14 +231,20 @@
 
         signed_transaction = Account.sign_transaction(transaction, private_key)
         raw_tx = to_hex(signed_transaction.raw_transaction)
 
         payload = {"method": "eth_sendRawTransaction", "params": [raw_tx]}
         result = await self._make_rpc_call(payload)
         return result["result"]
+    
+    async def get_chain_id(self) -> int:
+        payload = {"method": "eth_chainId", "params": []}
+        result = await self._make_rpc_call(payload)
+        tx_count = result["result"]
+        return 0 if tx_count == "0x" else int(tx_count, 16)
 
     async def _make_rpc_call(self, payload) -> dict:
         payload["jsonrpc"] = "2.0"
         payload["id"] = 1
         async with aiohttp.ClientSession() as session:
             async with session.post(self.node_url, data=json.dumps(payload)) as response:
                 result = await response.json()
```

### Comparing `aiotx-1.3.0/aiotx/clients/_utxo_base_client.py` & `aiotx-2.0.0/aiotx/clients/_utxo_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/aiotx/exceptions.py` & `aiotx-2.0.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/aiotx/utils/bep20_abi.json` & `aiotx-2.0.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/aiotx/utils/erc20_abi.json` & `aiotx-2.0.0/aiotx/utils/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/aiotx.egg-info/PKG-INFO` & `aiotx-2.0.0/aiotx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.3.0
+Version: 2.0.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
@@ -105,15 +105,15 @@
 ```
 
 Sending Tokens (Ethereum):
 ```python
 from aiotx.clients import AioTxETHClient
 
 async def main():
-    eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+    eth_client = AioTxETHClient("NODE_URL")
     
     private_key = "YOUR_PRIVATE_KEY"
     to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
     token_address = "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984"  # Example token address (Uniswap)
     amount = eth_client.to_wei(10, "ether")  # Sending 10 tokens
     
     tx_hash = await eth_client.send_token(private_key, to_address, token_address, amount)
@@ -123,15 +123,15 @@
 ```
 
 Sending Native Currency (Ethereum):
 ```python
 from aiotx.clients import AioTxETHClient
 
 async def main():
-    eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+    eth_client = AioTxETHClient("NODE_URL")
     
     private_key = "YOUR_PRIVATE_KEY"
     to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
     amount = eth_client.to_wei(0.5, "ether")  # Sending 0.5 ETH
     
     tx_hash = await eth_client.send(private_key, to_address, amount)
     print(f"Transaction Hash: {tx_hash}")
```

### Comparing `aiotx-1.3.0/aiotx.egg-info/SOURCES.txt` & `aiotx-2.0.0/aiotx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,22 +63,22 @@
 docs/clients/utxo_client/import_address.rst
 docs/clients/utxo_client/index.rst
 docs/clients/utxo_client/send.rst
 docs/clients/utxo_client/send_bulk.rst
 docs/clients/utxo_client/to_satoshi.rst
 examples/aiogram_notificator_bot.png
 examples/aiogram_notificator_bot.py
-examples/block_and_transactions_parser.py
 examples/eth_block_monitoring.py
 examples/ltc_block_monitoring.py
 examples/two_block_parsers.py
 scripts/build_and_test.sh
 tests/conftest.py
 tests/fixtures/networks.json
 tests/fixtures/cassettes/bsc/get_balance.yaml
+tests/fixtures/cassettes/bsc/get_chain_id.yaml
 tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
 tests/fixtures/cassettes/bsc/get_gas_price.yaml
 tests/fixtures/cassettes/bsc/get_last_block.yaml
 tests/fixtures/cassettes/bsc/get_token_balance.yaml
 tests/fixtures/cassettes/bsc/get_transaction.yaml
 tests/fixtures/cassettes/bsc/get_transaction_count.yaml
 tests/fixtures/cassettes/bsc/send_token_transaction.yaml
@@ -87,14 +87,15 @@
 tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
 tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
 tests/fixtures/cassettes/btc/send_transaction.yaml
 tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
 tests/fixtures/cassettes/btc/test_async_monitoring.yaml
 tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
 tests/fixtures/cassettes/eth/get_balance.yaml
+tests/fixtures/cassettes/eth/get_chain_id.yaml
 tests/fixtures/cassettes/eth/get_contract_decimals.yaml
 tests/fixtures/cassettes/eth/get_gas_price.yaml
 tests/fixtures/cassettes/eth/get_last_block.yaml
 tests/fixtures/cassettes/eth/get_token_balance.yaml
 tests/fixtures/cassettes/eth/get_transaction.yaml
 tests/fixtures/cassettes/eth/get_transaction_count.yaml
 tests/fixtures/cassettes/eth/send_token_transaction.yaml
```

### Comparing `aiotx-1.3.0/docs/Makefile` & `aiotx-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/get_balance.rst` & `aiotx-2.0.0/docs/clients/evm_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/get_block_by_number.rst` & `aiotx-2.0.0/docs/clients/evm_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/get_contract_balance.rst` & `aiotx-2.0.0/docs/clients/evm_client/get_contract_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/get_contract_decimals.rst` & `aiotx-2.0.0/docs/clients/evm_client/get_contract_decimals.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/get_transaction.rst` & `aiotx-2.0.0/docs/clients/evm_client/get_transaction.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/get_transaction_count.rst` & `aiotx-2.0.0/docs/clients/evm_client/get_transaction_count.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/index.rst` & `aiotx-2.0.0/docs/clients/evm_client/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 .. code-block:: python
 
    from aiotx.clients import AioTxETHClient
    import asyncio
 
 
    async def main():
-      eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+      eth_client = AioTxETHClient("NODE_URL")
 
       last_block = await eth_client.get_last_block_number()
       print("last_block", last_block)
 
       tx_data = await eth_client.get_transaction("tx_id")
       print("tx_data", tx_data)
```

### Comparing `aiotx-1.3.0/docs/clients/evm_client/send.rst` & `aiotx-2.0.0/docs/clients/evm_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/evm_client/send_token.rst` & `aiotx-2.0.0/docs/clients/evm_client/send_token.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/estimate_smart_fee.rst` & `aiotx-2.0.0/docs/clients/utxo_client/estimate_smart_fee.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/generate_address.rst` & `aiotx-2.0.0/docs/clients/utxo_client/generate_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/get_address_from_private_key.rst` & `aiotx-2.0.0/docs/clients/utxo_client/get_address_from_private_key.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/get_balance.rst` & `aiotx-2.0.0/docs/clients/utxo_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/get_block_by_number.rst` & `aiotx-2.0.0/docs/clients/utxo_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/import_address.rst` & `aiotx-2.0.0/docs/clients/utxo_client/import_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/index.rst` & `aiotx-2.0.0/docs/clients/utxo_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/send.rst` & `aiotx-2.0.0/docs/clients/utxo_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/clients/utxo_client/send_bulk.rst` & `aiotx-2.0.0/docs/clients/utxo_client/send_bulk.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/conf.py` & `aiotx-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/index.rst` & `aiotx-2.0.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 Sending Tokens (Ethereum):
 
 .. code-block:: python
 
    from aiotx.clients import AioTxETHClient
 
    async def main():
-      eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+      eth_client = AioTxETHClient("NODE_URL")
       
       private_key = "YOUR_PRIVATE_KEY"
       to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
       # Example token address (Uniswap)
       token_address = "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984"
       amount = eth_client.to_wei(10, "ether")  # Sending 10 tokens
       
@@ -88,15 +88,15 @@
 
 
 .. code-block:: python
 
    from aiotx.clients import AioTxETHClient
 
    async def main():
-      eth_client = AioTxETHClient("NODE_URL", "ETH_CHAIN_ID")
+      eth_client = AioTxETHClient("NODE_URL")
       
       private_key = "YOUR_PRIVATE_KEY"
       to_address = "0x742d35Cc6634C0532925a3b844Bc454e4438f44e"
       amount = eth_client.to_wei(0.5, "ether")  # Sending 0.5 ETH
       
       tx_hash = await eth_client.send(private_key, to_address, amount)
       print(f"Transaction Hash: {tx_hash}")
```

### Comparing `aiotx-1.3.0/docs/make.bat` & `aiotx-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/monitoring.rst` & `aiotx-2.0.0/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/docs/testing.rst` & `aiotx-2.0.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/examples/aiogram_notificator_bot.png` & `aiotx-2.0.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/examples/aiogram_notificator_bot.py` & `aiotx-2.0.0/examples/aiogram_notificator_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from aiotx.clients import AioTxBSCClient
 
 # Create an instance of the aiogram bot
 bot = Bot(token="BOT TOKEN")
 dispatcher = Dispatcher()
 
 # Create an instance of the AioTxBSCClient
-bsc_client = AioTxBSCClient("NODE URL", 97)
+bsc_client = AioTxBSCClient("https://bsc-testnet-rpc.publicnode.com")
 
 
 # Define the block handler
 @bsc_client.monitor.on_block
 async def handle_block(block):
     block_number = block
     chat_id = "5454053704"  # Replace with the actual chat ID
```

### Comparing `aiotx-1.3.0/examples/block_and_transactions_parser.py` & `aiotx-2.0.0/examples/eth_block_monitoring.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from aiotx.clients import AioTxBSCClient
+from aiotx.clients import AioTxETHClient
 import asyncio
 
-client = AioTxBSCClient("NODE_URL", 97)
+eth_client = AioTxETHClient(
+    node_url="https://ethereum-sepolia-rpc.publicnode.com")
 
-@client.monitor.on_block
+
+@eth_client.monitor.on_block
 async def handle_block(block):
-    print("block", block)
+    print("eth_client: block", block)
 
-@client.monitor.on_transaction
+@eth_client.monitor.on_transaction
 async def handle_transaction(transaction):
-    print("transaction", transaction)
-
+    print("eth_client: transaction", transaction)
 
 async def main():
-    await client.start_monitoring()
-
-    try:
-        while True:
-            await asyncio.sleep(1)
-    except KeyboardInterrupt:
-        client.stop_monitoring()
-
+    await eth_client.start_monitoring()
+    while True:
+        await asyncio.sleep(1)
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `aiotx-1.3.0/examples/eth_block_monitoring.py` & `aiotx-2.0.0/examples/ltc_block_monitoring.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from aiotx.clients import AioTxETHClient
+from aiotx.clients import AioTxLTCClient
 import asyncio
 
-eth_client = AioTxETHClient(
-    node_url="https://ethereum-sepolia-rpc.publicnode.com", 
-    chain_id=11155111)
+ltc_client = AioTxLTCClient(node_url="https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet", testnet=True)
 
 
-@eth_client.monitor.on_block
+@ltc_client.monitor.on_block
 async def handle_block(block):
-    print("eth_client: block", block)
+    print("ltc_client: block", block)
 
-@eth_client.monitor.on_transaction
+@ltc_client.monitor.on_transaction
 async def handle_transaction(transaction):
-    print("eth_client: transaction", transaction)
+    print("ltc_client: transaction", transaction)
 
 async def main():
-    await eth_client.start_monitoring()
+    await ltc_client.start_monitoring()
     while True:
         await asyncio.sleep(1)
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `aiotx-1.3.0/examples/two_block_parsers.py` & `aiotx-2.0.0/examples/two_block_parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from aiotx.clients import AioTxBSCClient, AioTxETHClient
 import asyncio
 
-bsc_client = AioTxBSCClient("NODE_URL", 97)
-eth_client = AioTxETHClient("NODE_URL", 1151511)
+BSC_TEST_NODE_URL = "https://bsc-testnet-rpc.publicnode.com"
+ETH_TEST_NODE_URL = "https://ethereum-sepolia-rpc.publicnode.com"
+
+bsc_client = AioTxBSCClient(BSC_TEST_NODE_URL)
+eth_client = AioTxETHClient(ETH_TEST_NODE_URL)
 
 @bsc_client.monitor.on_block
 async def handle_block(block):
     print("bsc_client: block", block)
 
 @bsc_client.monitor.on_transaction
 async def handle_transaction(transaction):
```

### Comparing `aiotx-1.3.0/setup.py` & `aiotx-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/conftest.py` & `aiotx-2.0.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,59 +10,52 @@
 
 # ALL = "all"
 # ANY = "any"
 # NEW_EPISODES = "new_episodes"
 # NONE = "none"
 # ONCE = "once"
 
+BSC_TEST_NODE_URL = "https://bsc-testnet-rpc.publicnode.com"
+ETH_TEST_NODE_URL = "https://ethereum-sepolia-rpc.publicnode.com"
+LTC_TEST_NODE_URL = "https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet"
+BTC_TEST_NODE_URL = "https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/"
+
+
 pytest.mark.mysql = pytest.mark.mysql
 logging.getLogger("vcr").setLevel(logging.WARNING)
 vcr_c = vcr.VCR(
     cassette_library_dir="tests/fixtures/cassettes",
     record_mode=os.environ.get("VCR_RECORD_MODE", "none"),
     match_on=["host", "path", "method", "query", "raw_body", "body"],
     filter_headers=["Authorization", "Cookie", "Date"],
 )
 
-BSC_TEST_NODE_URL = "https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/"
-BSC_TEST_CHAIN_ID = 97
-
 
 @pytest.fixture
 def bsc_client() -> AioTxBSCClient:
-    return AioTxBSCClient(BSC_TEST_NODE_URL, BSC_TEST_CHAIN_ID)
-
-
-ETH_TEST_NODE_URL = "https://ethereum-sepolia-rpc.publicnode.com"
-ETH_TEST_CHAIN_ID = 11155111
+    return AioTxBSCClient(BSC_TEST_NODE_URL)
 
 
 @pytest.fixture
 def eth_client() -> AioTxETHClient:
-    return AioTxETHClient(ETH_TEST_NODE_URL, ETH_TEST_CHAIN_ID)
-
-
-LTC_TEST_NODE_URL = "https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet"
+    return AioTxETHClient(ETH_TEST_NODE_URL)
 
 
 @pytest.fixture
 def ltc_public_client(request: FixtureRequest) -> AioTxLTCClient:
     def teardown():
         try:
             os.remove("test_ltc.sqlite")
         except FileNotFoundError:
             print("test_ltc.sqlite FileNotFoundError")
 
     request.addfinalizer(teardown)
     return AioTxLTCClient(LTC_TEST_NODE_URL, testnet=True, db_url="sqlite+aiosqlite:///test_ltc.sqlite")
 
 
-BTC_TEST_NODE_URL = "https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/"
-
-
 @pytest.fixture
 def btc_client(request: FixtureRequest) -> AioTxBTCClient:
     def teardown():
         try:
             os.remove("test_btc.sqlite")
         except FileNotFoundError:
             print("test_btc.sqlite FileNotFoundError")
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,106 @@
 interactions:
 - request:
-    body: '{"method": "eth_call", "params": [{"to": "0x337610d27c682E347C9cD60BD4b3b107C9d34dDd",
-      "data": "0x313ce567"}, "latest"], "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x0000000000000000000000000000000000000000000000000000000000000012"}
+      string: '{"result":2815689,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '103'
+      - '48'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:37:46 GMT
+      - Thu, 16 May 2024 06:18:06 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_call", "params": [{"to": "0x337610d27c682E347C9cD60BD4b3b107C9d34dD",
-      "data": "0x313ce567"}, "latest"], "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "estimatesmartfee", "params": [1, "CONSERVATIVE"], "jsonrpc":
+      "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32602,"message":"invalid argument
-        0: json: cannot unmarshal hex string of odd length into Go struct field TransactionArgs.to
-        of type common.Address"}}
+      string: '{"result":{"feerate":0.000365500,"blocks":2},"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '192'
+      - '74'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:37:46 GMT
+      - Thu, 16 May 2024 06:18:06 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
+      - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_call", "params": [{"to": "0x757fc78bb4df4ce6605ae669bf0b71074176aac3",
-      "data": "0x313ce567"}, "latest"], "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "sendrawtransaction", "params": ["01000000000101c23c8e8730b555d7cb96bcf06082eaad86594bc604d9f667bc57608b7a8b15350000000000ffffffff01e8030000000000001976a914912e2b234f941f30b18afbb4fa46171214bf66c888ac02483045022100b2cf6022cabe152a87f173542238565b953718159ad1932c9cc24fcd7af674a002201ca194aa7d32dfaadd1d3d7fbcd0bb1d7736b7b705734548cf41cfacb5946c420121032483516ae6532dbeaf537cb5c1da64f973a6066fbde788f665b3dbd45f7417a900000000"],
+      "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x0000000000000000000000000000000000000000000000000000000000000009"}
+      string: '{"result":"77cb20c4b0325242b9e5f45f4850e5387dc585d6b72bb36ba65a126534436973","error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '103'
+      - '107'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:37:46 GMT
+      - Thu, 16 May 2024 06:18:06 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 interactions:
 - request:
     body: '{"method": "eth_gasPrice", "params": [], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x12a05f200"}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x12d00e280"}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '48'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888270279bd752ba-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 08:12:58 GMT
+      - Thu, 23 May 2024 04:52:42 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '6'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/btc/send_transaction.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 interactions:
 - request:
-    body: '{"method": "eth_blockNumber", "params": [], "id": 1, "jsonrpc": "2.0"}'
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x261b51d"}'
+      string: '{"result":2814768,"error":null,"id":"curltest"}
+
+        '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '45'
+      - '48'
       Content-Type:
       - application/json
       Date:
-      - Wed, 01 May 2024 18:07:30 GMT
+      - Sat, 11 May 2024 12:16:41 GMT
       Vary:
       - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_blockNumber", "params": [], "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "sendrawtransaction", "params": ["01000000000101b91af3cb667b7367bd56a5c8380e93dbe866bdc8588ef9d3004d5c3d696fd5250000000000ffffffff02b73700000000000016001483a1f161bcfb3f6d290d1a0eeebe0e8e92589eeae803000000000000160014aad2f3a30a624ed4240b6c6599c6145b5a2d738f02473044022020a2c2de6daccbe4e26b241dca4db2247eded4efbaecc2cc9169de2e44a17dc802200bb36b447f4bebe26d59fd54f86e0d2106eb380f79def73e49eb4f03e7512fd70121032483516ae6532dbeaf537cb5c1da64f973a6066fbde788f665b3dbd45f7417a900000000"],
+      "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x261bd7a"}'
+      string: '{"result":"4f9a64d28ae22134379f7da50282d7ca2ead8a1f8378b20e25defcaaa5c59228","error":null,"id":"curltest"}
+
+        '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '45'
+      - '107'
       Content-Type:
       - application/json
       Date:
-      - Wed, 01 May 2024 19:54:32 GMT
+      - Sat, 11 May 2024 12:16:42 GMT
       Vary:
       - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,396 +1,390 @@
 interactions:
 - request:
-    body: '{"method": "eth_getTransactionCount", "params": ["0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e",
-      "pending"], "jsonrpc": "2.0", "id": 1}'
-    headers: {}
-    method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
-  response:
-    body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x7e"}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '41'
-      Content-Type:
-      - application/json
-      Date:
-      - Fri, 03 May 2024 10:46:45 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8aa7e85012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a0ba58900b587e6278f5476fc28a1f09bf4b326bb72e06361642aab898ef8939f8a06296f0183dad417850fb2e9d260a0887c77687b4c47069652fb6dbf4cf3af341"],
-      "jsonrpc": "2.0", "id": 1}'
-    headers: {}
-    method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
-  response:
-    body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x247e15f1dc165cb70964bb206c7bd0457490a33042c7a8c80453d250f8f30adb"}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '103'
-      Content-Type:
-      - application/json
-      Date:
-      - Fri, 03 May 2024 10:46:45 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8aa7e85012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a00000000000000000000000000000000000000000000003635c9adc5dea0000081e6a02b3a459ca69afce5840f287c4da1138622ba38eed7ea6c66718c5890ae5cfc75a06e928f4a2675fd1dfb3e9edf660ce020a4025f50e7ee3af331828ea1baa3ed01"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909118"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
-        transaction underpriced"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":{"blockHash":"0x4a8b62d56a105505bc7513afdcb99b5652b2208db94f6f295c9aebbd2e298c10","blockNumber":"0x261b4c2","from":"0x40d3256eb0babe89f0ea54edaa398513136612f5","gas":"0x7fffffffffffffff","gasPrice":"0x0","hash":"0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909118","input":"0xf340fa0100000000000000000000000040d3256eb0babe89f0ea54edaa398513136612f5","nonce":"0x12db1","to":"0x0000000000000000000000000000000000001000","transactionIndex":"0x24","value":"0x55b89a5486cac0","type":"0x0","chainId":"0x61","v":"0xe6","r":"0xf1964f5081e0be9c3bd893b6254fbbbce6d111fcc90cdbdd553a40cada838d64","s":"0x19bce7654b881b939dc01547276124cb4887e73b8b0d63b34b814bc0216a91e4"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '97'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888270102b4f7743-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:46 GMT
+      - Thu, 23 May 2024 04:52:39 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '16'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a57e8082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a03d89bf6188b6089d1b3adee999ed9b9005651a98b3859867bb19eef37987bfafa054f02f754f57f7b38c7154fab2dc154e9ef34f1bcd81751806be6477736201f0"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0xdeac5f03c42970ec4c89ec540c886a2738b8b8fc8c415d0bd231ea94dad81727"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 0, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":{"blockHash":"0x4a8b62d56a105505bc7513afdcb99b5652b2208db94f6f295c9aebbd2e298c10","blockNumber":"0x261b4c2","from":"0x6371b88cc8288527bc9dab7ec68671f69f0e0862","gas":"0x2dc6c0","gasPrice":"0x124101100","hash":"0xdeac5f03c42970ec4c89ec540c886a2738b8b8fc8c415d0bd231ea94dad81727","input":"0xe25ce13d0000000000000000000000000000000000000000000000000000018f35525052","nonce":"0x133cc","to":"0xc0e744910c357ef0c2560c8fbd4dc6a880ddeed2","transactionIndex":"0x1f","value":"0x0","type":"0x0","chainId":"0x61","v":"0xe6","r":"0x405351594b32cf9ae3350f20614933d7073b8412f10e66612a7182418ff48579","s":"0x6c11a1e056c78c146a5f27351c7646e84505ece8738fc4e4311fc3e615802bf1"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '127'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888270113ffd6402-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:46 GMT
+      - Thu, 23 May 2024 04:52:39 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '8'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8aa7e85012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a000000000000000000000000000000000000000000000000000000000000000081e6a01ad77489659872f1037f05f1463bdbc4a4bc88e07770fa29ecf231cea2aa2d2da074b6c5bc9a7d8a704dda251aec574de2d188f66703bf1c39eeab4a504ea1ccbd"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0x26611f5796882c8f45a52c4443c2cda4580ef0bb06d57686d34672207312dfd3"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
-        transaction underpriced"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":{"blockHash":"0x4a8b62d56a105505bc7513afdcb99b5652b2208db94f6f295c9aebbd2e298c10","blockNumber":"0x261b4c2","from":"0x1f419e592a7e2ea2a75fd8c529d6cbe59a4884a6","gas":"0x8ca0","gasPrice":"0x248202200","hash":"0x26611f5796882c8f45a52c4443c2cda4580ef0bb06d57686d34672207312dfd3","input":"0x","nonce":"0x98e","to":"0xc23e4cf1052e9b5bace3a903c3cbd6caf86fa987","transactionIndex":"0x7","value":"0x136a3c41ea31c3","type":"0x0","chainId":"0x61","v":"0xe5","r":"0x8dea66af54f144ade187737dc061652adc04b724fdf431fc7a199a6961a31fe1","s":"0x49dd96e4668404e29ab2299bc6125b9125a808499f5e501fa173f9573eec8642"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '97'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827011f921653e-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:46 GMT
+      - Thu, 23 May 2024 04:52:39 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '8'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a87e85012a05f2008094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a0c72ec598dde29546d5047253d68f08bb3259d82eb6bec1da59336c16b3052125a07616ed31466c365c61ceeed698ffcc3fc422de8ce84a21255b9c4806bf2845f9"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0xf82c96662db872899f16ea9dfed73fb7c29f3942fdbfc97500ca071793f5a397"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"intrinsic
-        gas too low: gas 0, minimum needed 21632"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":{"blockHash":"0x69640719fc4224dab84ed813ab8b4c87a691773582c62f4f098d7b74aca87923","blockNumber":"0x261b4c1","from":"0x1284214b9b9c85549ab3d2b972df0deef66ac2c9","gas":"0x7fffffffffffffff","gasPrice":"0x0","hash":"0xf82c96662db872899f16ea9dfed73fb7c29f3942fdbfc97500ca071793f5a397","input":"0xf340fa010000000000000000000000001284214b9b9c85549ab3d2b972df0deef66ac2c9","nonce":"0x46c1f3","to":"0x0000000000000000000000000000000000001000","transactionIndex":"0x14","value":"0x1ed7885f8e3900","type":"0x0","chainId":"0x61","v":"0xe6","r":"0x59727c87cb30990bcfed3f015fa58c20f24f016ede2a262fc075a722ff866704","s":"0x30c706b761c74536c3fa3ddb1105508d17359a32d4123368f167cd8aa912b0e5"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '112'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827012fed4954a-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:47 GMT
+      - Thu, 23 May 2024 04:52:39 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '8'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ad85012a05f20082ee48830186a094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a0a351c4d530f3ca015a214a1e9448ce6b2f19facbc971af5e0f65fa014da9a4b1a04c99106eab23cf51c72cac69ecd6413a985a88f2bd03374e95d71c5f757a1408"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0x8a0dc46462919c8a1c15c90e79782ba4e56b9053fad8975c9b6bec094f001895"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 61000, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":{"blockHash":"0x69640719fc4224dab84ed813ab8b4c87a691773582c62f4f098d7b74aca87923","blockNumber":"0x261b4c1","from":"0xb885e591186c8f8c597f579438ba2d5c5c3b347b","gas":"0x2d194","gasPrice":"0x12a05f200","maxFeePerGas":"0x12a05f200","maxPriorityFeePerGas":"0x12a05f200","hash":"0x8a0dc46462919c8a1c15c90e79782ba4e56b9053fad8975c9b6bec094f001895","input":"0xee4cc30300000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000000000120000000000000000000000000000000000000000000000000000000000000016000000000000000000000000000000000000000000000000000000000000001a000000000000000000000000000000000000000000000000000000000000001e0000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000019ffc09ffc1f91b9c5aa334b74e96b33c9434841494e49443937000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000b885e591186c8f8c597f579438ba2d5c5c3b347b0000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000001900000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000066322f54000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000663380d4","nonce":"0x2dc","to":"0xcb473481e185a86fd94088657ae67efdb8973e41","transactionIndex":"0xf","value":"0x64","type":"0x2","accessList":[],"chainId":"0x61","v":"0x1","r":"0x89f953cc88da8868554bdf6384c6e0ec0be82f1ee1ceb7250e5f640afb6d875e","s":"0x5ceac699ccdabfbdcc140e184170a613e2c454013fd8fd7483fe624a0f31249e","yParity":"0x1"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '131'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827013ec6c63cc-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:24:23 GMT
+      - Thu, 23 May 2024 04:52:39 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '9'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ad85012a05f20082ee48830186a094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a00000000000000000000000000000000000000000000003635c9adc5dea0000081e5a04fe631e2b872d300a91f69c040381dbd0a8a964488ffbe2da38988b254ba5000a055dd5025c9c7c6d2001e91e70bbe02a9049d58ef0bc2d50764680a73d0cf4a0b"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0x41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 61000, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":{"blockHash":"0x651eaa5b870befe4b8225c22bfef4d1c8f53282609f596725633ec5f410eddbc","blockNumber":"0x260dbf6","from":"0x3a82a5a2b77d33a12621e860d1d19cdfb8bf63b4","gas":"0x2d182","gasPrice":"0x12a05f200","maxFeePerGas":"0x12a05f200","maxPriorityFeePerGas":"0x12a05f200","hash":"0x41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae","input":"0xee4cc30300000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000000000120000000000000000000000000000000000000000000000000000000000000016000000000000000000000000000000000000000000000000000000000000001a000000000000000000000000000000000000000000000000000000000000001e0000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000019ef46411eb79f1f72ce96ca9d0e594100434841494e494439370000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000003a82a5a2b77d33a12621e860d1d19cdfb8bf63b400000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000019000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000662fcf1300000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000066312093","nonce":"0x265","to":"0xcb473481e185a86fd94088657ae67efdb8973e41","transactionIndex":"0xf","value":"0x64","type":"0x2","accessList":[],"chainId":"0x61","v":"0x0","r":"0x83e224c3651f5cc755dfe14278eed299236175856a5b35b35e1966bb81df9d3b","s":"0x7171ee68b62f871f1a8c5af55c6b3322291fdd69f320a4ab790b19bec1ecbe7","yParity":"0x0"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '131'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827014eb252401-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:24:24 GMT
+      - Thu, 23 May 2024 04:52:39 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '8'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a88082ee48830186a094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a0448fc0df64834102f5f6eda40007bd6f31b434905fbe1d7b1c314d84d5e5c9cca03f8d88875b4e7e020acd8ebccfce97eec62292a59741b6db01458d6840b402c5"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909111"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 61000, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":null}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827015eb39638e-LHR
+      Connection:
+      - keep-alive
       Content-Length:
-      - '131'
+      - '39'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:24:24 GMT
+      - Thu, 23 May 2024 04:52:40 GMT
+      Server:
+      - cloudflare
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-ecf10b7bc104d983
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '7'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ad85012a05f20082ee48830186a094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a000000000000000000000000000000000000000000000000000000000000000081e6a046f884aad1a6ab874d0b557dd90aaf19137528e4f614683bbf69161d35293c33a0375e0ec94ad63f576b3a6a2aa903ab256d2a81cf50b1a4e2159200e46861a953"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b945190911"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 61000, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32602,"message":"invalid argument
+        0: json: cannot unmarshal hex string of odd length into Go value of type common.Hash"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '131'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827016aa25633d-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:24:24 GMT
+      - Thu, 23 May 2024 04:52:40 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-ecf10b7bc104d983
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '6'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ab85012a05f20080830186a094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a06cb0f0e3dde3b85c4ea71cf90e9eeb0b8d9b0f82872152c2d75649d66518c0dba051499f3a60a51b89c738a9c9dd7d1cc30babdc8bd2f08c9365ff5b63616c94d5"],
+    body: '{"method": "eth_getTransactionByHash", "params": ["41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 0, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32602,"message":"invalid argument
+        0: json: cannot unmarshal hex string without 0x prefix into Go value of type
+        common.Hash"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '127'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 8882701768f27785-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:24:25 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Thu, 23 May 2024 04:52:40 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '9'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,253 +1,302 @@
 interactions:
 - request:
     body: '{"method": "eth_getTransactionCount", "params": ["0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e",
       "pending"], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x7f"}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x88"}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888277a19a44dc31-LHR
+      Connection:
+      - keep-alive
       Content-Length:
       - '41'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:47 GMT
+      - Thu, 23 May 2024 04:57:49 GMT
+      Server:
+      - cloudflare
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '7'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86b7f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0dd2ec3a72bee9de8e0367fbf926550e1bbac5d4860184dfa22fec644571f1568a05b3b44321e5976a00e23b91aed9e900a0e854b4b31ca47662d375c524ec2a58f"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ab818885012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a00000000000000000000000000000000000000000000000006f05b59d3b2000081e6a0dd02de25cff385e5c71625e46232c119be77d45eb0b16b2650a11005c77a1b01a035126b9e76371f8f0c484b51cf4d13c7dccb8e9239c2a6ef0fa2482ab497dc75"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0xdad97e8972e7a4cc72f28944a16aa5782d6562aac483b527c27d1ee88e33ed5a"}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0xdc67d13549a4b709a62e8814b63d8bd6d54afdcb935102afb1a019d1cb2e6faf"}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '103'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888277a2bd1c4149-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:47 GMT
+      - Thu, 23 May 2024 04:57:49 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '6'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86d7f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a884563918244f400008081e5a076bcd75b7ded882a7e7194a6588969a505b9b3e9d9f7fb0a7e0af90244cdd4e5a06b371861ae4283029ad8c2c4a6f8913190b949deeb815bd6028bd88564bc29a3"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ab818885012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a00000000000000000000000000000000000000000000003635c9adc5dea0000081e6a0d90026978fca4bbdbeb5fbb214177a289cfa788f04279a88d7e729d7c294e661a0131a378f25f7a39b7086dc646660856fc6329b2c14f909dcd22d15daa009baf9"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"insufficient
-        funds for gas * price + value: balance 19594850000960000, tx cost 5000105000000000000,
-        overshot 4980510149999040000"}}
+      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
+        transaction underpriced"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '190'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888277a3bdef79b4-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:48 GMT
+      - Thu, 23 May 2024 04:57:49 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-2bd95d6b916503dd
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '7'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8667f8082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0157babe76ee1d04f5dc9669b033779bc552f8047911e6ef74e20475e804282a7a06524c9fb61bbef7f4c77c67354d106742bd34eb8bc597c769ae9c1f4ebf638e4"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a681888082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a059ddc7617e123676efbde585c14c20cb735845ced951dad6ce953543693c58faa047ddecffc75e18e958fdc2b1b949801ef695de97167109376a7d12b6d0db531a"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
       string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 0, minimum needed 1000000000"}}
+        underpriced: gas tip cap 0, minimum needed 1"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '127'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888277a4bc8179b8-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:48 GMT
+      - Thu, 23 May 2024 04:57:49 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '7'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8657f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a808081e5a07650c5abd4d2e0f2d0a377c89381d0d56d762a0f9e94975cbb540363cd058959a01b626479385aad061246df6e54a9f59fa898c1f58b341716a533b5682921d28b"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8ab818885012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a000000000000000000000000000000000000000000000000000000000000000081e5a01d793a012991c665b5a14c232916534c6d639e69c171770025849c2b2df7c1d5a04cd5a3a7b75c8a3ea3c1f8101dd059a1a4aef22c4e780fa9b2f047d8de183ba0"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
       string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
         transaction underpriced"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '97'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888277a5ae5b4968-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:48 GMT
+      - Thu, 23 May 2024 04:57:49 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '7'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8697f85012a05f2008094f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e5a08c87832c5608247b85f2c8d24852172e704ff0cb11edb0db3800c49599d1d5c4a017026aaa07c5ce6b31ce684680146ff681d6a8edfb4c73eaf3d83347b8f4ff97"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a9818885012a05f2008094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e5a0bddf75a9cf57ae8a471959758edf0499e53f0cb360699cca6ccbcb1d0212bd46a042611a9f44e6fac88f8939d0376163883a79098e19cefe1520bccac2a531bdcc"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
       string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"intrinsic
-        gas too low: gas 0, minimum needed 21000"}}
+        gas too low: gas 0, minimum needed 21632"}}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '112'
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888277a678fe6353-LHR
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:49 GMT
+      - Thu, 23 May 2024 04:57:49 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '6'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86b7f85012a05f20082ee4894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e5a08eb0828e7d41dc68c8cbfbae52045328afbc4ddb490e982c356151b10d3ec630a00e8a57d4c6a159279e91fddb7f4e0f570a49cb08814da1b36d5828714afd4f16"],
-      "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "eth_chainId", "params": [], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://bsc-testnet-rpc.publicnode.com
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
-        transaction underpriced"}}
+      string: '{"jsonrpc":"2.0","result":"0x61","id":1}
 
         '
     headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827890cc793697-LHR
+      Connection:
+      - keep-alive
       Content-Length:
-      - '97'
+      - '41'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:49 GMT
+      - Thu, 23 May 2024 04:58:27 GMT
+      Server:
+      - cloudflare
       Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '2'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,16 @@
 interactions:
 - request:
-    body: '{"method": "eth_getTransactionCount", "params": ["0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e",
-      "latest"], "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x82"}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '41'
-      Content-Type:
-      - application/json
-      Date:
-      - Sat, 04 May 2024 08:29:18 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "eth_gasPrice", "params": [], "jsonrpc": "2.0", "id": 1}'
-    headers: {}
-    method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
-  response:
-    body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x123f92da0"}
+      string: '{"result":2815184,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -54,122 +19,89 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:29:19 GMT
+      - Tue, 14 May 2024 03:41:42 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
+      - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86c8182850123f92da082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0b04081f4c041911a511f34e23352c05ee7e46b88dafc9cd7d7f3c168322f3deda00ced47f99dc12d686ea384873f8d37d38ffb5dc0fcb2a5d18c25214a7f7e5245"],
-      "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "sendrawtransaction", "params": ["01000000000101b91af3cb667b7367bd56a5c8380e93dbe866bdc8588ef9d3004d5c3d696fd5250000000000ffffffff05ff2b00000000000016001483a1f161bcfb3f6d290d1a0eeebe0e8e92589eeae8030000000000001976a914912e2b234f941f30b18afbb4fa46171214bf66c888ace80300000000000017a914deb0be8cf350aced0168a5864cdc587d53cdb2e087e803000000000000160014057a4289cad910ee6055f3357837afaf4bf513b2e80300000000000022512072258d7a9a3e39a64f086674f5eb3dbade370ea17349b98c3910c390a220a2cf02473044022031c84a9eec646ae895425673042428573cf0aa5274c81e6117861894315620e7022044e068b4172c94d18fb4a48e3ece2f91cb48b2cf5fe2109f5d40cff6dd3f58530121032483516ae6532dbeaf537cb5c1da64f973a6066fbde788f665b3dbd45f7417a900000000"],
+      "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x0f47bdb42e18137f1e166e2fee68877fca081e6e6f639c0ce629a363db5a5e1e"}
+      string: '{"result":null,"error":{"code":-26,"message":"mempool min fee not met,
+        1000 < 5982"},"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '103'
+      - '102'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:29:19 GMT
+      - Tue, 14 May 2024 03:46:40 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-ecf10b7bc104d983
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "eth_gasPrice", "params": [], "jsonrpc": "2.0", "id": 1}'
-    headers: {}
-    method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
-  response:
-    body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x123f92da0"}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '48'
-      Content-Type:
-      - application/json
-      Date:
-      - Sat, 04 May 2024 08:29:19 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
-    status:
-      code: 200
-      message: OK
+      code: 500
+      message: Internal Server Error
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86c8183850123f92da0825208943ffecb152f95f7122990ab16eff4b0b5d533497e8609184e72a0008081e6a0fc492839015f1e9bc8381ebea382c72af6ac48c797050584d344bcc20a15437ba05ffcbd6ff4d80f15b143f4cc2b6f6e12f4c7b576f91c20804c4db72f421c01af"],
-      "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "sendrawtransaction", "params": ["01000000000101b91af3cb667b7367bd56a5c8380e93dbe866bdc8588ef9d3004d5c3d696fd5250000000000ffffffff05771800000000000016001483a1f161bcfb3f6d290d1a0eeebe0e8e92589eeae8030000000000001976a914912e2b234f941f30b18afbb4fa46171214bf66c888ace80300000000000017a914deb0be8cf350aced0168a5864cdc587d53cdb2e087e803000000000000160014057a4289cad910ee6055f3357837afaf4bf513b2e80300000000000022512072258d7a9a3e39a64f086674f5eb3dbade370ea17349b98c3910c390a220a2cf02473044022043d9458b77a69e55477e3674ecc39160de9340703a81254a82dff7cf70c052b202202f29540d74e50f22c402986982789ccee7b1d0860139057217e4105a4c9e38410121032483516ae6532dbeaf537cb5c1da64f973a6066fbde788f665b3dbd45f7417a900000000"],
+      "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x1b03c2e3590ed2193130dbbd25596877adc22e746f705b353d6f6b5f7ce0d192"}
+      string: '{"result":"35158b7a8b6057bc67f6d904c64b5986adea8260f0bc96cbd755b530878e3cc2","error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '103'
+      - '107'
       Content-Type:
       - application/json
       Date:
-      - Sat, 04 May 2024 08:29:19 GMT
+      - Tue, 14 May 2024 03:47:19 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
+      - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
+      - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_balance.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_gas_price.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_last_block.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_token_balance.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -255,8 +255,48 @@
       strict-transport-security:
       - max-age=31536000; includeSubDomains; preload
       x-envoy-upstream-service-time:
       - '7'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "eth_chainId", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0xaa36a7","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827896dfc39492-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 23 May 2024 04:58:28 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '1'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -121,8 +121,48 @@
       strict-transport-security:
       - max-age=31536000; includeSubDomains; preload
       x-envoy-upstream-service-time:
       - '6'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "eth_chainId", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0xaa36a7","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888278985c2c652a-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 23 May 2024 04:58:28 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '1'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/send_transaction.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -344,8 +344,48 @@
       strict-transport-security:
       - max-age=31536000; includeSubDomains; preload
       x-envoy-upstream-service-time:
       - '6'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "eth_chainId", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0xaa36a7","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 888278936c0188ad-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 23 May 2024 04:58:27 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '2'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -165,8 +165,48 @@
       strict-transport-security:
       - max-age=31536000; includeSubDomains; preload
       x-envoy-upstream-service-time:
       - '7'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "eth_chainId", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0xaa36a7","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827894bd2163dd-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 23 May 2024 04:58:28 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '3'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -206,8 +206,48 @@
       strict-transport-security:
       - max-age=31536000; includeSubDomains; preload
       x-envoy-upstream-service-time:
       - '7'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "eth_chainId", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0xaa36a7","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 88827895bab571d2-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 23 May 2024 04:58:28 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '2'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_last_block.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_bulk.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_bulk.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_transaction.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml` & `aiotx-2.0.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/fixtures/networks.json` & `aiotx-2.0.0/tests/fixtures/networks.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_client.py` & `aiotx-2.0.0/tests/test_evm/test_bsc/test_bsc_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,27 @@
 
 @vcr_c.use_cassette("bsc/get_last_block.yaml")
 async def test_get_last_block(bsc_client: AioTxBSCClient):
     block_id = await bsc_client.get_last_block_number()
     assert isinstance(block_id, int)
 
 
+@vcr_c.use_cassette("bsc/get_chain_id.yaml")
+async def test_get_chain_id(bsc_client: AioTxBSCClient):
+    chain_id = await bsc_client.get_chain_id()
+    assert isinstance(chain_id, int)
+    assert chain_id == 97
+
+
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_balance",
     [
-        ("0x1284214b9b9c85549aB3D2b972df0dEEf66aC2c9", None, 10561622435613231665),
-        ("0x3a82a5a2b77d33a12621e860d1d19cdfb8bf63b4", None, 99724094999968300),
-        ("0x0e28BD8B2D4efb8A3128f7fB310f4e227E25DB6F", None, 691239109999999988),
+        ("0x1284214b9b9c85549aB3D2b972df0dEEf66aC2c9", None, 10891723659733231665),
+        ("0x3a82a5a2b77d33a12621e860d1d19cdfb8bf63b4", None, 102029280699956200),
+        ("0x0e28BD8B2D4efb8A3128f7fB310f4e227E25DB6F", None, 690442684999999988),
         ("0xfb2bdebad0cb9486e714b053a2dbfaf7c05151c9", None, 271930000000000),
         ("0x040bA056435A7675847F4D577d3Cb8Fc2646A946", None, 421930000000000),
         ("0x040bA056435A7675847F4D577d3Cb8Fc2646A948", None, 0),
         ("040bA056435A7675847F4D577d3Cb8Fc2646A946", InvalidArgumentError, 0),
     ],
 )
 @vcr_c.use_cassette("bsc/get_balance.yaml")
@@ -70,20 +77,20 @@
         tx = await bsc_client.get_transaction(tx_id)
         assert "aiotx_decoded_input" in tx.keys()
 
 
 @pytest.mark.parametrize(
     "wallet_address, contract, expected_exception, expected_balance",
     [
-        ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, None, 1000000001000000000),
+        ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, None, 8000000001000000000),
         ("0x896c54023265f2c821f241BC694d8A0E1FA7DF2E", CONTRACT, None, 3570000000000000000),
-        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", CONTRACT, None, 15469999999000000000),
-        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", CONTRACT, None, 629546202581319287241),
+        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", CONTRACT, None, 8469999999000000000),
+        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", CONTRACT, None, 659546202581319287241),
         ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", CONTRACT, None, 950000000000000000),
-        ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", CONTRACT, None, 32963423288412440122),
+        ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", CONTRACT, None, 41624579772130211939),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", CONTRACT, None, 0),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", "Eeaa7E347ee4557f9a6F71C", InvalidArgumentError, 0),
     ],
 )
 @vcr_c.use_cassette("bsc/get_token_balance.yaml")
 async def test_get_token_balance(
     bsc_client: AioTxBSCClient, wallet_address, contract, expected_exception, expected_balance
@@ -99,16 +106,16 @@
 
 
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_count",
     [
         ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", None, 0),
         ("0x896c54023265f2c821f241BC694d8A0E1FA7DF2E", None, 0),
-        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", None, 102),
-        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", None, 1751),
+        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", None, 132),
+        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", None, 1788),
         ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", None, 17),
         ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", None, 1),
         ("2dbB5a4c235164B9f772179A43faca2c71a8abDB", InvalidArgumentError, 0),
         ("0x2dbB5a4c235164B9f772179A43faca2c71a8ab", InvalidArgumentError, 0),
     ],
 )
 @vcr_c.use_cassette("bsc/get_transaction_count.yaml")
@@ -122,15 +129,15 @@
         assert expected_count == count
 
 
 @vcr_c.use_cassette("bsc/get_gas_price.yaml")
 async def test_send_get_gas_price(bsc_client: AioTxBSCClient):
     result = await bsc_client.get_gas_price()
     assert isinstance(result, int)
-    assert result == 5000000000
+    assert result == 5050000000
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, amount, gas_price, gas_limit, expected_exception",
     [
         (
             "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
@@ -212,15 +219,15 @@
     else:
         result = await bsc_client.send(private_key, to_address, wei_amount)
         assert isinstance(result, str)
 
 
 @vcr_c.use_cassette("bsc/send_transaction_with_custom_nonce.yaml")
 async def test_send_transaction_with_custom_nonce(bsc_client: AioTxBSCClient):
-    wei_amount = bsc_client.to_wei(0.00001, "ether")
+    wei_amount = bsc_client.to_wei(0.00002, "ether")
     sender_address = bsc_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
     nonce = await bsc_client.get_transactions_count(sender_address)
     first_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, wei_amount, nonce=nonce)
     assert isinstance(first_tx, str)
     second_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, sender_address, wei_amount, nonce=nonce + 1)
     assert isinstance(second_tx, str)
 
@@ -281,20 +288,20 @@
             DESTINATION_ADDRESS,
             "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b",
             1,
             5,
             61000,
             TypeError,
         ),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, None),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 0.5, 5, 61000, None),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1000, 5, 61000, ReplacementTransactionUnderpriced),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 0, 61000, AioTxError),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 0, 5, 61000, ReplacementTransactionUnderpriced),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 0, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, None),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 0.5, 5, 61000, None),
     ],
 )
 @vcr_c.use_cassette("bsc/send_token_transaction.yaml")
 async def test_send_token_transaction(
     bsc_client: AioTxBSCClient, private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception
 ):
     """
```

### Comparing `aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py` & `aiotx-2.0.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_monitoring.py` & `aiotx-2.0.0/tests/test_evm/test_bsc/test_bsc_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_evm/test_eth/test_eth_client.py` & `aiotx-2.0.0/tests/test_evm/test_eth/test_eth_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 
 @vcr_c.use_cassette("eth/get_last_block.yaml")
 async def test_get_last_block(eth_client: AioTxETHClient):
     block_id = await eth_client.get_last_block_number()
     assert isinstance(block_id, int)
 
 
+@vcr_c.use_cassette("eth/get_chain_id.yaml")
+async def test_get_chain_id(eth_client: AioTxETHClient):
+    chain_id = await eth_client.get_chain_id()
+    assert isinstance(chain_id, int)
+    assert chain_id == 11155111
+
+
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_balance",
     [
         ("0x56ebc43d764761bc09d5918787672e2c8d46da5f", None, 22243749149992258),
         ("0xf663792Be0EdD00AFFB8BBe4Ac6d8185efD5671d", None, 72596311066831845012),
         ("0xA869aF2883DD6C881bC59594aDfB3e8b136321b4", None, 2360954490480603880),
         ("0xE27017DD9EF7e3D0A8321C2041Fc4402e89945b6", None, 9148320984250803464),
```

### Comparing `aiotx-1.3.0/tests/test_evm/test_eth/test_eth_input_decoding.py` & `aiotx-2.0.0/tests/test_evm/test_eth/test_eth_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_evm/test_eth/test_eth_monitoring.py` & `aiotx-2.0.0/tests/test_evm/test_eth/test_eth_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_client.py` & `aiotx-2.0.0/tests/test_utxo/test_btc/test_btc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_monitor.py` & `aiotx-2.0.0/tests/test_utxo/test_btc/test_btc_monitor.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_client.py` & `aiotx-2.0.0/tests/test_utxo/test_ltc/test_ltc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_monitor.py` & `aiotx-2.0.0/tests/test_utxo/test_ltc/test_ltc_monitor.py`

 * *Files identical despite different names*

