# Comparing `tmp/nautilus_trader-1.192.0.tar.gz` & `tmp/nautilus_trader-1.193.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus_trader-1.192.0.tar", max compression
+gzip compressed data, was "nautilus_trader-1.193.0.tar", max compression
```

## Comparing `nautilus_trader-1.192.0.tar` & `nautilus_trader-1.193.0.tar`

### file list

```diff
@@ -1,1129 +1,1129 @@
--rw-r--r--   0        0        0     7651 2024-05-18 09:12:24.907796 nautilus_trader-1.192.0/LICENSE
--rw-r--r--   0        0        0    25255 2024-05-18 09:12:24.907796 nautilus_trader-1.192.0/README.md
--rw-r--r--   0        0        0    12823 2024-05-18 09:12:24.907796 nautilus_trader-1.192.0/build.py
--rw-r--r--   0        0        0      663 2024-05-18 09:12:24.919796 nautilus_trader-1.192.0/nautilus_core/.cargo/config.toml
--rw-r--r--   0        0        0   138403 2024-05-18 09:12:24.919796 nautilus_trader-1.192.0/nautilus_core/Cargo.lock
--rw-r--r--   0        0        0     2305 2024-05-18 09:12:24.919796 nautilus_trader-1.192.0/nautilus_core/Cargo.toml
--rw-r--r--   0        0        0     7652 2024-05-18 09:12:24.919796 nautilus_trader-1.192.0/nautilus_core/LICENSE
--rw-r--r--   0        0        0     1248 2024-05-18 09:12:24.919796 nautilus_trader-1.192.0/nautilus_core/README.md
--rw-r--r--   0        0        0      967 2024-05-18 09:12:24.919796 nautilus_trader-1.192.0/nautilus_core/accounting/Cargo.toml
--rw-r--r--   0        0        0     9225 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/account/base.rs
--rw-r--r--   0        0        0    20176 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/account/cash.rs
--rw-r--r--   0        0        0    22074 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/account/margin.rs
--rw-r--r--   0        0        0     1015 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/account/mod.rs
--rw-r--r--   0        0        0     2376 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/account/stubs.rs
--rw-r--r--   0        0        0     1673 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/lib.rs
--rw-r--r--   0        0        0     6160 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/python/cash.rs
--rw-r--r--   0        0        0     8441 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/python/margin.rs
--rw-r--r--   0        0        0     1557 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/python/mod.rs
--rw-r--r--   0        0        0     2609 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/python/transformer.rs
--rw-r--r--   0        0        0     2542 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/accounting/src/stubs.rs
--rw-r--r--   0        0        0     1659 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/Cargo.toml
--rw-r--r--   0        0        0     1179 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/bin/sandbox.rs
--rw-r--r--   0        0        0     2250 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/common.rs
--rw-r--r--   0        0        0    44222 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/decode.rs
--rw-r--r--   0        0        0     3482 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/enums.rs
--rw-r--r--   0        0        0    15963 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/live.rs
--rw-r--r--   0        0        0    11607 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/loader.rs
--rw-r--r--   0        0        0     1113 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/mod.rs
--rw-r--r--   0        0        0    10104 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/publishers.json
--rw-r--r--   0        0        0     5323 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/enums.rs
--rw-r--r--   0        0        0    19510 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/historical.rs
--rw-r--r--   0        0        0     8154 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/live.rs
--rw-r--r--   0        0        0    13415 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/loader.rs
--rw-r--r--   0        0        0     1702 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/mod.rs
--rw-r--r--   0        0        0     7715 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/types.rs
--rw-r--r--   0        0        0     6477 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/symbology.rs
--rw-r--r--   0        0        0       81 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.cbbo.dbn.zst
--rw-r--r--   0        0        0      693 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst
--rw-r--r--   0        0        0      673 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst
--rw-r--r--   0        0        0      661 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst
--rw-r--r--   0        0        0      465 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn
--rw-r--r--   0        0        0      174 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn.zst
--rw-r--r--   0        0        0      192 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-1.dbn.zst
--rw-r--r--   0        0        0      374 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-10.dbn.zst
--rw-r--r--   0        0        0      103 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1d.dbn.zst
--rw-r--r--   0        0        0      186 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1h.dbn.zst
--rw-r--r--   0        0        0      165 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1m.dbn.zst
--rw-r--r--   0        0        0      157 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1s.dbn.zst
--rw-r--r--   0        0        0      139 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.statistics.dbn.zst
--rw-r--r--   0        0        0      197 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.tbbo.dbn.zst
--rw-r--r--   0        0        0      173 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.trades.dbn.zst
--rw-r--r--   0        0        0     6857 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/types.rs
--rw-r--r--   0        0        0     1771 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/adapters/src/lib.rs
--rw-r--r--   0        0        0     1234 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/Cargo.toml
--rw-r--r--   0        0        0     2046 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/build.rs
--rw-r--r--   0        0        0      484 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/cbindgen.toml
--rw-r--r--   0        0        0      807 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/cbindgen_cython.toml
--rw-r--r--   0        0        0     6213 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/src/engine.rs
--rw-r--r--   0        0        0     1701 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/src/lib.rs
--rw-r--r--   0        0        0     8782 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/backtest/src/matching_engine.rs
--rw-r--r--   0        0        0      669 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/cli/Cargo.toml
--rw-r--r--   0        0        0     1289 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/cli/src/bin/cli.rs
--rw-r--r--   0        0        0      902 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/cli/src/database/mod.rs
--rw-r--r--   0        0        0     2258 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/cli/src/database/postgres.rs
--rw-r--r--   0        0        0     1198 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/cli/src/lib.rs
--rw-r--r--   0        0        0     2230 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/cli/src/opt.rs
--rw-r--r--   0        0        0       65 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/clippy.toml
--rw-r--r--   0        0        0     1611 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/common/Cargo.toml
--rw-r--r--   0        0        0     2759 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/common/build.rs
--rw-r--r--   0        0        0      548 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/common/cbindgen.toml
--rw-r--r--   0        0        0      823 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/common/cbindgen_cython.toml
--rw-r--r--   0        0        0    96074 2024-05-18 09:12:24.923796 nautilus_trader-1.192.0/nautilus_core/common/src/cache/core.rs
--rw-r--r--   0        0        0     8710 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/cache/database.rs
--rw-r--r--   0        0        0     1086 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/cache/mod.rs
--rw-r--r--   0        0        0    11713 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/clock.rs
--rw-r--r--   0        0        0     9339 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/enums.rs
--rw-r--r--   0        0        0     8014 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/factories.rs
--rw-r--r--   0        0        0    12261 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/ffi/clock.rs
--rw-r--r--   0        0        0     3086 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/ffi/enums.rs
--rw-r--r--   0        0        0     5911 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/ffi/logging.rs
--rw-r--r--   0        0        0     1014 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/ffi/mod.rs
--rw-r--r--   0        0        0     1771 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/ffi/timer.rs
--rw-r--r--   0        0        0     5028 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/generators/client_order_id.rs
--rw-r--r--   0        0        0     1380 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/generators/mod.rs
--rw-r--r--   0        0        0     4982 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/generators/order_list_id.rs
--rw-r--r--   0        0        0     5582 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/generators/position_id.rs
--rw-r--r--   0        0        0     3412 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/handlers.rs
--rw-r--r--   0        0        0     2956 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/interface/account.rs
--rw-r--r--   0        0        0      977 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/interface/mod.rs
--rw-r--r--   0        0        0     2065 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/lib.rs
--rw-r--r--   0        0        0     7640 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/logging/headers.rs
--rw-r--r--   0        0        0    23893 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/logging/logger.rs
--rw-r--r--   0        0        0     5414 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/logging/mod.rs
--rw-r--r--   0        0        0     7744 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/logging/writer.rs
--rw-r--r--   0        0        0    20886 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/msgbus/core.rs
--rw-r--r--   0        0        0     1664 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/msgbus/database.rs
--rw-r--r--   0        0        0     1046 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/msgbus/mod.rs
--rw-r--r--   0        0        0     5841 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/python/clock.rs
--rw-r--r--   0        0        0     4513 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/python/enums.rs
--rw-r--r--   0        0        0     4896 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/python/logging.rs
--rw-r--r--   0        0        0     1999 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/python/mod.rs
--rw-r--r--   0        0        0     3479 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/python/timer.rs
--rw-r--r--   0        0        0     2848 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/python/versioning.rs
--rw-r--r--   0        0        0     1717 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/runtime.rs
--rw-r--r--   0        0        0     1374 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/stubs.rs
--rw-r--r--   0        0        0     2496 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/testing.rs
--rw-r--r--   0        0        0    17675 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/timer.rs
--rw-r--r--   0        0        0     5943 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/common/src/xrate.rs
--rw-r--r--   0        0        0      850 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/Cargo.toml
--rw-r--r--   0        0        0     2755 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/build.rs
--rw-r--r--   0        0        0      717 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/cbindgen.toml
--rw-r--r--   0        0        0      824 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/cbindgen_cython.toml
--rw-r--r--   0        0        0    18382 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/correctness.rs
--rw-r--r--   0        0        0     9172 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/datetime.rs
--rw-r--r--   0        0        0     2799 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/deserialization.rs
--rw-r--r--   0        0        0     1156 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/equality.rs
--rw-r--r--   0        0        0     5695 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/ffi/cvec.rs
--rw-r--r--   0        0        0     1248 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/ffi/datetime.rs
--rw-r--r--   0        0        0     1031 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/ffi/mod.rs
--rw-r--r--   0        0        0     8229 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/ffi/parsing.rs
--rw-r--r--   0        0        0     6642 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/ffi/string.rs
--rw-r--r--   0        0        0     3986 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/ffi/uuid.rs
--rw-r--r--   0        0        0     1924 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/lib.rs
--rw-r--r--   0        0        0     1409 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/message.rs
--rw-r--r--   0        0        0     8197 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/nanos.rs
--rw-r--r--   0        0        0     3425 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/parsing.rs
--rw-r--r--   0        0        0     1067 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/python/casing.rs
--rw-r--r--   0        0        0     2691 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/python/datetime.rs
--rw-r--r--   0        0        0     2894 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/python/mod.rs
--rw-r--r--   0        0        0     1407 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/python/serialization.rs
--rw-r--r--   0        0        0     3120 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/python/uuid.rs
--rw-r--r--   0        0        0     1814 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/serialization.rs
--rw-r--r--   0        0        0     8831 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/time.rs
--rw-r--r--   0        0        0     6040 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/core/src/uuid.rs
--rw-r--r--   0        0        0     1371 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/execution/Cargo.toml
--rw-r--r--   0        0        0     6813 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/execution/src/client.rs
--rw-r--r--   0        0        0     8306 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/execution/src/engine.rs
--rw-r--r--   0        0        0     1733 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/execution/src/lib.rs
--rw-r--r--   0        0        0    18827 2024-05-18 09:12:24.927796 nautilus_trader-1.192.0/nautilus_core/execution/src/matching_core.rs
--rw-r--r--   0        0        0     2761 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/cancel.rs
--rw-r--r--   0        0        0     2581 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/cancel_all.rs
--rw-r--r--   0        0        0     2561 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/cancel_batch.rs
--rw-r--r--   0        0        0     2809 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/mod.rs
--rw-r--r--   0        0        0     3416 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/modify.rs
--rw-r--r--   0        0        0     2757 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/query.rs
--rw-r--r--   0        0        0     3171 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/submit.rs
--rw-r--r--   0        0        0     3214 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/execution/src/messages/submit_list.rs
--rw-r--r--   0        0        0      746 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/Cargo.toml
--rw-r--r--   0        0        0     8897 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/ama.rs
--rw-r--r--   0        0        0     6979 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/dema.rs
--rw-r--r--   0        0        0     6902 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/ema.rs
--rw-r--r--   0        0        0     8322 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/hma.rs
--rw-r--r--   0        0        0     2875 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/mod.rs
--rw-r--r--   0        0        0     6925 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/rma.rs
--rw-r--r--   0        0        0     6142 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/sma.rs
--rw-r--r--   0        0        0     7476 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/vidya.rs
--rw-r--r--   0        0        0     7727 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/average/wma.rs
--rw-r--r--   0        0        0     6332 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/book/imbalance.rs
--rw-r--r--   0        0        0      940 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/book/mod.rs
--rw-r--r--   0        0        0     3206 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/indicator.rs
--rw-r--r--   0        0        0     1773 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/lib.rs
--rw-r--r--   0        0        0     7660 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/aroon.rs
--rw-r--r--   0        0        0     5019 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/bias.rs
--rw-r--r--   0        0        0     7008 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/cmo.rs
--rw-r--r--   0        0        0      970 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/mod.rs
--rw-r--r--   0        0        0     7876 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/rsi.rs
--rw-r--r--   0        0        0     2922 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/ama.rs
--rw-r--r--   0        0        0     2799 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/dema.rs
--rw-r--r--   0        0        0     2880 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/ema.rs
--rw-r--r--   0        0        0     2759 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/hma.rs
--rw-r--r--   0        0        0      976 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/mod.rs
--rw-r--r--   0        0        0     2865 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/rma.rs
--rw-r--r--   0        0        0     2765 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/sma.rs
--rw-r--r--   0        0        0     3101 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/vidya.rs
--rw-r--r--   0        0        0     2755 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/wma.rs
--rw-r--r--   0        0        0     2221 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/book/imbalance.rs
--rw-r--r--   0        0        0      903 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/book/mod.rs
--rw-r--r--   0        0        0     2217 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/mod.rs
--rw-r--r--   0        0        0     2901 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/aroon.rs
--rw-r--r--   0        0        0     2682 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/bias.rs
--rw-r--r--   0        0        0     2748 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/cmo.rs
--rw-r--r--   0        0        0      939 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/mod.rs
--rw-r--r--   0        0        0     2583 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/rsi.rs
--rw-r--r--   0        0        0     2005 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs
--rw-r--r--   0        0        0      910 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/ratio/mod.rs
--rw-r--r--   0        0        0     3005 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/volatility/atr.rs
--rw-r--r--   0        0        0      897 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/python/volatility/mod.rs
--rw-r--r--   0        0        0     8102 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs
--rw-r--r--   0        0        0      938 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/ratio/mod.rs
--rw-r--r--   0        0        0     5818 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/stubs.rs
--rw-r--r--   0        0        0     1509 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/testing.rs
--rw-r--r--   0        0        0     9258 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/volatility/atr.rs
--rw-r--r--   0        0        0      930 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/indicators/src/volatility/mod.rs
--rw-r--r--   0        0        0     1527 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/Cargo.toml
--rw-r--r--   0        0        0     1855 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/lib.rs
--rw-r--r--   0        0        0     1430 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/mod.rs
--rw-r--r--   0        0        0     3422 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/redis/cache.rs
--rw-r--r--   0        0        0     1065 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/redis/mod.rs
--rw-r--r--   0        0        0     1960 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs
--rw-r--r--   0        0        0     6286 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs
--rw-r--r--   0        0        0      908 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/sql/mod.rs
--rw-r--r--   0        0        0    21364 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/redis/cache.rs
--rw-r--r--   0        0        0    10578 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/redis/mod.rs
--rw-r--r--   0        0        0     7063 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/redis/msgbus.rs
--rw-r--r--   0        0        0    11170 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/cache_database.rs
--rw-r--r--   0        0        0     1137 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/mod.rs
--rw-r--r--   0        0        0      987 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/general.rs
--rw-r--r--   0        0        0    26965 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/instruments.rs
--rw-r--r--   0        0        0      953 2024-05-18 09:12:24.931796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/mod.rs
--rw-r--r--   0        0        0    14238 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/orders.rs
--rw-r--r--   0        0        0     1805 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/types.rs
--rw-r--r--   0        0        0    10685 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/pg.rs
--rw-r--r--   0        0        0    17820 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/queries.rs
--rw-r--r--   0        0        0    10218 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs
--rw-r--r--   0        0        0     1430 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/Cargo.toml
--rw-r--r--   0        0        0      400 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/benches/criterion_fixed_precision_benchmark.rs
--rw-r--r--   0        0        0      225 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/benches/iai_fixed_precision_benchmark.rs
--rw-r--r--   0        0        0     2757 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/build.rs
--rw-r--r--   0        0        0     1617 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/cbindgen.toml
--rw-r--r--   0        0        0     1839 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/cbindgen_cython.toml
--rw-r--r--   0        0        0    33910 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/currencies.rs
--rw-r--r--   0        0        0    16919 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/bar.rs
--rw-r--r--   0        0        0     8316 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/delta.rs
--rw-r--r--   0        0        0     8465 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/deltas.rs
--rw-r--r--   0        0        0    11159 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/depth.rs
--rw-r--r--   0        0        0     3040 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/mod.rs
--rw-r--r--   0        0        0     6445 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/order.rs
--rw-r--r--   0        0        0     8044 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/quote.rs
--rw-r--r--   0        0        0     9402 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/stubs.rs
--rw-r--r--   0        0        0     6693 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/data/trade.rs
--rw-r--r--   0        0        0    30931 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/enums.rs
--rw-r--r--   0        0        0      940 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/account/mod.rs
--rw-r--r--   0        0        0     4946 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/account/state.rs
--rw-r--r--   0        0        0     4078 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/account/stubs.rs
--rw-r--r--   0        0        0     1012 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/mod.rs
--rw-r--r--   0        0        0     7222 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/accepted.rs
--rw-r--r--   0        0        0     7827 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/cancel_rejected.rs
--rw-r--r--   0        0        0     7103 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/canceled.rs
--rw-r--r--   0        0        0     6601 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/denied.rs
--rw-r--r--   0        0        0     6445 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/emulated.rs
--rw-r--r--   0        0        0     5516 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/event.rs
--rw-r--r--   0        0        0     7542 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/expired.rs
--rw-r--r--   0        0        0    11143 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/filled.rs
--rw-r--r--   0        0        0    18098 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/initialized.rs
--rw-r--r--   0        0        0     3446 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/mod.rs
--rw-r--r--   0        0        0     7813 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/modify_rejected.rs
--rw-r--r--   0        0        0     7474 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/pending_cancel.rs
--rw-r--r--   0        0        0     7492 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/pending_update.rs
--rw-r--r--   0        0        0     7172 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/rejected.rs
--rw-r--r--   0        0        0     6699 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/released.rs
--rw-r--r--   0        0        0    11494 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/stubs.rs
--rw-r--r--   0        0        0     6745 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/submitted.rs
--rw-r--r--   0        0        0     7591 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/triggered.rs
--rw-r--r--   0        0        0     8427 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/order/updated.rs
--rw-r--r--   0        0        0     1987 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/position/changed.rs
--rw-r--r--   0        0        0     2106 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/position/closed.rs
--rw-r--r--   0        0        0     1200 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/position/mod.rs
--rw-r--r--   0        0        0     1791 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/position/opened.rs
--rw-r--r--   0        0        0     1985 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/events/position/state.rs
--rw-r--r--   0        0        0     6050 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/bar.rs
--rw-r--r--   0        0        0     1845 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/delta.rs
--rw-r--r--   0        0        0     3549 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/deltas.rs
--rw-r--r--   0        0        0     3787 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/depth.rs
--rw-r--r--   0        0        0      988 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/mod.rs
--rw-r--r--   0        0        0     2417 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/order.rs
--rw-r--r--   0        0        0     2745 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/quote.rs
--rw-r--r--   0        0        0     2203 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/trade.rs
--rw-r--r--   0        0        0    15015 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/enums.rs
--rw-r--r--   0        0        0      899 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/events/mod.rs
--rw-r--r--   0        0        0     4681 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/events/order.rs
--rw-r--r--   0        0        0     3279 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/account_id.rs
--rw-r--r--   0        0        0     2234 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/client_id.rs
--rw-r--r--   0        0        0     1398 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs
--rw-r--r--   0        0        0     1381 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/component_id.rs
--rw-r--r--   0        0        0     1412 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs
--rw-r--r--   0        0        0     4223 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1177 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/mod.rs
--rw-r--r--   0        0        0     1384 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs
--rw-r--r--   0        0        0     1374 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/position_id.rs
--rw-r--r--   0        0        0     1374 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs
--rw-r--r--   0        0        0     1343 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/symbol.rs
--rw-r--r--   0        0        0     1603 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs
--rw-r--r--   0        0        0     1360 2024-05-18 09:12:24.935796 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs
--rw-r--r--   0        0        0     2003 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/venue.rs
--rw-r--r--   0        0        0     1391 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs
--rw-r--r--   0        0        0      903 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/instruments/mod.rs
--rw-r--r--   0        0        0     5668 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/instruments/synthetic.rs
--rw-r--r--   0        0        0     1073 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/mod.rs
--rw-r--r--   0        0        0     8567 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/orderbook/book.rs
--rw-r--r--   0        0        0     3621 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/orderbook/level.rs
--rw-r--r--   0        0        0      913 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/orderbook/mod.rs
--rw-r--r--   0        0        0     5719 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/currency.rs
--rw-r--r--   0        0        0      950 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/mod.rs
--rw-r--r--   0        0        0     1596 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/money.rs
--rw-r--r--   0        0        0     1589 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/price.rs
--rw-r--r--   0        0        0     1845 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/quantity.rs
--rw-r--r--   0        0        0     4561 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/account_id.rs
--rw-r--r--   0        0        0     2846 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/client_id.rs
--rw-r--r--   0        0        0     4794 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/client_order_id.rs
--rw-r--r--   0        0        0     2897 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/component_id.rs
--rw-r--r--   0        0        0     2899 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs
--rw-r--r--   0        0        0     4866 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1909 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/macros.rs
--rw-r--r--   0        0        0     3032 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/mod.rs
--rw-r--r--   0        0        0     2899 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/order_list_id.rs
--rw-r--r--   0        0        0     2874 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/position_id.rs
--rw-r--r--   0        0        0     4369 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/strategy_id.rs
--rw-r--r--   0        0        0     4518 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/stubs.rs
--rw-r--r--   0        0        0     3053 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/symbol.rs
--rw-r--r--   0        0        0     4233 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/trade_id.rs
--rw-r--r--   0        0        0     3598 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/trader_id.rs
--rw-r--r--   0        0        0     3604 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/venue.rs
--rw-r--r--   0        0        0     2905 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/venue_order_id.rs
--rw-r--r--   0        0        0    11059 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/any.rs
--rw-r--r--   0        0        0     7700 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/crypto_future.rs
--rw-r--r--   0        0        0     7750 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/crypto_perpetual.rs
--rw-r--r--   0        0        0     7499 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/currency_pair.rs
--rw-r--r--   0        0        0     6626 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/equity.rs
--rw-r--r--   0        0        0     7324 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/futures_contract.rs
--rw-r--r--   0        0        0     7448 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/futures_spread.rs
--rw-r--r--   0        0        0     5480 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/mod.rs
--rw-r--r--   0        0        0     7574 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/options_contract.rs
--rw-r--r--   0        0        0     7439 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/options_spread.rs
--rw-r--r--   0        0        0    13302 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/stubs.rs
--rw-r--r--   0        0        0     6493 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/instruments/synthetic.rs
--rw-r--r--   0        0        0     2074 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/lib.rs
--rw-r--r--   0        0        0     1595 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/macros.rs
--rw-r--r--   0        0        0     3536 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/aggregation.rs
--rw-r--r--   0        0        0     4309 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/analysis.rs
--rw-r--r--   0        0        0    23019 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/book.rs
--rw-r--r--   0        0        0     2836 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/display.rs
--rw-r--r--   0        0        0     1988 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/error.rs
--rw-r--r--   0        0        0    22495 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/ladder.rs
--rw-r--r--   0        0        0    13057 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/level.rs
--rw-r--r--   0        0        0     1067 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/mod.rs
--rw-r--r--   0        0        0    24505 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/any.rs
--rw-r--r--   0        0        0    31687 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/base.rs
--rw-r--r--   0        0        0     9307 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/default.rs
--rw-r--r--   0        0        0    14285 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/limit.rs
--rw-r--r--   0        0        0    11226 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/limit_if_touched.rs
--rw-r--r--   0        0        0     4555 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/list.rs
--rw-r--r--   0        0        0    11942 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/market.rs
--rw-r--r--   0        0        0    10843 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/market_if_touched.rs
--rw-r--r--   0        0        0    10035 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/market_to_limit.rs
--rw-r--r--   0        0        0     1270 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/mod.rs
--rw-r--r--   0        0        0    12288 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/stop_limit.rs
--rw-r--r--   0        0        0    10817 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/stop_market.rs
--rw-r--r--   0        0        0     6823 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/stubs.rs
--rw-r--r--   0        0        0    11871 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/trailing_stop_limit.rs
--rw-r--r--   0        0        0    11317 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/orders/trailing_stop_market.rs
--rw-r--r--   0        0        0     3061 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/polymorphism.rs
--rw-r--r--   0        0        0    71452 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/position.rs
--rw-r--r--   0        0        0     7166 2024-05-18 09:12:24.939797 nautilus_trader-1.192.0/nautilus_core/model/src/python/common.rs
--rw-r--r--   0        0        0    12321 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/bar.rs
--rw-r--r--   0        0        0    10587 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/delta.rs
--rw-r--r--   0        0        0     4435 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/deltas.rs
--rw-r--r--   0        0        0     8920 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/depth.rs
--rw-r--r--   0        0        0     3425 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/mod.rs
--rw-r--r--   0        0        0     5608 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/order.rs
--rw-r--r--   0        0        0    14445 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/quote.rs
--rw-r--r--   0        0        0    12629 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/data/trade.rs
--rw-r--r--   0        0        0    44501 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/enums.rs
--rw-r--r--   0        0        0      899 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/account/mod.rs
--rw-r--r--   0        0        0     6244 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/account/state.rs
--rw-r--r--   0        0        0      966 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/mod.rs
--rw-r--r--   0        0        0     3621 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/accepted.rs
--rw-r--r--   0        0        0     4116 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs
--rw-r--r--   0        0        0     3893 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/canceled.rs
--rw-r--r--   0        0        0     3369 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/denied.rs
--rw-r--r--   0        0        0     3184 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/emulated.rs
--rw-r--r--   0        0        0     3888 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/expired.rs
--rw-r--r--   0        0        0     7686 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/filled.rs
--rw-r--r--   0        0        0    10715 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/initialized.rs
--rw-r--r--   0        0        0     5538 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/mod.rs
--rw-r--r--   0        0        0     4127 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/modify_rejected.rs
--rw-r--r--   0        0        0     3789 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/pending_cancel.rs
--rw-r--r--   0        0        0     3789 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/pending_update.rs
--rw-r--r--   0        0        0     3644 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/rejected.rs
--rw-r--r--   0        0        0     3343 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/released.rs
--rw-r--r--   0        0        0     3334 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/submitted.rs
--rw-r--r--   0        0        0     3892 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/triggered.rs
--rw-r--r--   0        0        0     4530 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/updated.rs
--rw-r--r--   0        0        0     3628 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1993 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/identifiers/mod.rs
--rw-r--r--   0        0        0     3411 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/identifiers/trade_id.rs
--rw-r--r--   0        0        0     9563 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/crypto_future.rs
--rw-r--r--   0        0        0     9055 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs
--rw-r--r--   0        0        0     8593 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/currency_pair.rs
--rw-r--r--   0        0        0     7022 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/equity.rs
--rw-r--r--   0        0        0     8544 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/futures_contract.rs
--rw-r--r--   0        0        0     8806 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/futures_spread.rs
--rw-r--r--   0        0        0     3614 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/mod.rs
--rw-r--r--   0        0        0     9059 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/options_contract.rs
--rw-r--r--   0        0        0     8804 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/options_spread.rs
--rw-r--r--   0        0        0     3531 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/macros.rs
--rw-r--r--   0        0        0     7351 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/mod.rs
--rw-r--r--   0        0        0     6786 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orderbook/book.rs
--rw-r--r--   0        0        0     2104 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orderbook/level.rs
--rw-r--r--   0        0        0      983 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orderbook/mod.rs
--rw-r--r--   0        0        0    22070 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/limit.rs
--rw-r--r--   0        0        0     4518 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/limit_if_touched.rs
--rw-r--r--   0        0        0    18609 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/market.rs
--rw-r--r--   0        0        0     4433 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/market_if_touched.rs
--rw-r--r--   0        0        0     4159 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/market_to_limit.rs
--rw-r--r--   0        0        0     4422 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/mod.rs
--rw-r--r--   0        0        0    22168 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/stop_limit.rs
--rw-r--r--   0        0        0     4412 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/stop_market.rs
--rw-r--r--   0        0        0     4750 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs
--rw-r--r--   0        0        0     4610 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs
--rw-r--r--   0        0        0    12642 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/position.rs
--rw-r--r--   0        0        0     6219 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/types/balance.rs
--rw-r--r--   0        0        0     5123 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/types/currency.rs
--rw-r--r--   0        0        0     1062 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/types/mod.rs
--rw-r--r--   0        0        0    14239 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/types/money.rs
--rw-r--r--   0        0        0    14708 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/types/price.rs
--rw-r--r--   0        0        0    14615 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/python/types/quantity.rs
--rw-r--r--   0        0        0     5414 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/stubs.rs
--rw-r--r--   0        0        0     5786 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/balance.rs
--rw-r--r--   0        0        0     7530 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/currency.rs
--rw-r--r--   0        0        0     6622 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/fixed.rs
--rw-r--r--   0        0        0     1118 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/mod.rs
--rw-r--r--   0        0        0    11756 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/money.rs
--rw-r--r--   0        0        0    14431 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/price.rs
--rw-r--r--   0        0        0    14504 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/quantity.rs
--rw-r--r--   0        0        0     1475 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/types/stubs.rs
--rw-r--r--   0        0        0     3064 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/model/src/venues.rs
--rw-r--r--   0        0        0     1036 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/network/Cargo.toml
--rw-r--r--   0        0        0     1655 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/network/benches/test_client.rs
--rw-r--r--   0        0        0     1374 2024-05-18 09:12:24.943796 nautilus_trader-1.192.0/nautilus_core/network/benches/test_server.rs
--rw-r--r--   0        0        0    12459 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/http.rs
--rw-r--r--   0        0        0     1802 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/lib.rs
--rw-r--r--   0        0        0     1475 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/python/mod.rs
--rw-r--r--   0        0        0     6239 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/clock.rs
--rw-r--r--   0        0        0     5417 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/gcra.rs
--rw-r--r--   0        0        0     8865 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/mod.rs
--rw-r--r--   0        0        0     4079 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/nanos.rs
--rw-r--r--   0        0        0     9739 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/quota.rs
--rw-r--r--   0        0        0    23594 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/socket.rs
--rw-r--r--   0        0        0    28915 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/src/websocket.rs
--rw-r--r--   0        0        0       18 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/.gitignore
--rw-r--r--   0        0        0     2862 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md
--rw-r--r--   0        0        0     2061 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/Cargo.toml
--rw-r--r--   0        0        0     1093 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/LICENSE
--rw-r--r--   0        0        0     2861 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/README.md
--rw-r--r--   0        0        0      268 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/rustfmt.toml
--rw-r--r--   0        0        0     6900 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/compat.rs
--rw-r--r--   0        0        0     2747 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/connect.rs
--rw-r--r--   0        0        0     5469 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs
--rw-r--r--   0        0        0    14303 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/lib.rs
--rw-r--r--   0        0        0     2854 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/stream.rs
--rw-r--r--   0        0        0     8647 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/tls.rs
--rw-r--r--   0        0        0     1300 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/Cargo.toml
--rw-r--r--   0        0        0     3658 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/benches/bench_persistence.rs
--rw-r--r--   0        0        0    12962 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/bar.rs
--rw-r--r--   0        0        0    15825 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/delta.rs
--rw-r--r--   0        0        0    41488 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/depth.rs
--rw-r--r--   0        0        0     4662 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/mod.rs
--rw-r--r--   0        0        0    12628 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/quote.rs
--rw-r--r--   0        0        0    12946 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/trade.rs
--rw-r--r--   0        0        0    10343 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/backend/kmerge_batch.rs
--rw-r--r--   0        0        0     1025 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/backend/mod.rs
--rw-r--r--   0        0        0     8048 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/backend/session.rs
--rw-r--r--   0        0        0     1736 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/lib.rs
--rw-r--r--   0        0        0      922 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/backend/mod.rs
--rw-r--r--   0        0        0     4265 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/backend/session.rs
--rw-r--r--   0        0        0    12804 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/backend/transformer.rs
--rw-r--r--   0        0        0     1696 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/mod.rs
--rw-r--r--   0        0        0     2824 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/bar.rs
--rw-r--r--   0        0        0     3031 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/delta.rs
--rw-r--r--   0        0        0      942 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/mod.rs
--rw-r--r--   0        0        0     2955 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/quote.rs
--rw-r--r--   0        0        0     2952 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/trade.rs
--rw-r--r--   0        0        0    10633 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/tests/test_catalog.rs
--rw-r--r--   0        0        0     2159 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/persistence/tests/test_util.rs
--rw-r--r--   0        0        0     1469 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/pyo3/Cargo.toml
--rw-r--r--   0        0        0     4929 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/pyo3/src/lib.rs
--rw-r--r--   0        0        0       50 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/rust-toolchain.toml
--rw-r--r--   0        0        0      225 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_core/rustfmt.toml
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/__init__.pxd
--rw-r--r--   0        0        0     2270 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/__init__.pxd
--rw-r--r--   0        0        0     1414 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/__init__.py
--rw-r--r--   0        0        0     4195 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/base.pxd
--rw-r--r--   0        0        0    14679 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/base.pyx
--rw-r--r--   0        0        0     1740 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/betting.pxd
--rw-r--r--   0        0        0     4117 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/betting.pyx
--rw-r--r--   0        0        0     2013 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/cash.pxd
--rw-r--r--   0        0        0    13601 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/cash.pyx
--rw-r--r--   0        0        0     3309 2024-05-18 09:12:24.947796 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/margin.pxd
--rw-r--r--   0        0        0    22719 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/margin.pyx
--rw-r--r--   0        0        0     1489 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/calculators.pxd
--rw-r--r--   0        0        0    10740 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/calculators.pyx
--rw-r--r--   0        0        0     2111 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/error.py
--rw-r--r--   0        0        0     1089 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/factory.pxd
--rw-r--r--   0        0        0     4065 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/factory.pyx
--rw-r--r--   0        0        0     2653 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/manager.pxd
--rw-r--r--   0        0        0    22688 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/accounting/manager.pyx
--rw-r--r--   0        0        0     1153 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/_template/__init__.py
--rw-r--r--   0        0        0     1013 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/_template/core.py
--rw-r--r--   0        0        0    14665 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/_template/data.py
--rw-r--r--   0        0        0     7371 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/_template/execution.py
--rw-r--r--   0        0        0     2601 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/_template/providers.py
--rw-r--r--   0        0        0      945 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/__init__.py
--rw-r--r--   0        0        0    12517 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/client.py
--rw-r--r--   0        0        0     3924 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/common.py
--rw-r--r--   0        0        0     2529 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/config.py
--rw-r--r--   0        0        0     2038 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/constants.py
--rw-r--r--   0        0        0    12440 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/data.py
--rw-r--r--   0        0        0    10941 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/data_types.py
--rw-r--r--   0        0        0    42389 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/execution.py
--rw-r--r--   0        0        0     7519 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/factories.py
--rw-r--r--   0        0        0     1257 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/orderbook.pxd
--rw-r--r--   0        0        0     1770 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/orderbook.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/__init__.py
--rw-r--r--   0        0        0     3234 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/common.py
--rw-r--r--   0        0        0     4607 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/core.py
--rw-r--r--   0        0        0    19955 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/requests.py
--rw-r--r--   0        0        0    19805 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/streaming.py
--rw-r--r--   0        0        0    12917 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/providers.py
--rw-r--r--   0        0        0     9450 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/sockets.py
--rw-r--r--   0        0        0      938 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/__init__.py
--rw-r--r--   0        0        0      997 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/constants.py
--rw-r--r--   0        0        0     1871 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/credentials.py
--rw-r--r--   0        0        0    39673 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/data.py
--rw-r--r--   0        0        0    19212 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/enums.py
--rw-r--r--   0        0        0    41882 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/execution.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/__init__.py
--rw-r--r--   0        0        0    10932 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/account.py
--rw-r--r--   0        0        0    22048 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/market.py
--rw-r--r--   0        0        0     1209 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/user.py
--rw-r--r--   0        0        0     2570 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/symbol.py
--rw-r--r--   0        0        0    15632 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/types.py
--rw-r--r--   0        0        0     3476 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/urls.py
--rw-r--r--   0        0        0     5353 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/config.py
--rw-r--r--   0        0        0    13709 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/factories.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.951797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/__init__.py
--rw-r--r--   0        0        0     6564 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/data.py
--rw-r--r--   0        0        0     6637 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/enums.py
--rw-r--r--   0        0        0    13348 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/execution.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/__init__.py
--rw-r--r--   0        0        0    16026 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/account.py
--rw-r--r--   0        0        0     3629 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/market.py
--rw-r--r--   0        0        0     1962 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/user.py
--rw-r--r--   0        0        0     4834 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/wallet.py
--rw-r--r--   0        0        0    17736 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/providers.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py
--rw-r--r--   0        0        0     7352 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/account.py
--rw-r--r--   0        0        0     7646 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/market.py
--rw-r--r--   0        0        0    15368 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/user.py
--rw-r--r--   0        0        0     1281 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py
--rw-r--r--   0        0        0     5070 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/types.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/__init__.py
--rw-r--r--   0        0        0    27258 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/account.py
--rw-r--r--   0        0        0     5511 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/client.py
--rw-r--r--   0        0        0     3295 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/endpoint.py
--rw-r--r--   0        0        0     1588 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/error.py
--rw-r--r--   0        0        0    32496 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/market.py
--rw-r--r--   0        0        0     7723 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/user.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/__init__.py
--rw-r--r--   0        0        0     5582 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/data.py
--rw-r--r--   0        0        0     5563 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/enums.py
--rw-r--r--   0        0        0    10055 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/execution.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/__init__.py
--rw-r--r--   0        0        0    26141 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/account.py
--rw-r--r--   0        0        0     6645 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/market.py
--rw-r--r--   0        0        0     1968 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/user.py
--rw-r--r--   0        0        0     4590 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/wallet.py
--rw-r--r--   0        0        0    13691 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/providers.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py
--rw-r--r--   0        0        0     3270 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/account.py
--rw-r--r--   0        0        0     6832 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/market.py
--rw-r--r--   0        0        0    11717 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/user.py
--rw-r--r--   0        0        0     1262 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/websocket/__init__.py
--rw-r--r--   0        0        0    16321 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/binance/websocket/client.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/__init__.py
--rw-r--r--   0        0        0     1572 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/constants.py
--rw-r--r--   0        0        0     1825 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/credentials.py
--rw-r--r--   0        0        0    10724 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/enums.py
--rw-r--r--   0        0        0     1502 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/error.py
--rw-r--r--   0        0        0     4018 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/parsing.py
--rw-r--r--   0        0        0     4250 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/symbol.py
--rw-r--r--   0        0        0     2623 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/urls.py
--rw-r--r--   0        0        0     3425 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/config.py
--rw-r--r--   0        0        0    28863 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/data.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py
--rw-r--r--   0        0        0     2369 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py
--rw-r--r--   0        0        0     2381 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py
--rw-r--r--   0        0        0     2293 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py
--rw-r--r--   0        0        0     2594 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py
--rw-r--r--   0        0        0     3608 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py
--rw-r--r--   0        0        0     2222 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py
--rw-r--r--   0        0        0     2060 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py
--rw-r--r--   0        0        0     3322 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py
--rw-r--r--   0        0        0     2132 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py
--rw-r--r--   0        0        0     2866 2024-05-18 09:12:24.955797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py
--rw-r--r--   0        0        0     2879 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py
--rw-r--r--   0        0        0     2525 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py
--rw-r--r--   0        0        0     3228 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py
--rw-r--r--   0        0        0     2433 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py
--rw-r--r--   0        0        0     2439 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py
--rw-r--r--   0        0        0     2466 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py
--rw-r--r--   0        0        0     2756 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py
--rw-r--r--   0        0        0     2987 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py
--rw-r--r--   0        0        0     2679 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py
--rw-r--r--   0        0        0    35884 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/execution.py
--rw-r--r--   0        0        0     9039 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/factories.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/__init__.py
--rw-r--r--   0        0        0    13207 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/account.py
--rw-r--r--   0        0        0     1963 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/asset.py
--rw-r--r--   0        0        0     6629 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/client.py
--rw-r--r--   0        0        0     1083 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/errors.py
--rw-r--r--   0        0        0     7979 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/market.py
--rw-r--r--   0        0        0     1180 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/user.py
--rw-r--r--   0        0        0    11303 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/providers.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py
--rw-r--r--   0        0        0     3413 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/account/balance.py
--rw-r--r--   0        0        0     1204 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py
--rw-r--r--   0        0        0     1947 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py
--rw-r--r--   0        0        0     2114 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/common.py
--rw-r--r--   0        0        0    15794 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/instrument.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py
--rw-r--r--   0        0        0     2184 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/kline.py
--rw-r--r--   0        0        0     4540 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py
--rw-r--r--   0        0        0     1088 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py
--rw-r--r--   0        0        0     4461 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py
--rw-r--r--   0        0        0     2476 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/trades.py
--rw-r--r--   0        0        0     9705 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/order.py
--rw-r--r--   0        0        0     2665 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/position.py
--rw-r--r--   0        0        0     4044 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/trade.py
--rw-r--r--   0        0        0    21528 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/ws.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/websocket/__init__.py
--rw-r--r--   0        0        0    11105 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/websocket/client.py
--rw-r--r--   0        0        0     1689 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/__init__.py
--rw-r--r--   0        0        0     2749 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/common.py
--rw-r--r--   0        0        0     2727 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/config.py
--rw-r--r--   0        0        0     1210 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/constants.py
--rw-r--r--   0        0        0    39036 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/data.py
--rw-r--r--   0        0        0     1315 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/enums.py
--rw-r--r--   0        0        0     6043 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/factories.py
--rw-r--r--   0        0        0    10712 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/loaders.py
--rw-r--r--   0        0        0    10149 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/providers.py
--rw-r--r--   0        0        0    10104 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/publishers.json
--rw-r--r--   0        0        0     1141 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/databento/types.py
--rw-r--r--   0        0        0     1193 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/env.py
--rw-r--r--   0        0        0      930 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/__init__.py
--rw-r--r--   0        0        0     1014 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py
--rw-r--r--   0        0        0     6415 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/account.py
--rw-r--r--   0        0        0    26860 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/client.py
--rw-r--r--   0        0        0    15878 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/common.py
--rw-r--r--   0        0        0     8356 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/connection.py
--rw-r--r--   0        0        0     7167 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/contract.py
--rw-r--r--   0        0        0     8724 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/error.py
--rw-r--r--   0        0        0    32019 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py
--rw-r--r--   0        0        0    10341 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/order.py
--rw-r--r--   0        0        0    43317 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py
--rw-r--r--   0        0        0     6988 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/common.py
--rw-r--r--   0        0        0     8127 2024-05-18 09:12:24.959797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/config.py
--rw-r--r--   0        0        0    17152 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/data.py
--rw-r--r--   0        0        0    38609 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/execution.py
--rw-r--r--   0        0        0     9005 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/factories.py
--rw-r--r--   0        0        0     7876 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/gateway.py
--rw-r--r--   0        0        0     1054 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py
--rw-r--r--   0        0        0    20988 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/historic/client.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py
--rw-r--r--   0        0        0     3579 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py
--rw-r--r--   0        0        0     3839 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py
--rw-r--r--   0        0        0    24117 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py
--rw-r--r--   0        0        0    12263 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/providers.py
--rw-r--r--   0        0        0     4904 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/web.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/__init__.py
--rw-r--r--   0        0        0     1500 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/config.py
--rw-r--r--   0        0        0     8063 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/execution.py
--rw-r--r--   0        0        0     2811 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/factory.py
--rw-r--r--   0        0        0      937 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/tardis/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/adapters/tardis/loaders.py
--rw-r--r--   0        0        0      978 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/__init__.py
--rw-r--r--   0        0        0    15183 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/analyzer.py
--rw-r--r--   0        0        0     5714 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/reporter.py
--rw-r--r--   0        0        0     3940 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistic.py
--rw-r--r--   0        0        0     2255 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/__init__.py
--rw-r--r--   0        0        0     1997 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/expectancy.py
--rw-r--r--   0        0        0     1705 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/long_ratio.py
--rw-r--r--   0        0        0     1468 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/loser_avg.py
--rw-r--r--   0        0        0     1514 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/loser_max.py
--rw-r--r--   0        0        0     1512 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/loser_min.py
--rw-r--r--   0        0        0     1563 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/profit_factor.py
--rw-r--r--   0        0        0     1399 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_avg.py
--rw-r--r--   0        0        0     1414 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_avg_loss.py
--rw-r--r--   0        0        0     1413 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_avg_win.py
--rw-r--r--   0        0        0     1716 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_volatility.py
--rw-r--r--   0        0        0     1323 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/risk_return_ratio.py
--rw-r--r--   0        0        0     1776 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/sharpe_ratio.py
--rw-r--r--   0        0        0     1883 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/sortino_ratio.py
--rw-r--r--   0        0        0     1498 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/win_rate.py
--rw-r--r--   0        0        0     1489 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/winner_avg.py
--rw-r--r--   0        0        0     1347 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/winner_max.py
--rw-r--r--   0        0        0     1494 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/winner_min.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/__init__.pxd
--rw-r--r--   0        0        0      946 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/__init__.py
--rw-r--r--   0        0        0     1868 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/__main__.py
--rw-r--r--   0        0        0     3840 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/auction.py
--rw-r--r--   0        0        0     9257 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/config.py
--rw-r--r--   0        0        0     1100 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/data_client.pxd
--rw-r--r--   0        0        0    13931 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/data_client.pyx
--rw-r--r--   0        0        0     2162 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/engine.pxd
--rw-r--r--   0        0        0    51527 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/engine.pyx
--rw-r--r--   0        0        0     7614 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/exchange.pxd
--rw-r--r--   0        0        0    31318 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/exchange.pyx
--rw-r--r--   0        0        0     1084 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/execution_client.pxd
--rw-r--r--   0        0        0     5264 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/execution_client.pyx
--rw-r--r--   0        0        0    12270 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/matching_engine.pxd
--rw-r--r--   0        0        0    98825 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/matching_engine.pyx
--rw-r--r--   0        0        0     2658 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/models.pxd
--rw-r--r--   0        0        0     8785 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/models.pyx
--rw-r--r--   0        0        0     1893 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/modules.pxd
--rw-r--r--   0        0        0     8483 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/modules.pyx
--rw-r--r--   0        0        0    15294 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/node.py
--rw-r--r--   0        0        0     3072 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/backtest/results.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/cache/__init__.pxd
--rw-r--r--   0        0        0     1220 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/cache/__init__.py
--rw-r--r--   0        0        0    10536 2024-05-18 09:12:24.963797 nautilus_trader-1.192.0/nautilus_trader/cache/base.pxd
--rw-r--r--   0        0        0    25831 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/base.pyx
--rw-r--r--   0        0        0     8701 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/cache.pxd
--rw-r--r--   0        0        0   135124 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/cache.pyx
--rw-r--r--   0        0        0     2884 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/config.py
--rw-r--r--   0        0        0     1104 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/database.pxd
--rw-r--r--   0        0        0    36283 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/database.pyx
--rw-r--r--   0        0        0     5051 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/facade.pxd
--rw-r--r--   0        0        0    11952 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/facade.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/postgres/__init__.py
--rw-r--r--   0        0        0     4086 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/postgres/adapter.py
--rw-r--r--   0        0        0     7632 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/cache/postgres/transformers.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/__init__.pxd
--rw-r--r--   0        0        0     1571 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/__init__.py
--rw-r--r--   0        0        0    11890 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/actor.pxd
--rw-r--r--   0        0        0    92278 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/actor.pyx
--rw-r--r--   0        0        0    11128 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/component.pxd
--rw-r--r--   0        0        0    88235 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/component.pyx
--rw-r--r--   0        0        0    16788 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/config.py
--rw-r--r--   0        0        0     1849 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/enums.py
--rw-r--r--   0        0        0    10785 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/executor.py
--rw-r--r--   0        0        0     9517 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/factories.pxd
--rw-r--r--   0        0        0    58923 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/factories.pyx
--rw-r--r--   0        0        0     1320 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/functions.py
--rw-r--r--   0        0        0     2143 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/generators.pxd
--rw-r--r--   0        0        0     7841 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/generators.pyx
--rw-r--r--   0        0        0     2723 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/messages.pxd
--rw-r--r--   0        0        0    11741 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/messages.pyx
--rw-r--r--   0        0        0    10413 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/common/providers.py
--rw-r--r--   0        0        0     5512 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/config/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/__init__.pxd
--rw-r--r--   0        0        0     1339 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/__init__.py
--rw-r--r--   0        0        0     1230 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/asynchronous.py
--rw-r--r--   0        0        0     3683 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/correctness.pxd
--rw-r--r--   0        0        0    37316 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/correctness.pyx
--rw-r--r--   0        0        0      897 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/data.pxd
--rw-r--r--   0        0        0     1954 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/data.pyx
--rw-r--r--   0        0        0     1363 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/datetime.pxd
--rw-r--r--   0        0        0     7616 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/datetime.pyx
--rw-r--r--   0        0        0     1230 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/fsm.pxd
--rw-r--r--   0        0        0     4364 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/fsm.pyx
--rw-r--r--   0        0        0     2511 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/includes/algorithms.h
--rw-r--r--   0        0        0      907 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/includes/backtest.h
--rw-r--r--   0        0        0    15890 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/includes/common.h
--rw-r--r--   0        0        0     3055 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/includes/core.h
--rw-r--r--   0        0        0    65849 2024-05-18 09:12:24.967797 nautilus_trader-1.192.0/nautilus_trader/core/includes/model.h
--rw-r--r--   0        0        0     2529 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/inspect.py
--rw-r--r--   0        0        0     2137 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/message.pxd
--rw-r--r--   0        0        0     6509 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/message.pyx
--rw-r--r--   0        0        0    87239 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/nautilus_pyo3.pyi
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/rust/__init__.pxd
--rw-r--r--   0        0        0     2685 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/rust/algorithms.pxd
--rw-r--r--   0        0        0     1050 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/rust/backtest.pxd
--rw-r--r--   0        0        0    15615 2024-05-18 09:18:20.258708 nautilus_trader-1.192.0/nautilus_trader/core/rust/common.pxd
--rw-r--r--   0        0        0     1222 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/rust/common.pyx
--rw-r--r--   0        0        0     3107 2024-05-18 09:15:47.077413 nautilus_trader-1.192.0/nautilus_trader/core/rust/core.pxd
--rw-r--r--   0        0        0    61890 2024-05-18 09:17:03.386044 nautilus_trader-1.192.0/nautilus_trader/core/rust/model.pxd
--rw-r--r--   0        0        0     2702 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/rust/model.pyx
--rw-r--r--   0        0        0     1359 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/stats.pxd
--rw-r--r--   0        0        0     5710 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/stats.pyx
--rw-r--r--   0        0        0     3870 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/string.pxd
--rw-r--r--   0        0        0     1049 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/uuid.pxd
--rw-r--r--   0        0        0     2755 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/core/uuid.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/__init__.pxd
--rw-r--r--   0        0        0     1360 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/__init__.py
--rw-r--r--   0        0        0     4191 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/aggregation.pxd
--rw-r--r--   0        0        0    24575 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/aggregation.pyx
--rw-r--r--   0        0        0     8072 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/client.pxd
--rw-r--r--   0        0        0    39952 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/client.pyx
--rw-r--r--   0        0        0     2142 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/config.py
--rw-r--r--   0        0        0    10088 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/engine.pxd
--rw-r--r--   0        0        0    65384 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/engine.pyx
--rw-r--r--   0        0        0     2391 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/messages.pxd
--rw-r--r--   0        0        0     8362 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/data/messages.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/algorithms/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/algorithms/blank.py
--rw-r--r--   0        0        0    11242 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/algorithms/twap.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/blank.py
--rw-r--r--   0        0        0    11736 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross.py
--rw-r--r--   0        0        0    11534 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_bracket.py
--rw-r--r--   0        0        0    14158 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py
--rw-r--r--   0        0        0    10284 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx
--rw-r--r--   0        0        0    11178 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_long_only.py
--rw-r--r--   0        0        0    15993 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py
--rw-r--r--   0        0        0    14118 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py
--rw-r--r--   0        0        0    12012 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_twap.py
--rw-r--r--   0        0        0     5286 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/market_maker.py
--rw-r--r--   0        0        0     8954 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/orderbook_imbalance.py
--rw-r--r--   0        0        0     9360 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py
--rw-r--r--   0        0        0     2839 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/signal_strategy.py
--rw-r--r--   0        0        0     4718 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/subscribe.py
--rw-r--r--   0        0        0     7283 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/talib_strategy.py
--rw-r--r--   0        0        0    14071 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/examples/strategies/volatility_market_maker.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/__init__.pxd
--rw-r--r--   0        0        0     1353 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/__init__.py
--rw-r--r--   0        0        0     8527 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/algorithm.pxd
--rw-r--r--   0        0        0    52607 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/algorithm.pyx
--rw-r--r--   0        0        0     7359 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/client.pxd
--rw-r--r--   0        0        0    29170 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/client.pyx
--rw-r--r--   0        0        0     3587 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/config.py
--rw-r--r--   0        0        0     4001 2024-05-18 09:12:24.971797 nautilus_trader-1.192.0/nautilus_trader/execution/emulator.pxd
--rw-r--r--   0        0        0    35586 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/emulator.pyx
--rw-r--r--   0        0        0     6956 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/engine.pxd
--rw-r--r--   0        0        0    46472 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/engine.pyx
--rw-r--r--   0        0        0     4593 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/manager.pxd
--rw-r--r--   0        0        0    24284 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/manager.pyx
--rw-r--r--   0        0        0     3590 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/matching_core.pxd
--rw-r--r--   0        0        0    16178 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/matching_core.pyx
--rw-r--r--   0        0        0     5598 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/messages.pxd
--rw-r--r--   0        0        0    34648 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/messages.pyx
--rw-r--r--   0        0        0    22236 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/reports.py
--rw-r--r--   0        0        0     1726 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/trailing.pxd
--rw-r--r--   0        0        0    17089 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/execution/trailing.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/__init__.pxd
--rw-r--r--   0        0        0     1188 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/__init__.py
--rw-r--r--   0        0        0     1722 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/amat.pxd
--rw-r--r--   0        0        0     4832 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/amat.pyx
--rw-r--r--   0        0        0     1482 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/aroon.pxd
--rw-r--r--   0        0        0     3470 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/aroon.pyx
--rw-r--r--   0        0        0     1474 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/atr.pxd
--rw-r--r--   0        0        0     4320 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/atr.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/ama.pxd
--rw-r--r--   0        0        0     5185 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/ama.pyx
--rw-r--r--   0        0        0     1063 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/dema.pxd
--rw-r--r--   0        0        0     3840 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/dema.pyx
--rw-r--r--   0        0        0     1096 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/ema.pxd
--rw-r--r--   0        0        0     3454 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/ema.pyx
--rw-r--r--   0        0        0     1247 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/hma.pxd
--rw-r--r--   0        0        0     4323 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/hma.pyx
--rw-r--r--   0        0        0     3114 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/ma_factory.pyx
--rw-r--r--   0        0        0     1568 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/moving_average.pxd
--rw-r--r--   0        0        0     2960 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/moving_average.pyx
--rw-r--r--   0        0        0     1080 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/rma.pxd
--rw-r--r--   0        0        0     3466 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/rma.pyx
--rw-r--r--   0        0        0     1020 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/sma.pxd
--rw-r--r--   0        0        0     3530 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/sma.pyx
--rw-r--r--   0        0        0     1283 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/vidya.pxd
--rw-r--r--   0        0        0     4592 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/vidya.pyx
--rw-r--r--   0        0        0     1174 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/wma.pxd
--rw-r--r--   0        0        0     4700 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/average/wma.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/base/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/base/__init__.py
--rw-r--r--   0        0        0     1701 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/base/indicator.pxd
--rw-r--r--   0        0        0     3029 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/base/indicator.pyx
--rw-r--r--   0        0        0     1315 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/bias.pxd
--rw-r--r--   0        0        0     2868 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/bias.pyx
--rw-r--r--   0        0        0     1579 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/bollinger_bands.pxd
--rw-r--r--   0        0        0     5219 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/bollinger_bands.pyx
--rw-r--r--   0        0        0     1635 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/cci.pxd
--rw-r--r--   0        0        0     4056 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/cci.pyx
--rw-r--r--   0        0        0     1375 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/cmo.pxd
--rw-r--r--   0        0        0     3766 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/cmo.pyx
--rw-r--r--   0        0        0     1658 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/dm.pxd
--rw-r--r--   0        0        0     3732 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/dm.pyx
--rw-r--r--   0        0        0     1490 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/donchian_channel.pxd
--rw-r--r--   0        0        0     4374 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/donchian_channel.pyx
--rw-r--r--   0        0        0     1231 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/efficiency_ratio.pxd
--rw-r--r--   0        0        0     3119 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/efficiency_ratio.pyx
--rw-r--r--   0        0        0     3168 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd
--rw-r--r--   0        0        0    12540 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx
--rw-r--r--   0        0        0     1347 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enum.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/__init__.py
--rw-r--r--   0        0        0      976 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd
--rw-r--r--   0        0        0      980 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx
--rw-r--r--   0        0        0      947 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd
--rw-r--r--   0        0        0      987 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx
--rw-r--r--   0        0        0     1020 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd
--rw-r--r--   0        0        0      972 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx
--rw-r--r--   0        0        0      972 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd
--rw-r--r--   0        0        0      980 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx
--rw-r--r--   0        0        0     1805 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_channel.pxd
--rw-r--r--   0        0        0     4675 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_channel.pyx
--rw-r--r--   0        0        0     1395 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_position.pxd
--rw-r--r--   0        0        0     4280 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_position.pyx
--rw-r--r--   0        0        0     1713 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/kvo.pxd
--rw-r--r--   0        0        0     4727 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/kvo.pyx
--rw-r--r--   0        0        0     1636 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/linear_regression.pxd
--rw-r--r--   0        0        0     3839 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/linear_regression.pyx
--rw-r--r--   0        0        0     1664 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/macd.pxd
--rw-r--r--   0        0        0     4809 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/macd.pyx
--rw-r--r--   0        0        0     1232 2024-05-18 09:12:24.975797 nautilus_trader-1.192.0/nautilus_trader/indicators/obv.pxd
--rw-r--r--   0        0        0     2958 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/obv.pyx
--rw-r--r--   0        0        0     1514 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/pressure.pxd
--rw-r--r--   0        0        0     4383 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/pressure.pyx
--rw-r--r--   0        0        0     1476 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/psl.pxd
--rw-r--r--   0        0        0     3311 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/psl.pyx
--rw-r--r--   0        0        0     1227 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/roc.pxd
--rw-r--r--   0        0        0     2726 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/roc.pyx
--rw-r--r--   0        0        0     1393 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/rsi.pxd
--rw-r--r--   0        0        0     3767 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/rsi.pyx
--rw-r--r--   0        0        0     1763 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/rvi.pxd
--rw-r--r--   0        0        0     4539 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/rvi.pyx
--rw-r--r--   0        0        0     1444 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/spread_analyzer.pxd
--rw-r--r--   0        0        0     3391 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/spread_analyzer.pyx
--rw-r--r--   0        0        0     1485 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/stochastics.pxd
--rw-r--r--   0        0        0     3884 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/stochastics.pyx
--rw-r--r--   0        0        0     2271 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/swings.pxd
--rw-r--r--   0        0        0     4678 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/swings.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/ta_lib/__init__.py
--rw-r--r--   0        0        0     1993 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/ta_lib/common.py
--rw-r--r--   0        0        0    29656 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/ta_lib/manager.py
--rw-r--r--   0        0        0     1458 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/vhf.pxd
--rw-r--r--   0        0        0     3513 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/vhf.pyx
--rw-r--r--   0        0        0     1485 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/volatility_ratio.pxd
--rw-r--r--   0        0        0     4482 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/volatility_ratio.pyx
--rw-r--r--   0        0        0     1270 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/vwap.pxd
--rw-r--r--   0        0        0     2938 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/indicators/vwap.pyx
--rw-r--r--   0        0        0     1155 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/__init__.py
--rw-r--r--   0        0        0     1861 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/__main__.py
--rw-r--r--   0        0        0     8314 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/config.py
--rw-r--r--   0        0        0    34312 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/data_client.py
--rw-r--r--   0        0        0    16375 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/data_engine.py
--rw-r--r--   0        0        0    18927 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/execution_client.py
--rw-r--r--   0        0        0    41082 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/execution_engine.py
--rw-r--r--   0        0        0     3395 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/factories.py
--rw-r--r--   0        0        0    16754 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/node.py
--rw-r--r--   0        0        0     9369 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/node_builder.py
--rw-r--r--   0        0        0     9696 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/live/risk_engine.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/__init__.pxd
--rw-r--r--   0        0        0     1652 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/__init__.py
--rw-r--r--   0        0        0     3380 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/book.pxd
--rw-r--r--   0        0        0    24325 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/book.pyx
--rw-r--r--   0        0        0     5067 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/currencies.py
--rw-r--r--   0        0        0    13066 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/data.pxd
--rw-r--r--   0        0        0   126566 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/data.pyx
--rw-r--r--   0        0        0     7811 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/enums.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/__init__.pxd
--rw-r--r--   0        0        0     2829 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/__init__.py
--rw-r--r--   0        0        0     2220 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/account.pxd
--rw-r--r--   0        0        0     6660 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/account.pyx
--rw-r--r--   0        0        0    12302 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/order.pxd
--rw-r--r--   0        0        0   136228 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/order.pyx
--rw-r--r--   0        0        0     5628 2024-05-18 09:12:24.979797 nautilus_trader-1.192.0/nautilus_trader/model/events/position.pxd
--rw-r--r--   0        0        0    35393 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/events/position.pyx
--rw-r--r--   0        0        0     5142 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/functions.pxd
--rw-r--r--   0        0        0    10333 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/functions.pyx
--rw-r--r--   0        0        0     4039 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/identifiers.pxd
--rw-r--r--   0        0        0    27544 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/identifiers.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/__init__.pxd
--rw-r--r--   0        0        0     2302 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/__init__.py
--rw-r--r--   0        0        0     5519 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/base.pxd
--rw-r--r--   0        0        0    21031 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/base.pyx
--rw-r--r--   0        0        0     1778 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/betting.pxd
--rw-r--r--   0        0        0     8622 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/betting.pyx
--rw-r--r--   0        0        0     1449 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/cfd.pxd
--rw-r--r--   0        0        0    13625 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/cfd.pyx
--rw-r--r--   0        0        0     1296 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/commodity.pxd
--rw-r--r--   0        0        0    13011 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/commodity.pyx
--rw-r--r--   0        0        0     1756 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_future.pxd
--rw-r--r--   0        0        0    14480 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_future.pyx
--rw-r--r--   0        0        0     1563 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_perpetual.pxd
--rw-r--r--   0        0        0    13388 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_perpetual.pyx
--rw-r--r--   0        0        0     1334 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/currency_pair.pxd
--rw-r--r--   0        0        0    13495 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/currency_pair.pyx
--rw-r--r--   0        0        0     1284 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/equity.pxd
--rw-r--r--   0        0        0     9201 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/equity.pyx
--rw-r--r--   0        0        0     1736 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_contract.pxd
--rw-r--r--   0        0        0    11356 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_contract.pyx
--rw-r--r--   0        0        0     1824 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_spread.pxd
--rw-r--r--   0        0        0    11963 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_spread.pyx
--rw-r--r--   0        0        0     2068 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_contract.pxd
--rw-r--r--   0        0        0    12508 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_contract.pyx
--rw-r--r--   0        0        0     1930 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_spread.pxd
--rw-r--r--   0        0        0    12096 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_spread.pyx
--rw-r--r--   0        0        0     1555 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/synthetic.pxd
--rw-r--r--   0        0        0    12487 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/instruments/synthetic.pyx
--rw-r--r--   0        0        0     5934 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/objects.pxd
--rw-r--r--   0        0        0    52381 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/objects.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/__init__.pxd
--rw-r--r--   0        0        0     2094 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/__init__.py
--rw-r--r--   0        0        0     9471 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/base.pxd
--rw-r--r--   0        0        0    37731 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/base.pyx
--rw-r--r--   0        0        0     1770 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/limit.pxd
--rw-r--r--   0        0        0    21400 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/limit.pyx
--rw-r--r--   0        0        0     2175 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/limit_if_touched.pxd
--rw-r--r--   0        0        0    17609 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/limit_if_touched.pyx
--rw-r--r--   0        0        0     1842 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/list.pxd
--rw-r--r--   0        0        0     2365 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/list.pyx
--rw-r--r--   0        0        0     1272 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/market.pxd
--rw-r--r--   0        0        0    15939 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/market.pyx
--rw-r--r--   0        0        0     1612 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/market_if_touched.pxd
--rw-r--r--   0        0        0    15818 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/market_if_touched.pyx
--rw-r--r--   0        0        0     1646 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/market_to_limit.pxd
--rw-r--r--   0        0        0    14283 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/market_to_limit.pyx
--rw-r--r--   0        0        0     2232 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_limit.pxd
--rw-r--r--   0        0        0    20646 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_limit.pyx
--rw-r--r--   0        0        0     1602 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_market.pxd
--rw-r--r--   0        0        0    15977 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_market.pyx
--rw-r--r--   0        0        0     2647 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_limit.pxd
--rw-r--r--   0        0        0    19580 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_limit.pyx
--rw-r--r--   0        0        0     1953 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_market.pxd
--rw-r--r--   0        0        0    17208 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_market.pyx
--rw-r--r--   0        0        0     1141 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/unpacker.pxd
--rw-r--r--   0        0        0     3926 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/orders/unpacker.pyx
--rw-r--r--   0        0        0     6940 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/position.pxd
--rw-r--r--   0        0        0    23901 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/position.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/__init__.pxd
--rw-r--r--   0        0        0     1443 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/__init__.py
--rw-r--r--   0        0        0     1581 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/base.pxd
--rw-r--r--   0        0        0     3709 2024-05-18 09:12:24.983797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/base.pyx
--rw-r--r--   0        0        0     1147 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd
--rw-r--r--   0        0        0     3921 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx
--rw-r--r--   0        0        0     1388 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd
--rw-r--r--   0        0        0     5436 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx
--rw-r--r--   0        0        0     1333 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/model/venues.py
--rw-r--r--   0        0        0      973 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/__init__.py
--rw-r--r--   0        0        0     1079 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/__init__.py
--rw-r--r--   0        0        0     6321 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/base.py
--rw-r--r--   0        0        0    28127 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/parquet.py
--rw-r--r--   0        0        0     2073 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/singleton.py
--rw-r--r--   0        0        0     1327 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/types.py
--rw-r--r--   0        0        0     2886 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/config.py
--rw-r--r--   0        0        0     3561 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/funcs.py
--rw-r--r--   0        0        0     7025 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/loaders.py
--rw-r--r--   0        0        0     3392 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/wranglers.pxd
--rw-r--r--   0        0        0    30305 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/wranglers.pyx
--rw-r--r--   0        0        0    16480 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/wranglers_v2.py
--rw-r--r--   0        0        0    12974 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/persistence/writer.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/portfolio/__init__.pxd
--rw-r--r--   0        0        0     1123 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     2132 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/portfolio/base.pxd
--rw-r--r--   0        0        0     4233 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/portfolio/base.pyx
--rw-r--r--   0        0        0     3111 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/portfolio/portfolio.pxd
--rw-r--r--   0        0        0    38292 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/portfolio/portfolio.pyx
--rw-r--r--   0        0        0        0 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/py.typed
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/__init__.pxd
--rw-r--r--   0        0        0     1084 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/__init__.py
--rw-r--r--   0        0        0     1974 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/config.py
--rw-r--r--   0        0        0     5474 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/engine.pxd
--rw-r--r--   0        0        0    38261 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/engine.pyx
--rw-r--r--   0        0        0     1747 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/sizing.pxd
--rw-r--r--   0        0        0     7059 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/risk/sizing.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/__init__.pxd
--rw-r--r--   0        0        0     1106 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/__init__.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/__init__.py
--rw-r--r--   0        0        0     5360 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/account_state.py
--rw-r--r--   0        0        0     1689 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/component_events.py
--rw-r--r--   0        0        0    14111 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/instruments.py
--rw-r--r--   0        0        0     2191 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/order_events.py
--rw-r--r--   0        0        0     5923 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/position_events.py
--rw-r--r--   0        0        0    15753 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/schema.py
--rw-r--r--   0        0        0    13886 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/serializer.py
--rw-r--r--   0        0        0     1096 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/base.pxd
--rw-r--r--   0        0        0    12000 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/base.pyx
--rw-r--r--   0        0        0     1303 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/serializer.pxd
--rw-r--r--   0        0        0     5404 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/serialization/serializer.pyx
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/system/__init__.py
--rw-r--r--   0        0        0     6506 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/system/config.py
--rw-r--r--   0        0        0    40208 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/system/kernel.py
--rw-r--r--   0        0        0     1034 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/functions.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/__init__.py
--rw-r--r--   0        0        0     6382 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/actors.py
--rw-r--r--   0        0        0     5793 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/cache_database.py
--rw-r--r--   0        0        0     1550 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/controller.py
--rw-r--r--   0        0        0     3177 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/data.py
--rw-r--r--   0        0        0     2976 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/engines.py
--rw-r--r--   0        0        0    12678 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/exec_clients.py
--rw-r--r--   0        0        0     7299 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/strategies.py
--rw-r--r--   0        0        0    29811 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/providers.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/__init__.py
--rw-r--r--   0        0        0     3697 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/accounting_pyo3.py
--rw-r--r--   0        0        0     6642 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/data_pyo3.py
--rw-r--r--   0        0        0    19951 2024-05-18 09:12:24.987797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/events_pyo3.py
--rw-r--r--   0        0        0     3912 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py
--rw-r--r--   0        0        0    15113 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/instruments_pyo3.py
--rw-r--r--   0        0        0     5508 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/orders_pyo3.py
--rw-r--r--   0        0        0     2451 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/types_pyo3.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/__init__.py
--rw-r--r--   0        0        0     4828 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/commands.py
--rw-r--r--   0        0        0     5842 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/component.py
--rw-r--r--   0        0        0     6234 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/config.py
--rw-r--r--   0        0        0    22352 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/data.py
--rw-r--r--   0        0        0    14777 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/events.py
--rw-r--r--   0        0        0     9471 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/execution.py
--rw-r--r--   0        0        0     3991 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/identifiers.py
--rw-r--r--   0        0        0     3415 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/persistence.py
--rw-r--r--   0        0        0      869 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/__init__.pxd
--rw-r--r--   0        0        0     1372 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/__init__.py
--rw-r--r--   0        0        0     4730 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/config.py
--rw-r--r--   0        0        0     5493 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/controller.py
--rw-r--r--   0        0        0    18226 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/filters.py
--rw-r--r--   0        0        0     8699 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/strategy.pxd
--rw-r--r--   0        0        0    59399 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/strategy.pyx
--rw-r--r--   0        0        0    25167 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/nautilus_trader/trading/trader.py
--rw-r--r--   0        0        0     8001 2024-05-18 09:12:24.991797 nautilus_trader-1.192.0/pyproject.toml
--rw-r--r--   0        0        0    27308 1970-01-01 00:00:00.000000 nautilus_trader-1.192.0/PKG-INFO
+-rw-r--r--   0        0        0     7651 2024-05-24 12:14:01.313010 nautilus_trader-1.193.0/LICENSE
+-rw-r--r--   0        0        0    25213 2024-05-24 12:14:01.313010 nautilus_trader-1.193.0/README.md
+-rw-r--r--   0        0        0    12823 2024-05-24 12:14:01.313010 nautilus_trader-1.193.0/build.py
+-rw-r--r--   0        0        0      663 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/.cargo/config.toml
+-rw-r--r--   0        0        0   135456 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/Cargo.lock
+-rw-r--r--   0        0        0     2305 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/Cargo.toml
+-rw-r--r--   0        0        0     7652 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/LICENSE
+-rw-r--r--   0        0        0     1248 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/README.md
+-rw-r--r--   0        0        0      967 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/Cargo.toml
+-rw-r--r--   0        0        0     9225 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/base.rs
+-rw-r--r--   0        0        0    20368 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/cash.rs
+-rw-r--r--   0        0        0    22074 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/margin.rs
+-rw-r--r--   0        0        0     1015 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/mod.rs
+-rw-r--r--   0        0        0     2376 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/stubs.rs
+-rw-r--r--   0        0        0     1673 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/lib.rs
+-rw-r--r--   0        0        0     6160 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/cash.rs
+-rw-r--r--   0        0        0     8441 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/margin.rs
+-rw-r--r--   0        0        0     1557 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/mod.rs
+-rw-r--r--   0        0        0     2609 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/transformer.rs
+-rw-r--r--   0        0        0     2598 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/stubs.rs
+-rw-r--r--   0        0        0     1669 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/Cargo.toml
+-rw-r--r--   0        0        0     1217 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/bin/sandbox.rs
+-rw-r--r--   0        0        0     2250 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/common.rs
+-rw-r--r--   0        0        0    44341 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/decode.rs
+-rw-r--r--   0        0        0     3482 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/enums.rs
+-rw-r--r--   0        0        0    15981 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/live.rs
+-rw-r--r--   0        0        0    11923 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/loader.rs
+-rw-r--r--   0        0        0     1113 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/mod.rs
+-rw-r--r--   0        0        0    10104 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/publishers.json
+-rw-r--r--   0        0        0     5323 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/enums.rs
+-rw-r--r--   0        0        0    19510 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/historical.rs
+-rw-r--r--   0        0        0     8154 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/live.rs
+-rw-r--r--   0        0        0    13415 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/loader.rs
+-rw-r--r--   0        0        0     1702 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/mod.rs
+-rw-r--r--   0        0        0     7715 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/types.rs
+-rw-r--r--   0        0        0     6477 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/symbology.rs
+-rw-r--r--   0        0        0       81 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.cbbo.dbn.zst
+-rw-r--r--   0        0        0      693 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst
+-rw-r--r--   0        0        0      673 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst
+-rw-r--r--   0        0        0      661 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst
+-rw-r--r--   0        0        0      465 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn
+-rw-r--r--   0        0        0      174 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn.zst
+-rw-r--r--   0        0        0      192 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-1.dbn.zst
+-rw-r--r--   0        0        0      374 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-10.dbn.zst
+-rw-r--r--   0        0        0      103 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1d.dbn.zst
+-rw-r--r--   0        0        0      186 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1h.dbn.zst
+-rw-r--r--   0        0        0      165 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1m.dbn.zst
+-rw-r--r--   0        0        0      157 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1s.dbn.zst
+-rw-r--r--   0        0        0      139 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.statistics.dbn.zst
+-rw-r--r--   0        0        0      197 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.tbbo.dbn.zst
+-rw-r--r--   0        0        0      173 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.trades.dbn.zst
+-rw-r--r--   0        0        0     6857 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/types.rs
+-rw-r--r--   0        0        0     1771 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/lib.rs
+-rw-r--r--   0        0        0     1234 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/Cargo.toml
+-rw-r--r--   0        0        0     2046 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/build.rs
+-rw-r--r--   0        0        0      484 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/cbindgen.toml
+-rw-r--r--   0        0        0      807 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/cbindgen_cython.toml
+-rw-r--r--   0        0        0     6213 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/src/engine.rs
+-rw-r--r--   0        0        0     1701 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/src/lib.rs
+-rw-r--r--   0        0        0     8782 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/src/matching_engine.rs
+-rw-r--r--   0        0        0      669 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/Cargo.toml
+-rw-r--r--   0        0        0     1289 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/bin/cli.rs
+-rw-r--r--   0        0        0      902 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/database/mod.rs
+-rw-r--r--   0        0        0     2258 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/database/postgres.rs
+-rw-r--r--   0        0        0     1198 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/lib.rs
+-rw-r--r--   0        0        0     2230 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/opt.rs
+-rw-r--r--   0        0        0       65 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/clippy.toml
+-rw-r--r--   0        0        0     1611 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/Cargo.toml
+-rw-r--r--   0        0        0     2759 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/build.rs
+-rw-r--r--   0        0        0      548 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/cbindgen.toml
+-rw-r--r--   0        0        0      823 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/cbindgen_cython.toml
+-rw-r--r--   0        0        0    96074 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/cache/core.rs
+-rw-r--r--   0        0        0     8710 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/cache/database.rs
+-rw-r--r--   0        0        0     1086 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/cache/mod.rs
+-rw-r--r--   0        0        0    11713 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/clock.rs
+-rw-r--r--   0        0        0     9339 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/enums.rs
+-rw-r--r--   0        0        0     8014 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/factories.rs
+-rw-r--r--   0        0        0    12261 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/clock.rs
+-rw-r--r--   0        0        0     3086 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/enums.rs
+-rw-r--r--   0        0        0     5911 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/logging.rs
+-rw-r--r--   0        0        0     1014 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/mod.rs
+-rw-r--r--   0        0        0     1771 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/timer.rs
+-rw-r--r--   0        0        0     5028 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/client_order_id.rs
+-rw-r--r--   0        0        0     1380 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/mod.rs
+-rw-r--r--   0        0        0     4982 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/order_list_id.rs
+-rw-r--r--   0        0        0     5582 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/position_id.rs
+-rw-r--r--   0        0        0     3412 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/handlers.rs
+-rw-r--r--   0        0        0     2956 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/interface/account.rs
+-rw-r--r--   0        0        0      977 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/interface/mod.rs
+-rw-r--r--   0        0        0     2065 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/lib.rs
+-rw-r--r--   0        0        0     7640 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/headers.rs
+-rw-r--r--   0        0        0    23893 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/logger.rs
+-rw-r--r--   0        0        0     5414 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/mod.rs
+-rw-r--r--   0        0        0     7744 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/writer.rs
+-rw-r--r--   0        0        0    20886 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/core.rs
+-rw-r--r--   0        0        0     1664 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/database.rs
+-rw-r--r--   0        0        0     1046 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/mod.rs
+-rw-r--r--   0        0        0     5841 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/clock.rs
+-rw-r--r--   0        0        0     4513 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/enums.rs
+-rw-r--r--   0        0        0     4896 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/logging.rs
+-rw-r--r--   0        0        0     1999 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/mod.rs
+-rw-r--r--   0        0        0     3479 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/timer.rs
+-rw-r--r--   0        0        0     2848 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/versioning.rs
+-rw-r--r--   0        0        0     1717 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/runtime.rs
+-rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/stubs.rs
+-rw-r--r--   0        0        0     2496 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/testing.rs
+-rw-r--r--   0        0        0    17675 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/timer.rs
+-rw-r--r--   0        0        0     5943 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/xrate.rs
+-rw-r--r--   0        0        0      850 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/Cargo.toml
+-rw-r--r--   0        0        0     2755 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/build.rs
+-rw-r--r--   0        0        0      717 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/cbindgen.toml
+-rw-r--r--   0        0        0      824 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/cbindgen_cython.toml
+-rw-r--r--   0        0        0    18382 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/correctness.rs
+-rw-r--r--   0        0        0     9172 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/datetime.rs
+-rw-r--r--   0        0        0     2799 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/deserialization.rs
+-rw-r--r--   0        0        0     1156 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/equality.rs
+-rw-r--r--   0        0        0     5695 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/cvec.rs
+-rw-r--r--   0        0        0     1248 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/datetime.rs
+-rw-r--r--   0        0        0     1031 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/mod.rs
+-rw-r--r--   0        0        0     8229 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/parsing.rs
+-rw-r--r--   0        0        0     6642 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/string.rs
+-rw-r--r--   0        0        0     3986 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/uuid.rs
+-rw-r--r--   0        0        0     1924 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/lib.rs
+-rw-r--r--   0        0        0     1409 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/message.rs
+-rw-r--r--   0        0        0     8197 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/nanos.rs
+-rw-r--r--   0        0        0     3425 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/parsing.rs
+-rw-r--r--   0        0        0     1067 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/casing.rs
+-rw-r--r--   0        0        0     2691 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/datetime.rs
+-rw-r--r--   0        0        0     2894 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/mod.rs
+-rw-r--r--   0        0        0     1407 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/serialization.rs
+-rw-r--r--   0        0        0     3120 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/uuid.rs
+-rw-r--r--   0        0        0     1814 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/serialization.rs
+-rw-r--r--   0        0        0     8831 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/time.rs
+-rw-r--r--   0        0        0     6040 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/uuid.rs
+-rw-r--r--   0        0        0     1371 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/Cargo.toml
+-rw-r--r--   0        0        0     6813 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/client.rs
+-rw-r--r--   0        0        0     8306 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/engine.rs
+-rw-r--r--   0        0        0     1733 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/lib.rs
+-rw-r--r--   0        0        0    18827 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/matching_core.rs
+-rw-r--r--   0        0        0     2761 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel.rs
+-rw-r--r--   0        0        0     2581 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_all.rs
+-rw-r--r--   0        0        0     2561 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_batch.rs
+-rw-r--r--   0        0        0     2809 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/mod.rs
+-rw-r--r--   0        0        0     3416 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/modify.rs
+-rw-r--r--   0        0        0     2757 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/query.rs
+-rw-r--r--   0        0        0     3171 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit.rs
+-rw-r--r--   0        0        0     3214 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit_list.rs
+-rw-r--r--   0        0        0      746 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/Cargo.toml
+-rw-r--r--   0        0        0     8897 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ama.rs
+-rw-r--r--   0        0        0     6979 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/dema.rs
+-rw-r--r--   0        0        0     6902 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ema.rs
+-rw-r--r--   0        0        0     8322 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/hma.rs
+-rw-r--r--   0        0        0     2875 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/mod.rs
+-rw-r--r--   0        0        0     6925 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/rma.rs
+-rw-r--r--   0        0        0     6142 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/sma.rs
+-rw-r--r--   0        0        0     7476 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/vidya.rs
+-rw-r--r--   0        0        0     7727 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/wma.rs
+-rw-r--r--   0        0        0     6332 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/book/imbalance.rs
+-rw-r--r--   0        0        0      940 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/book/mod.rs
+-rw-r--r--   0        0        0     3206 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/indicator.rs
+-rw-r--r--   0        0        0     1773 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/lib.rs
+-rw-r--r--   0        0        0     7660 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/aroon.rs
+-rw-r--r--   0        0        0     5019 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/bias.rs
+-rw-r--r--   0        0        0     7008 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/cmo.rs
+-rw-r--r--   0        0        0      970 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/mod.rs
+-rw-r--r--   0        0        0     7876 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/rsi.rs
+-rw-r--r--   0        0        0     2922 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ama.rs
+-rw-r--r--   0        0        0     2799 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/dema.rs
+-rw-r--r--   0        0        0     2880 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ema.rs
+-rw-r--r--   0        0        0     2759 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/hma.rs
+-rw-r--r--   0        0        0      976 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/mod.rs
+-rw-r--r--   0        0        0     2865 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/rma.rs
+-rw-r--r--   0        0        0     2765 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/sma.rs
+-rw-r--r--   0        0        0     3101 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/vidya.rs
+-rw-r--r--   0        0        0     2755 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/wma.rs
+-rw-r--r--   0        0        0     2221 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/imbalance.rs
+-rw-r--r--   0        0        0      903 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/mod.rs
+-rw-r--r--   0        0        0     2217 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/mod.rs
+-rw-r--r--   0        0        0     2901 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/aroon.rs
+-rw-r--r--   0        0        0     2682 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/bias.rs
+-rw-r--r--   0        0        0     2748 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/cmo.rs
+-rw-r--r--   0        0        0      939 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/mod.rs
+-rw-r--r--   0        0        0     2583 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/rsi.rs
+-rw-r--r--   0        0        0     2005 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs
+-rw-r--r--   0        0        0      910 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/mod.rs
+-rw-r--r--   0        0        0     3005 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/atr.rs
+-rw-r--r--   0        0        0      897 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/mod.rs
+-rw-r--r--   0        0        0     8102 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs
+-rw-r--r--   0        0        0      938 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/mod.rs
+-rw-r--r--   0        0        0     5818 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/stubs.rs
+-rw-r--r--   0        0        0     1509 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/testing.rs
+-rw-r--r--   0        0        0     9258 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/atr.rs
+-rw-r--r--   0        0        0      930 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/mod.rs
+-rw-r--r--   0        0        0     1527 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/Cargo.toml
+-rw-r--r--   0        0        0     1855 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/lib.rs
+-rw-r--r--   0        0        0     1430 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/mod.rs
+-rw-r--r--   0        0        0     3422 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/cache.rs
+-rw-r--r--   0        0        0     1065 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/mod.rs
+-rw-r--r--   0        0        0     1960 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs
+-rw-r--r--   0        0        0     6622 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs
+-rw-r--r--   0        0        0      908 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/mod.rs
+-rw-r--r--   0        0        0    21364 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/cache.rs
+-rw-r--r--   0        0        0    10578 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/mod.rs
+-rw-r--r--   0        0        0     7063 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/msgbus.rs
+-rw-r--r--   0        0        0    11599 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/cache_database.rs
+-rw-r--r--   0        0        0     1137 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/mod.rs
+-rw-r--r--   0        0        0      987 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/general.rs
+-rw-r--r--   0        0        0    26965 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/instruments.rs
+-rw-r--r--   0        0        0      953 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/mod.rs
+-rw-r--r--   0        0        0    19284 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/orders.rs
+-rw-r--r--   0        0        0     1805 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/types.rs
+-rw-r--r--   0        0        0    10685 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/pg.rs
+-rw-r--r--   0        0        0    18517 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/queries.rs
+-rw-r--r--   0        0        0    13104 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs
+-rw-r--r--   0        0        0     1430 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/Cargo.toml
+-rw-r--r--   0        0        0      400 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/benches/criterion_fixed_precision_benchmark.rs
+-rw-r--r--   0        0        0      225 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/benches/iai_fixed_precision_benchmark.rs
+-rw-r--r--   0        0        0     2757 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/build.rs
+-rw-r--r--   0        0        0     1617 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/cbindgen.toml
+-rw-r--r--   0        0        0     1839 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/cbindgen_cython.toml
+-rw-r--r--   0        0        0    33910 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/currencies.rs
+-rw-r--r--   0        0        0    16919 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/bar.rs
+-rw-r--r--   0        0        0     8316 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/delta.rs
+-rw-r--r--   0        0        0     8465 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/deltas.rs
+-rw-r--r--   0        0        0    11159 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/depth.rs
+-rw-r--r--   0        0        0     3040 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/mod.rs
+-rw-r--r--   0        0        0     6445 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/order.rs
+-rw-r--r--   0        0        0     8044 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/quote.rs
+-rw-r--r--   0        0        0     9402 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/stubs.rs
+-rw-r--r--   0        0        0     6693 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/trade.rs
+-rw-r--r--   0        0        0    30931 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/enums.rs
+-rw-r--r--   0        0        0      940 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/account/mod.rs
+-rw-r--r--   0        0        0     4946 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/account/state.rs
+-rw-r--r--   0        0        0     4078 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/account/stubs.rs
+-rw-r--r--   0        0        0     1012 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/mod.rs
+-rw-r--r--   0        0        0     7811 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/accepted.rs
+-rw-r--r--   0        0        0     8419 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/cancel_rejected.rs
+-rw-r--r--   0        0        0     7695 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/canceled.rs
+-rw-r--r--   0        0        0     7190 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/denied.rs
+-rw-r--r--   0        0        0     7034 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/emulated.rs
+-rw-r--r--   0        0        0     5516 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/event.rs
+-rw-r--r--   0        0        0     8131 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/expired.rs
+-rw-r--r--   0        0        0    11711 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/filled.rs
+-rw-r--r--   0        0        0    18687 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/initialized.rs
+-rw-r--r--   0        0        0     3888 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/mod.rs
+-rw-r--r--   0        0        0     8402 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/modify_rejected.rs
+-rw-r--r--   0        0        0     8063 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_cancel.rs
+-rw-r--r--   0        0        0     8081 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_update.rs
+-rw-r--r--   0        0        0     7761 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/rejected.rs
+-rw-r--r--   0        0        0     7291 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/released.rs
+-rw-r--r--   0        0        0    11494 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/stubs.rs
+-rw-r--r--   0        0        0     7334 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/submitted.rs
+-rw-r--r--   0        0        0     8180 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/triggered.rs
+-rw-r--r--   0        0        0     9016 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/updated.rs
+-rw-r--r--   0        0        0     1987 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/changed.rs
+-rw-r--r--   0        0        0     2106 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/closed.rs
+-rw-r--r--   0        0        0     1200 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/mod.rs
+-rw-r--r--   0        0        0     1791 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/opened.rs
+-rw-r--r--   0        0        0     1985 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/state.rs
+-rw-r--r--   0        0        0     6050 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/bar.rs
+-rw-r--r--   0        0        0     1845 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/delta.rs
+-rw-r--r--   0        0        0     3549 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/deltas.rs
+-rw-r--r--   0        0        0     3787 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/depth.rs
+-rw-r--r--   0        0        0      988 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/mod.rs
+-rw-r--r--   0        0        0     2417 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/order.rs
+-rw-r--r--   0        0        0     2745 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/quote.rs
+-rw-r--r--   0        0        0     2203 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/trade.rs
+-rw-r--r--   0        0        0    15015 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/enums.rs
+-rw-r--r--   0        0        0      899 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/mod.rs
+-rw-r--r--   0        0        0     4681 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/order.rs
+-rw-r--r--   0        0        0     3279 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/account_id.rs
+-rw-r--r--   0        0        0     2234 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_id.rs
+-rw-r--r--   0        0        0     1398 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs
+-rw-r--r--   0        0        0     1381 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/component_id.rs
+-rw-r--r--   0        0        0     1412 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs
+-rw-r--r--   0        0        0     4223 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1177 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/mod.rs
+-rw-r--r--   0        0        0     1384 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs
+-rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/position_id.rs
+-rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs
+-rw-r--r--   0        0        0     1343 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/symbol.rs
+-rw-r--r--   0        0        0     1603 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     1360 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs
+-rw-r--r--   0        0        0     2003 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue.rs
+-rw-r--r--   0        0        0     1391 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs
+-rw-r--r--   0        0        0      903 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/mod.rs
+-rw-r--r--   0        0        0     5668 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/synthetic.rs
+-rw-r--r--   0        0        0     1073 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/mod.rs
+-rw-r--r--   0        0        0     8567 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/book.rs
+-rw-r--r--   0        0        0     3621 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/level.rs
+-rw-r--r--   0        0        0      913 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/mod.rs
+-rw-r--r--   0        0        0     5719 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/currency.rs
+-rw-r--r--   0        0        0      950 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/mod.rs
+-rw-r--r--   0        0        0     1596 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/money.rs
+-rw-r--r--   0        0        0     1589 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/price.rs
+-rw-r--r--   0        0        0     1845 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/quantity.rs
+-rw-r--r--   0        0        0     4561 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/account_id.rs
+-rw-r--r--   0        0        0     2846 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_id.rs
+-rw-r--r--   0        0        0     4794 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_order_id.rs
+-rw-r--r--   0        0        0     2897 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/component_id.rs
+-rw-r--r--   0        0        0     2899 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs
+-rw-r--r--   0        0        0     4866 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1909 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/macros.rs
+-rw-r--r--   0        0        0     3032 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/mod.rs
+-rw-r--r--   0        0        0     2899 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/order_list_id.rs
+-rw-r--r--   0        0        0     2874 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/position_id.rs
+-rw-r--r--   0        0        0     4369 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/strategy_id.rs
+-rw-r--r--   0        0        0     4518 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/stubs.rs
+-rw-r--r--   0        0        0     3053 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/symbol.rs
+-rw-r--r--   0        0        0     4233 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     3598 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trader_id.rs
+-rw-r--r--   0        0        0     3604 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue.rs
+-rw-r--r--   0        0        0     2905 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue_order_id.rs
+-rw-r--r--   0        0        0    11059 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/any.rs
+-rw-r--r--   0        0        0     7700 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_future.rs
+-rw-r--r--   0        0        0     7750 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_perpetual.rs
+-rw-r--r--   0        0        0     7499 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/currency_pair.rs
+-rw-r--r--   0        0        0     6626 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/equity.rs
+-rw-r--r--   0        0        0     7324 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_contract.rs
+-rw-r--r--   0        0        0     7448 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_spread.rs
+-rw-r--r--   0        0        0     5480 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/mod.rs
+-rw-r--r--   0        0        0     7574 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_contract.rs
+-rw-r--r--   0        0        0     7439 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_spread.rs
+-rw-r--r--   0        0        0    13302 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/stubs.rs
+-rw-r--r--   0        0        0     6493 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/synthetic.rs
+-rw-r--r--   0        0        0     2074 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/lib.rs
+-rw-r--r--   0        0        0     1595 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/macros.rs
+-rw-r--r--   0        0        0     3536 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/aggregation.rs
+-rw-r--r--   0        0        0     4309 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/analysis.rs
+-rw-r--r--   0        0        0    23019 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/book.rs
+-rw-r--r--   0        0        0     2836 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/display.rs
+-rw-r--r--   0        0        0     1988 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/error.rs
+-rw-r--r--   0        0        0    22495 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/ladder.rs
+-rw-r--r--   0        0        0    13057 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/level.rs
+-rw-r--r--   0        0        0     1067 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/mod.rs
+-rw-r--r--   0        0        0    24817 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/any.rs
+-rw-r--r--   0        0        0    31687 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/base.rs
+-rw-r--r--   0        0        0     9307 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/default.rs
+-rw-r--r--   0        0        0    14285 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit.rs
+-rw-r--r--   0        0        0    11226 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit_if_touched.rs
+-rw-r--r--   0        0        0     4555 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/list.rs
+-rw-r--r--   0        0        0    11942 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/market.rs
+-rw-r--r--   0        0        0    10843 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_if_touched.rs
+-rw-r--r--   0        0        0    10035 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_to_limit.rs
+-rw-r--r--   0        0        0     1270 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/mod.rs
+-rw-r--r--   0        0        0    12288 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_limit.rs
+-rw-r--r--   0        0        0    10817 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_market.rs
+-rw-r--r--   0        0        0     8366 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/stubs.rs
+-rw-r--r--   0        0        0    11871 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_limit.rs
+-rw-r--r--   0        0        0    11317 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_market.rs
+-rw-r--r--   0        0        0     3061 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/polymorphism.rs
+-rw-r--r--   0        0        0    72892 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/position.rs
+-rw-r--r--   0        0        0     7166 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/common.rs
+-rw-r--r--   0        0        0    12321 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/bar.rs
+-rw-r--r--   0        0        0    10587 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/delta.rs
+-rw-r--r--   0        0        0     4435 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/deltas.rs
+-rw-r--r--   0        0        0     8920 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/depth.rs
+-rw-r--r--   0        0        0     3425 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/mod.rs
+-rw-r--r--   0        0        0     5608 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/order.rs
+-rw-r--r--   0        0        0    14445 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/quote.rs
+-rw-r--r--   0        0        0    12629 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/trade.rs
+-rw-r--r--   0        0        0    44501 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/enums.rs
+-rw-r--r--   0        0        0      899 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/mod.rs
+-rw-r--r--   0        0        0     6244 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/state.rs
+-rw-r--r--   0        0        0      966 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/mod.rs
+-rw-r--r--   0        0        0     3547 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/accepted.rs
+-rw-r--r--   0        0        0     4036 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs
+-rw-r--r--   0        0        0     3819 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/canceled.rs
+-rw-r--r--   0        0        0     3297 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/denied.rs
+-rw-r--r--   0        0        0     3110 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/emulated.rs
+-rw-r--r--   0        0        0     3815 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/expired.rs
+-rw-r--r--   0        0        0     7663 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/filled.rs
+-rw-r--r--   0        0        0    11003 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/initialized.rs
+-rw-r--r--   0        0        0     5587 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/mod.rs
+-rw-r--r--   0        0        0     4047 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/modify_rejected.rs
+-rw-r--r--   0        0        0     3710 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_cancel.rs
+-rw-r--r--   0        0        0     3710 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_update.rs
+-rw-r--r--   0        0        0     3570 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/rejected.rs
+-rw-r--r--   0        0        0     3269 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/released.rs
+-rw-r--r--   0        0        0     3259 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/submitted.rs
+-rw-r--r--   0        0        0     3817 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/triggered.rs
+-rw-r--r--   0        0        0     4457 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/updated.rs
+-rw-r--r--   0        0        0     3628 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1993 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/mod.rs
+-rw-r--r--   0        0        0     3411 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     9563 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_future.rs
+-rw-r--r--   0        0        0     9055 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs
+-rw-r--r--   0        0        0     8593 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/currency_pair.rs
+-rw-r--r--   0        0        0     7022 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/equity.rs
+-rw-r--r--   0        0        0     8544 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_contract.rs
+-rw-r--r--   0        0        0     8806 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_spread.rs
+-rw-r--r--   0        0        0     3614 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/mod.rs
+-rw-r--r--   0        0        0     9059 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_contract.rs
+-rw-r--r--   0        0        0     8804 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_spread.rs
+-rw-r--r--   0        0        0     3531 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/macros.rs
+-rw-r--r--   0        0        0     7351 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/mod.rs
+-rw-r--r--   0        0        0     6786 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/book.rs
+-rw-r--r--   0        0        0     2104 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/level.rs
+-rw-r--r--   0        0        0      983 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/mod.rs
+-rw-r--r--   0        0        0    22070 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit.rs
+-rw-r--r--   0        0        0     4518 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit_if_touched.rs
+-rw-r--r--   0        0        0    18609 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market.rs
+-rw-r--r--   0        0        0     4433 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_if_touched.rs
+-rw-r--r--   0        0        0     4159 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_to_limit.rs
+-rw-r--r--   0        0        0     4422 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/mod.rs
+-rw-r--r--   0        0        0    22168 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_limit.rs
+-rw-r--r--   0        0        0     4412 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_market.rs
+-rw-r--r--   0        0        0     4750 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs
+-rw-r--r--   0        0        0     4610 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs
+-rw-r--r--   0        0        0    12642 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/position.rs
+-rw-r--r--   0        0        0     6219 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/balance.rs
+-rw-r--r--   0        0        0     5123 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/currency.rs
+-rw-r--r--   0        0        0     1062 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/mod.rs
+-rw-r--r--   0        0        0    14239 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/money.rs
+-rw-r--r--   0        0        0    14708 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/price.rs
+-rw-r--r--   0        0        0    14615 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/quantity.rs
+-rw-r--r--   0        0        0     5470 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/stubs.rs
+-rw-r--r--   0        0        0     5786 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/types/balance.rs
+-rw-r--r--   0        0        0     7530 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/types/currency.rs
+-rw-r--r--   0        0        0     6622 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/types/fixed.rs
+-rw-r--r--   0        0        0     1118 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/mod.rs
+-rw-r--r--   0        0        0    11756 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/money.rs
+-rw-r--r--   0        0        0    14431 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/price.rs
+-rw-r--r--   0        0        0    14504 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/quantity.rs
+-rw-r--r--   0        0        0     1475 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/stubs.rs
+-rw-r--r--   0        0        0     3064 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/venues.rs
+-rw-r--r--   0        0        0     1036 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/Cargo.toml
+-rw-r--r--   0        0        0     1655 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/benches/test_client.rs
+-rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/benches/test_server.rs
+-rw-r--r--   0        0        0    12459 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/http.rs
+-rw-r--r--   0        0        0     1802 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/lib.rs
+-rw-r--r--   0        0        0     1475 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/python/mod.rs
+-rw-r--r--   0        0        0     6239 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/clock.rs
+-rw-r--r--   0        0        0     5417 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/gcra.rs
+-rw-r--r--   0        0        0     8865 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/mod.rs
+-rw-r--r--   0        0        0     4079 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/nanos.rs
+-rw-r--r--   0        0        0     9739 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/quota.rs
+-rw-r--r--   0        0        0    23594 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/socket.rs
+-rw-r--r--   0        0        0    28915 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/websocket.rs
+-rw-r--r--   0        0        0       18 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/.gitignore
+-rw-r--r--   0        0        0     2862 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md
+-rw-r--r--   0        0        0     2061 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/Cargo.toml
+-rw-r--r--   0        0        0     1093 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/LICENSE
+-rw-r--r--   0        0        0     2861 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/README.md
+-rw-r--r--   0        0        0      268 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/rustfmt.toml
+-rw-r--r--   0        0        0     6900 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/compat.rs
+-rw-r--r--   0        0        0     2747 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/connect.rs
+-rw-r--r--   0        0        0     5469 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs
+-rw-r--r--   0        0        0    14303 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/lib.rs
+-rw-r--r--   0        0        0     2854 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/stream.rs
+-rw-r--r--   0        0        0     8647 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/tls.rs
+-rw-r--r--   0        0        0     1300 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/Cargo.toml
+-rw-r--r--   0        0        0     3658 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/benches/bench_persistence.rs
+-rw-r--r--   0        0        0    12962 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/bar.rs
+-rw-r--r--   0        0        0    15825 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/delta.rs
+-rw-r--r--   0        0        0    41488 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/depth.rs
+-rw-r--r--   0        0        0     4662 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/mod.rs
+-rw-r--r--   0        0        0    12628 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/quote.rs
+-rw-r--r--   0        0        0    12946 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/trade.rs
+-rw-r--r--   0        0        0    10343 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/kmerge_batch.rs
+-rw-r--r--   0        0        0     1025 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/mod.rs
+-rw-r--r--   0        0        0     8065 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/session.rs
+-rw-r--r--   0        0        0     1736 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/lib.rs
+-rw-r--r--   0        0        0      922 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/mod.rs
+-rw-r--r--   0        0        0     4265 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/session.rs
+-rw-r--r--   0        0        0    12804 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/transformer.rs
+-rw-r--r--   0        0        0     1696 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/mod.rs
+-rw-r--r--   0        0        0     2824 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/bar.rs
+-rw-r--r--   0        0        0     3031 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/delta.rs
+-rw-r--r--   0        0        0      942 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/mod.rs
+-rw-r--r--   0        0        0     2955 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/quote.rs
+-rw-r--r--   0        0        0     2952 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/trade.rs
+-rw-r--r--   0        0        0    10633 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_catalog.rs
+-rw-r--r--   0        0        0     2159 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_util.rs
+-rw-r--r--   0        0        0     1469 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/pyo3/Cargo.toml
+-rw-r--r--   0        0        0     4929 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/pyo3/src/lib.rs
+-rw-r--r--   0        0        0       50 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/rust-toolchain.toml
+-rw-r--r--   0        0        0      225 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/rustfmt.toml
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_trader/__init__.pxd
+-rw-r--r--   0        0        0     2270 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_trader/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.pxd
+-rw-r--r--   0        0        0     1414 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.py
+-rw-r--r--   0        0        0     4195 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pxd
+-rw-r--r--   0        0        0    14679 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pyx
+-rw-r--r--   0        0        0     1740 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pxd
+-rw-r--r--   0        0        0     4117 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pyx
+-rw-r--r--   0        0        0     2013 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pxd
+-rw-r--r--   0        0        0    13601 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pyx
+-rw-r--r--   0        0        0     3309 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pxd
+-rw-r--r--   0        0        0    22719 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pyx
+-rw-r--r--   0        0        0     1489 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pxd
+-rw-r--r--   0        0        0    10740 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pyx
+-rw-r--r--   0        0        0     2111 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/error.py
+-rw-r--r--   0        0        0     1089 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pxd
+-rw-r--r--   0        0        0     4065 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pyx
+-rw-r--r--   0        0        0     2653 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pxd
+-rw-r--r--   0        0        0    22688 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pyx
+-rw-r--r--   0        0        0     1153 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/__init__.py
+-rw-r--r--   0        0        0     1013 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/core.py
+-rw-r--r--   0        0        0    14665 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/data.py
+-rw-r--r--   0        0        0     7371 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/execution.py
+-rw-r--r--   0        0        0     2601 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/providers.py
+-rw-r--r--   0        0        0      945 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/__init__.py
+-rw-r--r--   0        0        0    12517 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/client.py
+-rw-r--r--   0        0        0     3924 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/common.py
+-rw-r--r--   0        0        0     2529 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/config.py
+-rw-r--r--   0        0        0     2038 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/constants.py
+-rw-r--r--   0        0        0    12440 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data.py
+-rw-r--r--   0        0        0    10941 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data_types.py
+-rw-r--r--   0        0        0    42389 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/execution.py
+-rw-r--r--   0        0        0     7519 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/factories.py
+-rw-r--r--   0        0        0     1257 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pxd
+-rw-r--r--   0        0        0     1770 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/__init__.py
+-rw-r--r--   0        0        0     3234 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/common.py
+-rw-r--r--   0        0        0     4607 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/core.py
+-rw-r--r--   0        0        0    19955 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/requests.py
+-rw-r--r--   0        0        0    19805 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/streaming.py
+-rw-r--r--   0        0        0    12917 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/providers.py
+-rw-r--r--   0        0        0     9450 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/sockets.py
+-rw-r--r--   0        0        0      938 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/constants.py
+-rw-r--r--   0        0        0     1871 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/credentials.py
+-rw-r--r--   0        0        0    39673 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/data.py
+-rw-r--r--   0        0        0    19212 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/enums.py
+-rw-r--r--   0        0        0    41882 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/execution.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/__init__.py
+-rw-r--r--   0        0        0    10932 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/account.py
+-rw-r--r--   0        0        0    22048 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/market.py
+-rw-r--r--   0        0        0     1209 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/user.py
+-rw-r--r--   0        0        0     2570 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/symbol.py
+-rw-r--r--   0        0        0    15632 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/types.py
+-rw-r--r--   0        0        0     3476 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/urls.py
+-rw-r--r--   0        0        0     5353 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/config.py
+-rw-r--r--   0        0        0    13709 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/factories.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/__init__.py
+-rw-r--r--   0        0        0     6564 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/data.py
+-rw-r--r--   0        0        0     6637 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/enums.py
+-rw-r--r--   0        0        0    13348 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/execution.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/__init__.py
+-rw-r--r--   0        0        0    16026 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/account.py
+-rw-r--r--   0        0        0     3629 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/market.py
+-rw-r--r--   0        0        0     1962 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/user.py
+-rw-r--r--   0        0        0     4834 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/wallet.py
+-rw-r--r--   0        0        0    17736 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/providers.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py
+-rw-r--r--   0        0        0     7352 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/account.py
+-rw-r--r--   0        0        0     7646 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/market.py
+-rw-r--r--   0        0        0    15368 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/user.py
+-rw-r--r--   0        0        0     1281 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py
+-rw-r--r--   0        0        0     5070 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/types.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/__init__.py
+-rw-r--r--   0        0        0    27258 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/account.py
+-rw-r--r--   0        0        0     5511 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/client.py
+-rw-r--r--   0        0        0     3295 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/endpoint.py
+-rw-r--r--   0        0        0     1588 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/error.py
+-rw-r--r--   0        0        0    32496 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/market.py
+-rw-r--r--   0        0        0     7723 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/user.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/__init__.py
+-rw-r--r--   0        0        0     5582 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/data.py
+-rw-r--r--   0        0        0     5563 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/enums.py
+-rw-r--r--   0        0        0    10055 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/execution.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/__init__.py
+-rw-r--r--   0        0        0    26141 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/account.py
+-rw-r--r--   0        0        0     6645 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/market.py
+-rw-r--r--   0        0        0     1968 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/user.py
+-rw-r--r--   0        0        0     4590 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/wallet.py
+-rw-r--r--   0        0        0    13691 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/providers.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py
+-rw-r--r--   0        0        0     3270 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/account.py
+-rw-r--r--   0        0        0     6832 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/market.py
+-rw-r--r--   0        0        0    11717 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/user.py
+-rw-r--r--   0        0        0     1262 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/__init__.py
+-rw-r--r--   0        0        0    16321 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/client.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/__init__.py
+-rw-r--r--   0        0        0     1572 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/constants.py
+-rw-r--r--   0        0        0     1825 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/credentials.py
+-rw-r--r--   0        0        0    10724 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/enums.py
+-rw-r--r--   0        0        0     1502 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/error.py
+-rw-r--r--   0        0        0     4018 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/parsing.py
+-rw-r--r--   0        0        0     4250 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/symbol.py
+-rw-r--r--   0        0        0     2623 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/urls.py
+-rw-r--r--   0        0        0     3425 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/config.py
+-rw-r--r--   0        0        0    28863 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/data.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py
+-rw-r--r--   0        0        0     2369 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py
+-rw-r--r--   0        0        0     2381 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py
+-rw-r--r--   0        0        0     2293 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py
+-rw-r--r--   0        0        0     2594 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py
+-rw-r--r--   0        0        0     3608 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py
+-rw-r--r--   0        0        0     2222 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py
+-rw-r--r--   0        0        0     2060 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py
+-rw-r--r--   0        0        0     3322 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py
+-rw-r--r--   0        0        0     2132 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py
+-rw-r--r--   0        0        0     2866 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py
+-rw-r--r--   0        0        0     2879 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py
+-rw-r--r--   0        0        0     2525 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py
+-rw-r--r--   0        0        0     3228 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py
+-rw-r--r--   0        0        0     2433 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py
+-rw-r--r--   0        0        0     2439 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py
+-rw-r--r--   0        0        0     2466 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py
+-rw-r--r--   0        0        0     2756 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py
+-rw-r--r--   0        0        0     2987 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py
+-rw-r--r--   0        0        0     2679 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py
+-rw-r--r--   0        0        0    35884 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/execution.py
+-rw-r--r--   0        0        0     9039 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/factories.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/__init__.py
+-rw-r--r--   0        0        0    13207 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/account.py
+-rw-r--r--   0        0        0     1963 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/asset.py
+-rw-r--r--   0        0        0     6629 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/client.py
+-rw-r--r--   0        0        0     1083 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/errors.py
+-rw-r--r--   0        0        0     7979 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/market.py
+-rw-r--r--   0        0        0     1180 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/user.py
+-rw-r--r--   0        0        0    11303 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/providers.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py
+-rw-r--r--   0        0        0     3413 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/balance.py
+-rw-r--r--   0        0        0     1204 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py
+-rw-r--r--   0        0        0     1947 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py
+-rw-r--r--   0        0        0     2114 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/common.py
+-rw-r--r--   0        0        0    15794 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/instrument.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py
+-rw-r--r--   0        0        0     2184 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/kline.py
+-rw-r--r--   0        0        0     4540 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py
+-rw-r--r--   0        0        0     1088 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py
+-rw-r--r--   0        0        0     4461 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py
+-rw-r--r--   0        0        0     2476 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/trades.py
+-rw-r--r--   0        0        0     9705 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/order.py
+-rw-r--r--   0        0        0     2665 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/position.py
+-rw-r--r--   0        0        0     4044 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/trade.py
+-rw-r--r--   0        0        0    21528 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/ws.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/__init__.py
+-rw-r--r--   0        0        0    11105 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/client.py
+-rw-r--r--   0        0        0     1689 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/__init__.py
+-rw-r--r--   0        0        0     2749 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/common.py
+-rw-r--r--   0        0        0     2727 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/config.py
+-rw-r--r--   0        0        0     1210 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/constants.py
+-rw-r--r--   0        0        0    39036 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/data.py
+-rw-r--r--   0        0        0     1315 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/enums.py
+-rw-r--r--   0        0        0     6043 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/factories.py
+-rw-r--r--   0        0        0    10712 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/loaders.py
+-rw-r--r--   0        0        0    10149 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/providers.py
+-rw-r--r--   0        0        0    10104 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/publishers.json
+-rw-r--r--   0        0        0     1141 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/types.py
+-rw-r--r--   0        0        0     1193 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/env.py
+-rw-r--r--   0        0        0      930 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/__init__.py
+-rw-r--r--   0        0        0     1014 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py
+-rw-r--r--   0        0        0     6415 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/account.py
+-rw-r--r--   0        0        0    26860 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/client.py
+-rw-r--r--   0        0        0    15878 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/common.py
+-rw-r--r--   0        0        0     8356 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/connection.py
+-rw-r--r--   0        0        0     7167 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/contract.py
+-rw-r--r--   0        0        0     8724 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/error.py
+-rw-r--r--   0        0        0    32019 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py
+-rw-r--r--   0        0        0    10341 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/order.py
+-rw-r--r--   0        0        0    43317 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py
+-rw-r--r--   0        0        0     6988 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/common.py
+-rw-r--r--   0        0        0     8127 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/config.py
+-rw-r--r--   0        0        0    17152 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/data.py
+-rw-r--r--   0        0        0    39055 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/execution.py
+-rw-r--r--   0        0        0     9005 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/factories.py
+-rw-r--r--   0        0        0     7876 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/gateway.py
+-rw-r--r--   0        0        0     1054 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py
+-rw-r--r--   0        0        0    21095 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/client.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py
+-rw-r--r--   0        0        0     3579 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py
+-rw-r--r--   0        0        0     4007 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py
+-rw-r--r--   0        0        0    24117 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py
+-rw-r--r--   0        0        0    12263 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/providers.py
+-rw-r--r--   0        0        0     4904 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/web.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/__init__.py
+-rw-r--r--   0        0        0     2360 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/config.py
+-rw-r--r--   0        0        0     8365 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/execution.py
+-rw-r--r--   0        0        0     2676 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/factory.py
+-rw-r--r--   0        0        0      937 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/loaders.py
+-rw-r--r--   0        0        0      978 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/__init__.py
+-rw-r--r--   0        0        0    15183 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/analyzer.py
+-rw-r--r--   0        0        0     5714 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/reporter.py
+-rw-r--r--   0        0        0     3940 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistic.py
+-rw-r--r--   0        0        0     2255 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/__init__.py
+-rw-r--r--   0        0        0     1997 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/expectancy.py
+-rw-r--r--   0        0        0     1705 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/long_ratio.py
+-rw-r--r--   0        0        0     1468 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_avg.py
+-rw-r--r--   0        0        0     1514 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_max.py
+-rw-r--r--   0        0        0     1512 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_min.py
+-rw-r--r--   0        0        0     1563 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/profit_factor.py
+-rw-r--r--   0        0        0     1399 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg.py
+-rw-r--r--   0        0        0     1414 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_loss.py
+-rw-r--r--   0        0        0     1413 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_win.py
+-rw-r--r--   0        0        0     1716 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_volatility.py
+-rw-r--r--   0        0        0     1323 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/risk_return_ratio.py
+-rw-r--r--   0        0        0     1776 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sharpe_ratio.py
+-rw-r--r--   0        0        0     1883 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sortino_ratio.py
+-rw-r--r--   0        0        0     1498 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/win_rate.py
+-rw-r--r--   0        0        0     1489 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_avg.py
+-rw-r--r--   0        0        0     1347 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_max.py
+-rw-r--r--   0        0        0     1494 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_min.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.pxd
+-rw-r--r--   0        0        0      946 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.py
+-rw-r--r--   0        0        0     1868 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/__main__.py
+-rw-r--r--   0        0        0     3840 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/auction.py
+-rw-r--r--   0        0        0     9257 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/config.py
+-rw-r--r--   0        0        0     1100 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pxd
+-rw-r--r--   0        0        0    13931 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pyx
+-rw-r--r--   0        0        0     2162 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pxd
+-rw-r--r--   0        0        0    51527 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pyx
+-rw-r--r--   0        0        0     7614 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pxd
+-rw-r--r--   0        0        0    31318 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pyx
+-rw-r--r--   0        0        0     1084 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pxd
+-rw-r--r--   0        0        0     5264 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pyx
+-rw-r--r--   0        0        0    12270 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pxd
+-rw-r--r--   0        0        0    98825 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pyx
+-rw-r--r--   0        0        0     2658 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/models.pxd
+-rw-r--r--   0        0        0     8785 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/models.pyx
+-rw-r--r--   0        0        0     1893 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pxd
+-rw-r--r--   0        0        0     8483 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pyx
+-rw-r--r--   0        0        0    15294 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/node.py
+-rw-r--r--   0        0        0     3072 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/results.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/__init__.pxd
+-rw-r--r--   0        0        0     1220 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/__init__.py
+-rw-r--r--   0        0        0    10536 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/base.pxd
+-rw-r--r--   0        0        0    25831 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/base.pyx
+-rw-r--r--   0        0        0     8701 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/cache.pxd
+-rw-r--r--   0        0        0   135124 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/cache.pyx
+-rw-r--r--   0        0        0     2884 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/config.py
+-rw-r--r--   0        0        0     1104 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/database.pxd
+-rw-r--r--   0        0        0    36283 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/database.pyx
+-rw-r--r--   0        0        0     5051 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/facade.pxd
+-rw-r--r--   0        0        0    11952 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/facade.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/postgres/__init__.py
+-rw-r--r--   0        0        0     4228 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/postgres/adapter.py
+-rw-r--r--   0        0        0    12833 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/postgres/transformers.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/__init__.pxd
+-rw-r--r--   0        0        0     1571 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/__init__.py
+-rw-r--r--   0        0        0    11890 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/actor.pxd
+-rw-r--r--   0        0        0    92278 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/actor.pyx
+-rw-r--r--   0        0        0    11128 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/component.pxd
+-rw-r--r--   0        0        0    88235 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/component.pyx
+-rw-r--r--   0        0        0    16788 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/config.py
+-rw-r--r--   0        0        0     1849 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/enums.py
+-rw-r--r--   0        0        0    10785 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/executor.py
+-rw-r--r--   0        0        0     9517 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/factories.pxd
+-rw-r--r--   0        0        0    58923 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/factories.pyx
+-rw-r--r--   0        0        0     1320 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/functions.py
+-rw-r--r--   0        0        0     2143 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/generators.pxd
+-rw-r--r--   0        0        0     7841 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/generators.pyx
+-rw-r--r--   0        0        0     2723 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/messages.pxd
+-rw-r--r--   0        0        0    11741 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/messages.pyx
+-rw-r--r--   0        0        0    10413 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/providers.py
+-rw-r--r--   0        0        0     5512 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/config/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/__init__.pxd
+-rw-r--r--   0        0        0     1339 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/__init__.py
+-rw-r--r--   0        0        0     1230 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/asynchronous.py
+-rw-r--r--   0        0        0     3683 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/correctness.pxd
+-rw-r--r--   0        0        0    37316 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/correctness.pyx
+-rw-r--r--   0        0        0      897 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/data.pxd
+-rw-r--r--   0        0        0     1954 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/data.pyx
+-rw-r--r--   0        0        0     1363 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/datetime.pxd
+-rw-r--r--   0        0        0     7616 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/datetime.pyx
+-rw-r--r--   0        0        0     1230 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/fsm.pxd
+-rw-r--r--   0        0        0     4364 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/fsm.pyx
+-rw-r--r--   0        0        0     2511 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/algorithms.h
+-rw-r--r--   0        0        0      907 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/backtest.h
+-rw-r--r--   0        0        0    15890 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/common.h
+-rw-r--r--   0        0        0     3055 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/core.h
+-rw-r--r--   0        0        0    65849 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/model.h
+-rw-r--r--   0        0        0     2529 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/inspect.py
+-rw-r--r--   0        0        0     2137 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/message.pxd
+-rw-r--r--   0        0        0     6509 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/message.pyx
+-rw-r--r--   0        0        0    87295 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/nautilus_pyo3.pyi
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/__init__.pxd
+-rw-r--r--   0        0        0     2685 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/algorithms.pxd
+-rw-r--r--   0        0        0     1050 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/backtest.pxd
+-rw-r--r--   0        0        0    15615 2024-05-24 12:19:06.972391 nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pxd
+-rw-r--r--   0        0        0     1222 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pyx
+-rw-r--r--   0        0        0     3107 2024-05-24 12:16:20.244731 nautilus_trader-1.193.0/nautilus_trader/core/rust/core.pxd
+-rw-r--r--   0        0        0    61890 2024-05-24 12:17:40.812571 nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pxd
+-rw-r--r--   0        0        0     2702 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pyx
+-rw-r--r--   0        0        0     1359 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/stats.pxd
+-rw-r--r--   0        0        0     5710 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/stats.pyx
+-rw-r--r--   0        0        0     3870 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/string.pxd
+-rw-r--r--   0        0        0     1049 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/uuid.pxd
+-rw-r--r--   0        0        0     2755 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/uuid.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/__init__.pxd
+-rw-r--r--   0        0        0     1360 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/__init__.py
+-rw-r--r--   0        0        0     4191 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pxd
+-rw-r--r--   0        0        0    24575 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pyx
+-rw-r--r--   0        0        0     8072 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/client.pxd
+-rw-r--r--   0        0        0    39952 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/client.pyx
+-rw-r--r--   0        0        0     2142 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/config.py
+-rw-r--r--   0        0        0    10088 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/engine.pxd
+-rw-r--r--   0        0        0    65384 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/engine.pyx
+-rw-r--r--   0        0        0     2391 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/messages.pxd
+-rw-r--r--   0        0        0     8362 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/messages.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/__init__.py
+-rw-r--r--   0        0        0     4226 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/blank.py
+-rw-r--r--   0        0        0    11242 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/twap.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/blank.py
+-rw-r--r--   0        0        0    11736 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross.py
+-rw-r--r--   0        0        0    11534 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket.py
+-rw-r--r--   0        0        0    14158 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py
+-rw-r--r--   0        0        0    10284 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx
+-rw-r--r--   0        0        0    11178 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_long_only.py
+-rw-r--r--   0        0        0    15993 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py
+-rw-r--r--   0        0        0    14118 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py
+-rw-r--r--   0        0        0    12012 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_twap.py
+-rw-r--r--   0        0        0     5286 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/market_maker.py
+-rw-r--r--   0        0        0     8954 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance.py
+-rw-r--r--   0        0        0     9291 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py
+-rw-r--r--   0        0        0     2839 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/signal_strategy.py
+-rw-r--r--   0        0        0     4718 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/subscribe.py
+-rw-r--r--   0        0        0     7283 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/talib_strategy.py
+-rw-r--r--   0        0        0    14071 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/volatility_market_maker.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/__init__.pxd
+-rw-r--r--   0        0        0     1353 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/__init__.py
+-rw-r--r--   0        0        0     8527 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pxd
+-rw-r--r--   0        0        0    52607 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pyx
+-rw-r--r--   0        0        0     7359 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/client.pxd
+-rw-r--r--   0        0        0    29170 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/client.pyx
+-rw-r--r--   0        0        0     3587 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/config.py
+-rw-r--r--   0        0        0     4001 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pxd
+-rw-r--r--   0        0        0    35586 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pyx
+-rw-r--r--   0        0        0     6956 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/engine.pxd
+-rw-r--r--   0        0        0    46472 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/engine.pyx
+-rw-r--r--   0        0        0     4593 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/manager.pxd
+-rw-r--r--   0        0        0    24284 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/manager.pyx
+-rw-r--r--   0        0        0     3590 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pxd
+-rw-r--r--   0        0        0    16178 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pyx
+-rw-r--r--   0        0        0     5598 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/messages.pxd
+-rw-r--r--   0        0        0    34648 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/messages.pyx
+-rw-r--r--   0        0        0    22236 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/reports.py
+-rw-r--r--   0        0        0     1726 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pxd
+-rw-r--r--   0        0        0    17089 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.pxd
+-rw-r--r--   0        0        0     1188 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.py
+-rw-r--r--   0        0        0     1722 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pxd
+-rw-r--r--   0        0        0     4832 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pyx
+-rw-r--r--   0        0        0     1482 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pxd
+-rw-r--r--   0        0        0     3470 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pyx
+-rw-r--r--   0        0        0     1474 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pxd
+-rw-r--r--   0        0        0     4320 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pxd
+-rw-r--r--   0        0        0     5185 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pyx
+-rw-r--r--   0        0        0     1063 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pxd
+-rw-r--r--   0        0        0     3840 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pyx
+-rw-r--r--   0        0        0     1096 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pxd
+-rw-r--r--   0        0        0     3454 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pyx
+-rw-r--r--   0        0        0     1247 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pxd
+-rw-r--r--   0        0        0     4323 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pyx
+-rw-r--r--   0        0        0     3114 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ma_factory.pyx
+-rw-r--r--   0        0        0     1568 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pxd
+-rw-r--r--   0        0        0     2960 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pyx
+-rw-r--r--   0        0        0     1080 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pxd
+-rw-r--r--   0        0        0     3466 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pyx
+-rw-r--r--   0        0        0     1020 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pxd
+-rw-r--r--   0        0        0     3530 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pyx
+-rw-r--r--   0        0        0     1283 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pxd
+-rw-r--r--   0        0        0     4592 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pyx
+-rw-r--r--   0        0        0     1174 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pxd
+-rw-r--r--   0        0        0     4700 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.py
+-rw-r--r--   0        0        0     1701 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pxd
+-rw-r--r--   0        0        0     3029 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pyx
+-rw-r--r--   0        0        0     1315 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pxd
+-rw-r--r--   0        0        0     2868 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pyx
+-rw-r--r--   0        0        0     1579 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pxd
+-rw-r--r--   0        0        0     5219 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pyx
+-rw-r--r--   0        0        0     1635 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pxd
+-rw-r--r--   0        0        0     4056 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pyx
+-rw-r--r--   0        0        0     1375 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pxd
+-rw-r--r--   0        0        0     3766 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pyx
+-rw-r--r--   0        0        0     1658 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pxd
+-rw-r--r--   0        0        0     3732 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pyx
+-rw-r--r--   0        0        0     1490 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pxd
+-rw-r--r--   0        0        0     4374 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pyx
+-rw-r--r--   0        0        0     1231 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pxd
+-rw-r--r--   0        0        0     3119 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pyx
+-rw-r--r--   0        0        0     3168 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd
+-rw-r--r--   0        0        0    12540 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx
+-rw-r--r--   0        0        0     1347 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enum.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.py
+-rw-r--r--   0        0        0      976 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd
+-rw-r--r--   0        0        0      980 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx
+-rw-r--r--   0        0        0      947 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd
+-rw-r--r--   0        0        0      987 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx
+-rw-r--r--   0        0        0     1020 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd
+-rw-r--r--   0        0        0      972 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx
+-rw-r--r--   0        0        0      972 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd
+-rw-r--r--   0        0        0      980 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx
+-rw-r--r--   0        0        0     1805 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pxd
+-rw-r--r--   0        0        0     4675 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pyx
+-rw-r--r--   0        0        0     1395 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pxd
+-rw-r--r--   0        0        0     4280 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pyx
+-rw-r--r--   0        0        0     1713 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pxd
+-rw-r--r--   0        0        0     4727 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pyx
+-rw-r--r--   0        0        0     1636 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pxd
+-rw-r--r--   0        0        0     3839 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pyx
+-rw-r--r--   0        0        0     1664 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pxd
+-rw-r--r--   0        0        0     4809 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pyx
+-rw-r--r--   0        0        0     1232 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pxd
+-rw-r--r--   0        0        0     2958 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pyx
+-rw-r--r--   0        0        0     1514 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pxd
+-rw-r--r--   0        0        0     4383 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pyx
+-rw-r--r--   0        0        0     1476 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pxd
+-rw-r--r--   0        0        0     3311 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pyx
+-rw-r--r--   0        0        0     1227 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pxd
+-rw-r--r--   0        0        0     2726 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pyx
+-rw-r--r--   0        0        0     1393 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pxd
+-rw-r--r--   0        0        0     3767 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pyx
+-rw-r--r--   0        0        0     1763 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pxd
+-rw-r--r--   0        0        0     4539 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pyx
+-rw-r--r--   0        0        0     1444 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pxd
+-rw-r--r--   0        0        0     3391 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pyx
+-rw-r--r--   0        0        0     1485 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pxd
+-rw-r--r--   0        0        0     3884 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pyx
+-rw-r--r--   0        0        0     2271 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pxd
+-rw-r--r--   0        0        0     4678 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/__init__.py
+-rw-r--r--   0        0        0     1993 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/common.py
+-rw-r--r--   0        0        0    29656 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/manager.py
+-rw-r--r--   0        0        0     1458 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pxd
+-rw-r--r--   0        0        0     3513 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pyx
+-rw-r--r--   0        0        0     1485 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pxd
+-rw-r--r--   0        0        0     4482 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pyx
+-rw-r--r--   0        0        0     1270 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pxd
+-rw-r--r--   0        0        0     2938 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pyx
+-rw-r--r--   0        0        0     1155 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/__init__.py
+-rw-r--r--   0        0        0     1861 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/__main__.py
+-rw-r--r--   0        0        0     8314 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/config.py
+-rw-r--r--   0        0        0    34312 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/data_client.py
+-rw-r--r--   0        0        0    16375 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/data_engine.py
+-rw-r--r--   0        0        0    18927 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/execution_client.py
+-rw-r--r--   0        0        0    41082 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/execution_engine.py
+-rw-r--r--   0        0        0     3395 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/factories.py
+-rw-r--r--   0        0        0    16754 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/node.py
+-rw-r--r--   0        0        0     9369 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/node_builder.py
+-rw-r--r--   0        0        0     9696 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/risk_engine.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/__init__.pxd
+-rw-r--r--   0        0        0     1652 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/__init__.py
+-rw-r--r--   0        0        0     3380 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/book.pxd
+-rw-r--r--   0        0        0    24325 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/book.pyx
+-rw-r--r--   0        0        0     5067 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/currencies.py
+-rw-r--r--   0        0        0    13066 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/data.pxd
+-rw-r--r--   0        0        0   126566 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/data.pyx
+-rw-r--r--   0        0        0     7811 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/enums.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.pxd
+-rw-r--r--   0        0        0     2829 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/account.pxd
+-rw-r--r--   0        0        0     6660 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/account.pyx
+-rw-r--r--   0        0        0    12302 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/order.pxd
+-rw-r--r--   0        0        0   136228 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/order.pyx
+-rw-r--r--   0        0        0     5628 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/position.pxd
+-rw-r--r--   0        0        0    35393 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/position.pyx
+-rw-r--r--   0        0        0     5142 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/functions.pxd
+-rw-r--r--   0        0        0    10333 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/functions.pyx
+-rw-r--r--   0        0        0     4039 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pxd
+-rw-r--r--   0        0        0    27544 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.pxd
+-rw-r--r--   0        0        0     2302 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.py
+-rw-r--r--   0        0        0     5519 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pxd
+-rw-r--r--   0        0        0    21031 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pyx
+-rw-r--r--   0        0        0     1778 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pxd
+-rw-r--r--   0        0        0     8622 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pyx
+-rw-r--r--   0        0        0     1449 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pxd
+-rw-r--r--   0        0        0    13625 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pyx
+-rw-r--r--   0        0        0     1296 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pxd
+-rw-r--r--   0        0        0    13011 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pyx
+-rw-r--r--   0        0        0     1756 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pxd
+-rw-r--r--   0        0        0    14480 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pyx
+-rw-r--r--   0        0        0     1563 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pxd
+-rw-r--r--   0        0        0    13388 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pyx
+-rw-r--r--   0        0        0     1334 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pxd
+-rw-r--r--   0        0        0    13495 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pyx
+-rw-r--r--   0        0        0     1284 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pxd
+-rw-r--r--   0        0        0     9201 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pyx
+-rw-r--r--   0        0        0     1736 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pxd
+-rw-r--r--   0        0        0    11356 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pyx
+-rw-r--r--   0        0        0     1824 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pxd
+-rw-r--r--   0        0        0    11963 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pyx
+-rw-r--r--   0        0        0     2068 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pxd
+-rw-r--r--   0        0        0    12508 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pyx
+-rw-r--r--   0        0        0     1930 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pxd
+-rw-r--r--   0        0        0    12096 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pyx
+-rw-r--r--   0        0        0     1555 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pxd
+-rw-r--r--   0        0        0    12487 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pyx
+-rw-r--r--   0        0        0     5934 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/objects.pxd
+-rw-r--r--   0        0        0    52381 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/objects.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.pxd
+-rw-r--r--   0        0        0     2094 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.py
+-rw-r--r--   0        0        0     9471 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pxd
+-rw-r--r--   0        0        0    37731 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pyx
+-rw-r--r--   0        0        0     1770 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pxd
+-rw-r--r--   0        0        0    21400 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pyx
+-rw-r--r--   0        0        0     2175 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pxd
+-rw-r--r--   0        0        0    17609 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pyx
+-rw-r--r--   0        0        0     1842 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pxd
+-rw-r--r--   0        0        0     2365 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pyx
+-rw-r--r--   0        0        0     1272 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pxd
+-rw-r--r--   0        0        0    15939 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pyx
+-rw-r--r--   0        0        0     1612 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pxd
+-rw-r--r--   0        0        0    15818 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pyx
+-rw-r--r--   0        0        0     1646 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pxd
+-rw-r--r--   0        0        0    14283 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pyx
+-rw-r--r--   0        0        0     2232 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pxd
+-rw-r--r--   0        0        0    20646 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pyx
+-rw-r--r--   0        0        0     1602 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pxd
+-rw-r--r--   0        0        0    16030 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pyx
+-rw-r--r--   0        0        0     2647 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pxd
+-rw-r--r--   0        0        0    19580 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pyx
+-rw-r--r--   0        0        0     1953 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pxd
+-rw-r--r--   0        0        0    17208 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pyx
+-rw-r--r--   0        0        0     1141 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pxd
+-rw-r--r--   0        0        0     3926 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pyx
+-rw-r--r--   0        0        0     6940 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/position.pxd
+-rw-r--r--   0        0        0    23901 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/position.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.pxd
+-rw-r--r--   0        0        0     1443 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.py
+-rw-r--r--   0        0        0     1581 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pxd
+-rw-r--r--   0        0        0     3709 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pyx
+-rw-r--r--   0        0        0     1147 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd
+-rw-r--r--   0        0        0     3921 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx
+-rw-r--r--   0        0        0     1388 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd
+-rw-r--r--   0        0        0     5436 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx
+-rw-r--r--   0        0        0     1333 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/venues.py
+-rw-r--r--   0        0        0      973 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/__init__.py
+-rw-r--r--   0        0        0     1079 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/__init__.py
+-rw-r--r--   0        0        0     6321 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/base.py
+-rw-r--r--   0        0        0    28127 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/parquet.py
+-rw-r--r--   0        0        0     2073 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/singleton.py
+-rw-r--r--   0        0        0     1327 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/types.py
+-rw-r--r--   0        0        0     2886 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/config.py
+-rw-r--r--   0        0        0     3561 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/funcs.py
+-rw-r--r--   0        0        0     7025 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/loaders.py
+-rw-r--r--   0        0        0     3392 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pxd
+-rw-r--r--   0        0        0    30305 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pyx
+-rw-r--r--   0        0        0    16480 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers_v2.py
+-rw-r--r--   0        0        0    12974 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/writer.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.pxd
+-rw-r--r--   0        0        0     1123 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     2132 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pxd
+-rw-r--r--   0        0        0     4233 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pyx
+-rw-r--r--   0        0        0     3111 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pxd
+-rw-r--r--   0        0        0    38292 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pyx
+-rw-r--r--   0        0        0        0 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/py.typed
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/__init__.pxd
+-rw-r--r--   0        0        0     1084 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/__init__.py
+-rw-r--r--   0        0        0     1974 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/config.py
+-rw-r--r--   0        0        0     5474 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/engine.pxd
+-rw-r--r--   0        0        0    38261 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/engine.pyx
+-rw-r--r--   0        0        0     1747 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pxd
+-rw-r--r--   0        0        0     7059 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.pxd
+-rw-r--r--   0        0        0     1106 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/__init__.py
+-rw-r--r--   0        0        0     5360 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/account_state.py
+-rw-r--r--   0        0        0     1689 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/component_events.py
+-rw-r--r--   0        0        0    14111 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/instruments.py
+-rw-r--r--   0        0        0     2191 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/order_events.py
+-rw-r--r--   0        0        0     5923 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/position_events.py
+-rw-r--r--   0        0        0    15753 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/schema.py
+-rw-r--r--   0        0        0    13886 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/serializer.py
+-rw-r--r--   0        0        0     1096 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/base.pxd
+-rw-r--r--   0        0        0    12000 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/base.pyx
+-rw-r--r--   0        0        0     1303 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pxd
+-rw-r--r--   0        0        0     5404 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pyx
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/system/__init__.py
+-rw-r--r--   0        0        0     6506 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/system/config.py
+-rw-r--r--   0        0        0    40208 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/system/kernel.py
+-rw-r--r--   0        0        0     1034 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/functions.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/__init__.py
+-rw-r--r--   0        0        0     6382 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/actors.py
+-rw-r--r--   0        0        0     5793 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/cache_database.py
+-rw-r--r--   0        0        0     1550 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/controller.py
+-rw-r--r--   0        0        0     3177 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/data.py
+-rw-r--r--   0        0        0     2976 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/engines.py
+-rw-r--r--   0        0        0    12678 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/exec_clients.py
+-rw-r--r--   0        0        0     7299 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/strategies.py
+-rw-r--r--   0        0        0    29811 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/providers.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/__init__.py
+-rw-r--r--   0        0        0     3697 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/accounting_pyo3.py
+-rw-r--r--   0        0        0     6642 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/data_pyo3.py
+-rw-r--r--   0        0        0    19951 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/events_pyo3.py
+-rw-r--r--   0        0        0     3912 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py
+-rw-r--r--   0        0        0    15113 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/instruments_pyo3.py
+-rw-r--r--   0        0        0     5508 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/orders_pyo3.py
+-rw-r--r--   0        0        0     2451 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/types_pyo3.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/__init__.py
+-rw-r--r--   0        0        0     4828 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/commands.py
+-rw-r--r--   0        0        0     5842 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/component.py
+-rw-r--r--   0        0        0     6234 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/config.py
+-rw-r--r--   0        0        0    22352 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/data.py
+-rw-r--r--   0        0        0    14777 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/events.py
+-rw-r--r--   0        0        0     9471 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/execution.py
+-rw-r--r--   0        0        0     3991 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/identifiers.py
+-rw-r--r--   0        0        0     3415 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/persistence.py
+-rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/__init__.pxd
+-rw-r--r--   0        0        0     1372 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/__init__.py
+-rw-r--r--   0        0        0     4730 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/config.py
+-rw-r--r--   0        0        0     5493 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/controller.py
+-rw-r--r--   0        0        0    18226 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/filters.py
+-rw-r--r--   0        0        0     8699 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pxd
+-rw-r--r--   0        0        0    59399 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pyx
+-rw-r--r--   0        0        0    25167 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/trader.py
+-rw-r--r--   0        0        0     8001 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/pyproject.toml
+-rw-r--r--   0        0        0    27266 1970-01-01 00:00:00.000000 nautilus_trader-1.193.0/PKG-INFO
```

### Comparing `nautilus_trader-1.192.0/LICENSE` & `nautilus_trader-1.193.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/README.md` & `nautilus_trader-1.193.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 | `master`  | ![version](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnautechsystems%2Fnautilus_trader%2Fmaster%2Fversion.json)  | [![build](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml)  |
 | `nightly` | ![version](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnautechsystems%2Fnautilus_trader%2Fnightly%2Fversion.json) | [![build](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml/badge.svg?branch=nightly)](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml) |
 | `develop` | ![version](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnautechsystems%2Fnautilus_trader%2Fdevelop%2Fversion.json) | [![build](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml/badge.svg?branch=develop)](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml) |
 
 | Platform           | Rust    | Python |
 | :----------------- | :------ | :----- |
 | `Linux (x86_64)`   | 1.78.0+ | 3.10+  |
-| `macOS (x86_64)`   | 1.78.0+ | 3.10+  |
 | `macOS (arm64)`    | 1.78.0+ | 3.10+  |
 | `Windows (x86_64)` | 1.78.0+ | 3.10+  |
 
 - **Website:** https://nautilustrader.io
 - **Docs:** https://docs.nautilustrader.io
 - **Support:** [support@nautilustrader.io](mailto:support@nautilustrader.io)
```

### Comparing `nautilus_trader-1.192.0/build.py` & `nautilus_trader-1.193.0/build.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/.cargo/config.toml` & `nautilus_trader-1.193.0/nautilus_core/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/Cargo.lock` & `nautilus_trader-1.193.0/nautilus_core/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.84"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18b8795de6d09abb2b178fa5a9e3bb10da935750f33449a132b328b9391b2c6a"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "arc-swap"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
@@ -404,15 +404,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -449,18 +449,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a6c9af12842a67734c9a2e355436e5d03b22383ed60cf13cd0c18fbfe3dcbcf"
 dependencies = [
  "async-trait",
  "axum-core",
  "bytes",
  "futures-util",
- "http 1.1.0",
- "http-body 1.0.0",
+ "http",
+ "http-body",
  "http-body-util",
- "hyper 1.3.1",
+ "hyper",
  "hyper-util",
  "itoa",
  "matchit",
  "memchr",
  "mime",
  "percent-encoding",
  "pin-project-lite",
@@ -482,16 +482,16 @@
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a15c63fd72d41492dc4f497196f5da1fb04fb7529e631d73630d1b491e47a2e3"
 dependencies = [
  "async-trait",
  "bytes",
  "futures-util",
- "http 1.1.0",
- "http-body 1.0.0",
+ "http",
+ "http-body",
  "http-body-util",
  "mime",
  "pin-project-lite",
  "rustversion",
  "sync_wrapper 0.1.2",
  "tower-layer",
  "tower-service",
@@ -592,15 +592,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d7a8646f94ab393e43e8b35a2558b1624bed28b97ee09c5d15456e3c9463f46d"
 dependencies = [
  "once_cell",
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
  "syn_derive",
 ]
 
 [[package]]
 name = "brotli"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -711,17 +711,17 @@
  "syn 1.0.109",
  "tempfile",
  "toml",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.97"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -841,15 +841,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
@@ -974,17 +974,17 @@
 name = "crc-catalog"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19d374276b40fb8bbdee95aef7c7fa6b5316ec764510eb64b8dd0e2ed0d7e7f5"
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.5.1"
@@ -1047,17 +1047,17 @@
 checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -1109,26 +1109,26 @@
 checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim 0.11.1",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
 dependencies = [
  "darling_core",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
@@ -1144,23 +1144,23 @@
 name = "data-encoding"
 version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8566979429cf69b49a5c740c60791108e86440e8be149bbea4fe54d2c32d6e2"
 
 [[package]]
 name = "databento"
-version = "0.9.1"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a338c81ee0781aa34b24423ca61c083620284e2a1a1198d20e73fb52e63ba2cd"
+checksum = "958e83b1f051563971485b8b8acf6de4fe016ec5d4e9cf3e10aa810416b7d160"
 dependencies = [
  "dbn",
  "futures",
  "hex",
  "log",
- "reqwest 0.11.27",
+ "reqwest",
  "serde",
  "serde_json",
  "sha2",
  "thiserror",
  "time",
  "tokio",
  "tokio-util",
@@ -1436,42 +1436,42 @@
  "log",
  "sqlparser",
  "strum",
 ]
 
 [[package]]
 name = "dbn"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75c616347fc28872f993b5e9b80a5d25128db3557b852fc6642a0739b2f97003"
+checksum = "f78191ea0a044d346c1d05b11325414bc6d615c6bfdda4934634b19291295b92"
 dependencies = [
  "async-compression",
  "csv",
  "dbn-macros",
+ "fallible-streaming-iterator",
  "itoa",
  "json-writer",
  "num_enum",
  "serde",
- "streaming-iterator",
  "thiserror",
  "time",
  "tokio",
  "zstd",
 ]
 
 [[package]]
 name = "dbn-macros"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "405f6fb410dad990ea1e56ce02609ea103ffd5c153c489c770c909e3bb7b165c"
+checksum = "8a1fea28cc8c78a5626ea0d4965f896ef65466237c497f5373d2264eac803011"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "der"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
@@ -1505,25 +1505,25 @@
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "derive_builder_macro"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
@@ -1622,14 +1622,20 @@
 [[package]]
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
+name = "fallible-streaming-iterator"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7360491ce676a36bf9bb3c56c1aa791658183a54d2744120f27285738d90465a"
+
+[[package]]
 name = "fastrand"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "finl_unicode"
@@ -1782,15 +1788,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1833,17 +1839,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -1856,43 +1862,24 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
-dependencies = [
- "bytes",
- "fnv",
- "futures-core",
- "futures-sink",
- "futures-util",
- "http 0.2.12",
- "indexmap 2.2.6",
- "slab",
- "tokio",
- "tokio-util",
- "tracing",
-]
-
-[[package]]
-name = "h2"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa82e28a107a8cc405f0839610bdc9b15f1e25ec7d696aa5cf173edbcb1486ab"
 dependencies = [
  "atomic-waker",
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
- "http 1.1.0",
+ "http",
  "indexmap 2.2.6",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
@@ -1996,65 +1983,43 @@
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
-dependencies = [
- "bytes",
- "fnv",
- "itoa",
-]
-
-[[package]]
-name = "http"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
-dependencies = [
- "bytes",
- "http 0.2.12",
- "pin-project-lite",
-]
-
-[[package]]
-name = "http-body"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
 dependencies = [
  "bytes",
- "http 1.1.0",
+ "http",
 ]
 
 [[package]]
 name = "http-body-util"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
 dependencies = [
  "bytes",
  "futures-core",
- "http 1.1.0",
- "http-body 1.0.0",
+ "http",
+ "http-body",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2070,79 +2035,42 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
-dependencies = [
- "bytes",
- "futures-channel",
- "futures-core",
- "futures-util",
- "h2 0.3.26",
- "http 0.2.12",
- "http-body 0.4.6",
- "httparse",
- "httpdate",
- "itoa",
- "pin-project-lite",
- "socket2",
- "tokio",
- "tower-service",
- "tracing",
- "want",
-]
-
-[[package]]
-name = "hyper"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
- "h2 0.4.5",
- "http 1.1.0",
- "http-body 1.0.0",
+ "h2",
+ "http",
+ "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "smallvec",
  "tokio",
  "want",
 ]
 
 [[package]]
 name = "hyper-tls"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
-dependencies = [
- "bytes",
- "hyper 0.14.28",
- "native-tls",
- "tokio",
- "tokio-native-tls",
-]
-
-[[package]]
-name = "hyper-tls"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "70206fc6890eaca9fde8a0bf71caa2ddfc9fe045ac9e5c70df101a7dbde866e0"
 dependencies = [
  "bytes",
  "http-body-util",
- "hyper 1.3.1",
+ "hyper",
  "hyper-util",
  "native-tls",
  "tokio",
  "tokio-native-tls",
  "tower-service",
 ]
 
@@ -2151,17 +2079,17 @@
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
- "http 1.1.0",
- "http-body 1.0.0",
- "hyper 1.3.1",
+ "http",
+ "http-body",
+ "hyper",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower",
  "tower-service",
  "tracing",
 ]
@@ -2402,17 +2330,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -2561,15 +2489,15 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "nautilus-accounting"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "nautilus-common",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
@@ -2577,46 +2505,46 @@
  "rust_decimal",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "nautilus-adapters"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "chrono",
  "criterion",
  "databento",
+ "fallible-streaming-iterator",
  "indexmap 2.2.6",
  "itoa",
  "log",
  "nautilus-common",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
  "pyo3-asyncio",
  "rand",
  "rstest",
  "rust_decimal",
  "rust_decimal_macros",
  "serde",
  "serde_json",
- "streaming-iterator",
  "strum",
  "thiserror",
  "time",
  "tokio",
  "tracing",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-backtest"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "log",
  "nautilus-common",
  "nautilus-core",
  "nautilus-execution",
@@ -2625,15 +2553,15 @@
  "rstest",
  "tempfile",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-cli"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "clap 4.5.4",
  "clap_derive",
  "dotenvy",
  "log",
  "nautilus-common",
@@ -2642,15 +2570,15 @@
  "nautilus-model",
  "simple_logger",
  "tokio",
 ]
 
 [[package]]
 name = "nautilus-common"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "chrono",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "log",
@@ -2670,15 +2598,15 @@
  "tracing",
  "tracing-subscriber",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-core"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "chrono",
  "criterion",
  "heck 0.5.0",
  "iai",
@@ -2690,15 +2618,15 @@
  "serde_json",
  "ustr",
  "uuid",
 ]
 
 [[package]]
 name = "nautilus-execution"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "criterion",
  "derive_builder",
  "indexmap 2.2.6",
  "log",
  "nautilus-common",
@@ -2715,27 +2643,27 @@
  "thiserror",
  "tracing",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-indicators"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
  "rstest",
  "strum",
 ]
 
 [[package]]
 name = "nautilus-infrastructure"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "log",
  "nautilus-common",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
@@ -2750,15 +2678,15 @@
  "tokio",
  "tracing",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-model"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "chrono",
  "criterion",
  "derive_builder",
  "evalexpr",
@@ -2778,40 +2706,40 @@
  "thiserror",
  "thousands",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-network"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "axum",
  "criterion",
  "dashmap",
  "futures",
  "futures-util",
- "http 1.1.0",
- "hyper 1.3.1",
+ "http",
+ "hyper",
  "nautilus-core",
  "nonzero_ext",
  "pyo3",
  "pyo3-asyncio",
- "reqwest 0.12.4",
+ "reqwest",
  "rstest",
  "serde_json",
  "tokio",
  "tokio-tungstenite",
  "tracing",
  "tracing-test",
 ]
 
 [[package]]
 name = "nautilus-persistence"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "anyhow",
  "binary-heap-plus",
  "compare",
  "criterion",
  "datafusion",
  "dotenv",
@@ -2826,15 +2754,15 @@
  "rstest",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "nautilus-pyo3"
-version = "0.22.0"
+version = "0.23.0"
 dependencies = [
  "nautilus-accounting",
  "nautilus-adapters",
  "nautilus-common",
  "nautilus-core",
  "nautilus-indicators",
  "nautilus-infrastructure",
@@ -3000,15 +2928,15 @@
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "num_threads"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c7398b9c8b70908f6371f47ed36737907c87c52af34c268fed0bf0ceb92ead9"
@@ -3077,28 +3005,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "300.2.3+3.2.1"
+version = "300.3.0+3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
+checksum = "eba8804a1c5765b18c4b3f907e6897ebabeedebc9830e1a0046c4a4cf44663e1"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
 version = "0.9.102"
@@ -3293,15 +3221,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -3337,36 +3265,36 @@
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plotters"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+checksum = "a15b6eccb8484002195a3e44fe65a4ce8e93a625797a063735536fd59cb01cf3"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+checksum = "414cec62c6634ae900ea1c56128dfe87cf63e7caece0852ec76aba307cebadb7"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+checksum = "81b30686a7d9c3e010b84284bdd26a29f2138574f52f5eb6f794fc0ad924e705"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -3426,17 +3354,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "procfs"
 version = "0.16.0"
@@ -3552,28 +3480,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quickcheck"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "588f6378e4dd99458b60ec275b4477add41ce4fa9f64dcba6f15adccb19b50d6"
@@ -3672,15 +3600,15 @@
  "futures",
  "futures-util",
  "itoa",
  "percent-encoding",
  "pin-project-lite",
  "rustls",
  "rustls-native-certs",
- "rustls-pemfile 2.1.2",
+ "rustls-pemfile",
  "rustls-pki-types",
  "ryu",
  "sha1_smol",
  "socket2",
  "tokio",
  "tokio-retry",
  "tokio-rustls",
@@ -3764,94 +3692,54 @@
 checksum = "71fe3824f5629716b1589be05dacd749f6aa084c87e00e016714a8cdfccc997c"
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.27"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
-dependencies = [
- "base64 0.21.7",
- "bytes",
- "encoding_rs",
- "futures-core",
- "futures-util",
- "h2 0.3.26",
- "http 0.2.12",
- "http-body 0.4.6",
- "hyper 0.14.28",
- "hyper-tls 0.5.0",
- "ipnet",
- "js-sys",
- "log",
- "mime",
- "native-tls",
- "once_cell",
- "percent-encoding",
- "pin-project-lite",
- "rustls-pemfile 1.0.4",
- "serde",
- "serde_json",
- "serde_urlencoded",
- "sync_wrapper 0.1.2",
- "system-configuration",
- "tokio",
- "tokio-native-tls",
- "tokio-util",
- "tower-service",
- "url",
- "wasm-bindgen",
- "wasm-bindgen-futures",
- "wasm-streams",
- "web-sys",
- "winreg 0.50.0",
-]
-
-[[package]]
-name = "reqwest"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "base64 0.22.1",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
- "h2 0.4.5",
- "http 1.1.0",
- "http-body 1.0.0",
+ "h2",
+ "http",
+ "http-body",
  "http-body-util",
- "hyper 1.3.1",
- "hyper-tls 0.6.0",
+ "hyper",
+ "hyper-tls",
  "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls-pemfile 2.1.2",
+ "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper 0.1.2",
  "system-configuration",
  "tokio",
  "tokio-native-tls",
+ "tokio-util",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
+ "wasm-streams",
  "web-sys",
- "winreg 0.52.0",
+ "winreg",
 ]
 
 [[package]]
 name = "ring"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
@@ -3957,15 +3845,15 @@
  "cfg-if",
  "glob",
  "proc-macro2",
  "quote",
  "regex",
  "relative-path",
  "rustc_version",
- "syn 2.0.64",
+ "syn 2.0.66",
  "unicode-ident",
 ]
 
 [[package]]
 name = "rust_decimal"
 version = "1.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4036,31 +3924,22 @@
 [[package]]
 name = "rustls-native-certs"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f1fb85efa936c42c6d5fc28d2629bb51e4b2f4b8a5211e297d599cc5a093792"
 dependencies = [
  "openssl-probe",
- "rustls-pemfile 2.1.2",
+ "rustls-pemfile",
  "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
-dependencies = [
- "base64 0.21.7",
-]
-
-[[package]]
-name = "rustls-pemfile"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
  "base64 0.22.1",
  "rustls-pki-types",
 ]
@@ -4187,15 +4066,15 @@
 name = "serde_derive"
 version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
@@ -4245,15 +4124,15 @@
 name = "serial_test_derive"
 version = "3.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82fe9db325bcef1fbcde82e078a5cc4efdf787e96b3b9cf45b50b529f2083d67"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sha1"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
@@ -4435,15 +4314,15 @@
 name = "sqlparser_derive"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01b2e185515564f15375f593fb966b5718bc624ba77fe49fa4616ad619690554"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sqlx"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c9a2ccff1a000a5a59cd33da541d9f2fdcd9e6e8229cc200565942bff36d0aaa"
@@ -4639,20 +4518,14 @@
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
-name = "streaming-iterator"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2231b7c3057d5e4ad0156fb3dc807d900806020c5ffa3ee6ff2c8c76fb8520"
-
-[[package]]
 name = "stringprep"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb41d74e231a107a1b4ee36bd1214b11285b77768d2e3824aedafa988fd36ee6"
 dependencies = [
  "finl_unicode",
  "unicode-bidi",
@@ -4686,15 +4559,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -4708,17 +4581,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.64"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ad3dee41f36859875573074334c200d1add8e4a87bb37113ebd31d926b7b11f"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -4726,15 +4599,15 @@
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1329189c02ff984e9736652b1631330da25eaa6bc639089ed4915d25446cbe7b"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
@@ -4857,15 +4730,15 @@
 name = "thiserror-impl"
 version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "thousands"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3bf63baf9f5039dadc247375c29eb13706706cfde997d0330d05aa63a77d8820"
@@ -4981,15 +4854,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -5131,15 +5004,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -5211,15 +5084,15 @@
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ef1a641ea34f399a848dea702823bbecfb4c486f911735368f1f137cb8257e1"
 dependencies = [
  "byteorder",
  "bytes",
  "data-encoding",
- "http 1.1.0",
+ "http",
  "httparse",
  "log",
  "native-tls",
  "rand",
  "rustls",
  "rustls-pki-types",
  "sha1",
@@ -5251,15 +5124,15 @@
 name = "typed-builder-macro"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f718dfaf347dcb5b983bfc87608144b0bad87970aebcbea5ce44d2a30c08e63"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
@@ -5438,15 +5311,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5472,15 +5345,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -5725,24 +5598,14 @@
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
-version = "0.50.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
-dependencies = [
- "cfg-if",
- "windows-sys 0.48.0",
-]
-
-[[package]]
-name = "winreg"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
@@ -5784,15 +5647,15 @@
 name = "zerocopy-derive"
 version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     "persistence",
     "pyo3",
     "cli"
 ]
 
 [workspace.package]
 rust-version = "1.78.0"
-version = "0.22.0"
+version = "0.23.0"
 edition = "2021"
 authors = ["Nautech Systems <info@nautechsystems.io>"]
 description = "A high-performance algorithmic trading platform and event-driven backtester"
 documentation = "https://docs.nautilustrader.io"
 
 [workspace.dependencies]
-anyhow = "1.0.84"
+anyhow = "1.0.86"
 chrono = "0.4.38"
 derive_builder = "0.20.0"
 futures = "0.3.30"
 indexmap = { version = "2.2.6", features = ["serde"] }
 itertools = "0.12.1"
 itoa = "1.0.11"
 once_cell = "1.19.0"
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/LICENSE` & `nautilus_trader-1.193.0/nautilus_core/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/README.md` & `nautilus_trader-1.193.0/nautilus_core/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/accounting/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/account/base.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/base.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/account/cash.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/cash.rs`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,17 @@
             Some(StrategyId::new("S-001").unwrap()),
             None,
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("0.8")),
             None,
             None,
             None,
-        );
+            Some(AccountId::from("SIM-001")),
+        )
+        .unwrap();
         let position = Position::new(audusd_sim, fill).unwrap();
         let pnls = cash_account_million_usd
             .calculate_pnls(audusd_sim.into_any(), fill, Some(position))
             .unwrap();
         assert_eq!(pnls, vec![Money::from("-800000 USD")]);
     }
 
@@ -492,15 +494,17 @@
             Some(StrategyId::new("S-001").unwrap()),
             None,
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("45500.00")),
             None,
             None,
             None,
-        );
+            Some(AccountId::from("SIM-001")),
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill1).unwrap();
         let result1 = cash_account_multi
             .calculate_pnls(
                 currency_pair_btcusdt.into_any(),
                 fill1,
                 Some(position.clone()),
             )
@@ -522,15 +526,17 @@
             Some(StrategyId::new("S-001").unwrap()),
             None,
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("45500.00")),
             None,
             None,
             None,
-        );
+            Some(AccountId::from("SIM-001")),
+        )
+        .unwrap();
         let result2 = cash_account_multi
             .calculate_pnls(currency_pair_btcusdt.into_any(), fill2, Some(position))
             .unwrap();
         // use hash set to ignore order of results
         let result1_set: HashSet<Money> = result1.into_iter().collect();
         let result1_expected: HashSet<Money> =
             vec![Money::from("22750 USDT"), Money::from("-0.5 BTC")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/account/margin.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/margin.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/account/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/account/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/python/cash.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/cash.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/python/margin.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/margin.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/python/transformer.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/transformer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/accounting/src/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/accounting/src/stubs.rs`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         None,
         None,
         None,
         Some(Price::from("1.0002")),
         None,
         None,
         None,
-    );
+        None,
+    )
+    .unwrap();
     Position::new(audusd_sim, order_filled).unwrap()
 }
 
 #[fixture]
 pub fn test_position_short(mut order_factory: OrderFactory, audusd_sim: CurrencyPair) -> Position {
     let order = order_factory.market(
         InstrumentId::from("AUD/USD.SIM"),
@@ -70,10 +72,12 @@
         None,
         None,
         None,
         Some(Price::from("22000.0")),
         None,
         None,
         None,
-    );
+        None,
+    )
+    .unwrap();
     Position::new(audusd_sim, order_filled).unwrap()
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/adapters/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 tracing = { workspace = true }
 serde = { workspace = true }
 serde_json = { workspace = true }
 strum = { workspace = true }
 tokio = { workspace = true }
 thiserror = { workspace = true }
 ustr = { workspace = true }
-databento = { version = "0.9.1", optional = true }
-streaming-iterator = "0.1.9"
+databento = { version = "0.10.0", optional = true }
+fallible-streaming-iterator = "0.1.9"
 time = "0.3.36"
 
 [dev-dependencies]
 criterion = { workspace = true }
 rstest = { workspace = true }
 
 [features]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/bin/sandbox.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/bin/sandbox.rs`

 * *Files 8% similar despite different names*

```diff
@@ -36,13 +36,15 @@
     while let Some(record) = client.next_record().await.unwrap() {
         if let Some(msg) = record.get::<TradeMsg>() {
             println!("{msg:#?}");
         }
         if let Some(msg) = record.get::<MboMsg>() {
             println!(
                 "Received delta: {} {} flags={}",
-                count, msg.hd.ts_event, msg.flags,
+                count,
+                msg.hd.ts_event,
+                msg.flags.raw(),
             );
             count += 1;
         }
     }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/common.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/common.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/decode.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/decode.rs`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         msg.order_id,
     );
 
     let delta = OrderBookDelta::new(
         instrument_id,
         parse_book_action(msg.action)?,
         order,
-        msg.flags,
+        msg.flags.raw(),
         msg.sequence.into(),
         msg.ts_recv.into(),
         ts_init,
     );
 
     Ok((Some(delta), None))
 }
@@ -546,15 +546,15 @@
 
     let depth = OrderBookDepth10::new(
         instrument_id,
         bids,
         asks,
         bid_counts,
         ask_counts,
-        msg.flags,
+        msg.flags.raw(),
         msg.sequence.into(),
         msg.ts_recv.into(),
         ts_init,
     );
 
     Ok(depth)
 }
@@ -1020,29 +1020,29 @@
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use std::path::PathBuf;
 
     use databento::dbn::decode::{dbn::Decoder, DecodeStream};
+    use fallible_streaming_iterator::FallibleStreamingIterator;
     use rstest::*;
-    use streaming_iterator::StreamingIterator;
 
     use super::*;
 
     pub const TEST_DATA_PATH: &str =
         concat!(env!("CARGO_MANIFEST_DIR"), "/src/databento/test_data");
 
     #[rstest]
     fn test_decode_mbo_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.mbo.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::MboMsg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let (delta, _) = decode_mbo_msg(msg, instrument_id, 2, 0.into(), false).unwrap();
         let delta = delta.unwrap();
 
         assert_eq!(delta.instrument_id, instrument_id);
         assert_eq!(delta.action, BookAction::Delete);
@@ -1059,15 +1059,15 @@
 
     #[rstest]
     fn test_decode_mbp1_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.mbp-1.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::Mbp1Msg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let (quote, _) = decode_mbp1_msg(msg, instrument_id, 2, 0.into(), false).unwrap();
 
         assert_eq!(quote.instrument_id, instrument_id);
         assert_eq!(quote.bid_price, Price::from("3720.25"));
         assert_eq!(quote.ask_price, Price::from("3720.50"));
@@ -1080,15 +1080,15 @@
 
     #[rstest]
     fn test_decode_mbp10_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.mbp-10.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::Mbp10Msg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let depth10 = decode_mbp10_msg(msg, instrument_id, 2, 0.into()).unwrap();
 
         assert_eq!(depth10.instrument_id, instrument_id);
         assert_eq!(depth10.bids.len(), 10);
         assert_eq!(depth10.asks.len(), 10);
@@ -1103,15 +1103,15 @@
 
     #[rstest]
     fn test_decode_trade_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.trades.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::TradeMsg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let trade = decode_trade_msg(msg, instrument_id, 2, 0.into()).unwrap();
 
         assert_eq!(trade.instrument_id, instrument_id);
         assert_eq!(trade.price, Price::from("3720.25"));
         assert_eq!(trade.size, Quantity::from("5"));
@@ -1124,15 +1124,15 @@
 
     #[rstest]
     fn test_decode_tbbo_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.tbbo.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::Mbp1Msg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let (quote, trade) = decode_tbbo_msg(msg, instrument_id, 2, 0.into()).unwrap();
 
         assert_eq!(quote.instrument_id, instrument_id);
         assert_eq!(quote.bid_price, Price::from("3720.25"));
         assert_eq!(quote.ask_price, Price::from("3720.50"));
@@ -1154,15 +1154,15 @@
 
     #[rstest]
     fn test_decode_ohlcv_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.ohlcv-1s.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::OhlcvMsg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let bar = decode_ohlcv_msg(msg, instrument_id, 2, 0.into()).unwrap();
 
         assert_eq!(
             bar.bar_type,
             BarType::from("ESM4.GLBX-1-SECOND-LAST-EXTERNAL")
@@ -1177,43 +1177,43 @@
 
     #[rstest]
     fn test_decode_definition_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.definition.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::InstrumentDefMsg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let result = decode_instrument_def_msg(msg, instrument_id, 0.into());
 
         assert!(result.is_ok());
     }
 
     #[rstest]
     fn test_decode_definition_v1_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.definition.v1.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::compat::InstrumentDefMsgV1>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let result = decode_instrument_def_msg_v1(msg, instrument_id, 0.into());
 
         assert!(result.is_ok());
     }
 
     #[rstest]
     fn test_decode_imbalance_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.imbalance.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::ImbalanceMsg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let imbalance = decode_imbalance_msg(msg, instrument_id, 2, 0.into()).unwrap();
 
         assert_eq!(imbalance.instrument_id, instrument_id);
         assert_eq!(imbalance.ref_price, Price::from("229.43"));
         assert_eq!(imbalance.cont_book_clr_price, Price::from("0.00"));
@@ -1229,15 +1229,15 @@
 
     #[rstest]
     fn test_decode_statistics_msg() {
         let path = PathBuf::from(format!("{TEST_DATA_PATH}/test_data.statistics.dbn.zst"));
         let mut dbn_stream = Decoder::from_zstd_file(path)
             .unwrap()
             .decode_stream::<dbn::StatMsg>();
-        let msg = dbn_stream.next().unwrap();
+        let msg = dbn_stream.next().unwrap().unwrap();
 
         let instrument_id = InstrumentId::from("ESM4.GLBX");
         let statistics = decode_statistics_msg(msg, instrument_id, 2, 0.into()).unwrap();
 
         assert_eq!(statistics.instrument_id, instrument_id);
         assert_eq!(statistics.stat_type, DatabentoStatisticType::LowestOffer);
         assert_eq!(
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/live.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/live.rs`

 * *Files 1% similar despite different names*

```diff
@@ -258,24 +258,24 @@
                         // TODO: Temporary for debugging
                         deltas_count += 1;
                         trace!(
                             "Buffering delta: {} {} {:?} flags={}",
                             deltas_count,
                             delta.ts_event,
                             buffering_start,
-                            msg.flags,
+                            msg.flags.raw(),
                         );
 
                         // Check if last message in the packet
-                        if !RecordFlag::F_LAST.matches(msg.flags) {
+                        if !RecordFlag::F_LAST.matches(msg.flags.raw()) {
                             continue; // NOT last message
                         }
 
                         // Check if snapshot
-                        if RecordFlag::F_SNAPSHOT.matches(msg.flags) {
+                        if RecordFlag::F_SNAPSHOT.matches(msg.flags.raw()) {
                             continue; // Buffer snapshot
                         }
 
                         // Check if buffering a replay
                         if let Some(start_ns) = buffering_start {
                             if delta.ts_event <= start_ns {
                                 continue; // Continue buffering replay
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/loader.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/loader.rs`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 use std::{env, fs, path::PathBuf};
 
 use databento::dbn;
 use dbn::{
     compat::InstrumentDefMsgV1,
     decode::{dbn::Decoder, DbnMetadata, DecodeStream},
 };
+use fallible_streaming_iterator::FallibleStreamingIterator;
 use indexmap::IndexMap;
 use nautilus_model::{
     data::Data,
     identifiers::{instrument_id::InstrumentId, symbol::Symbol, venue::Venue},
     instruments::any::InstrumentAny,
     types::currency::Currency,
 };
-use streaming_iterator::StreamingIterator;
 use ustr::Ustr;
 
 use super::{
     decode::{
         decode_imbalance_msg, decode_instrument_def_msg_v1, decode_record, decode_statistics_msg,
         raw_ptr_to_ustr,
     },
@@ -149,16 +149,17 @@
         path: PathBuf,
     ) -> anyhow::Result<impl Iterator<Item = anyhow::Result<InstrumentAny>> + '_> {
         let mut decoder = Decoder::from_zstd_file(path)?;
         decoder.set_upgrade_policy(dbn::VersionUpgradePolicy::Upgrade);
         let mut dbn_stream = decoder.decode_stream::<InstrumentDefMsgV1>();
 
         Ok(std::iter::from_fn(move || {
-            dbn_stream.advance();
-
+            if let Err(e) = dbn_stream.advance() {
+                return Some(Err(e.into()));
+            }
             match dbn_stream.get() {
                 Some(rec) => {
                     let record = dbn::RecordRef::from(rec);
                     let msg = record.get::<InstrumentDefMsgV1>().unwrap();
 
                     let raw_symbol = unsafe {
                         raw_ptr_to_ustr(rec.raw_symbol.as_ptr())
@@ -194,15 +195,17 @@
         let decoder = Decoder::from_zstd_file(path)?;
         let metadata = decoder.metadata().clone();
         let mut dbn_stream = decoder.decode_stream::<T>();
 
         let price_precision = Currency::USD().precision; // Hard coded for now
 
         Ok(std::iter::from_fn(move || {
-            dbn_stream.advance();
+            if let Err(e) = dbn_stream.advance() {
+                return Some(Err(e.into()));
+            }
             match dbn_stream.get() {
                 Some(rec) => {
                     let record = dbn::RecordRef::from(rec);
                     let instrument_id = match &instrument_id {
                         Some(id) => *id, // Copy
                         None => decode_nautilus_instrument_id(
                             &record,
@@ -239,15 +242,17 @@
         let decoder = Decoder::from_zstd_file(path)?;
         let metadata = decoder.metadata().clone();
         let mut dbn_stream = decoder.decode_stream::<T>();
 
         let price_precision = Currency::USD().precision; // Hard coded for now
 
         Ok(std::iter::from_fn(move || {
-            dbn_stream.advance();
+            if let Err(e) = dbn_stream.advance() {
+                return Some(Err(e.into()));
+            }
             match dbn_stream.get() {
                 Some(rec) => {
                     let record = dbn::RecordRef::from(rec);
                     let instrument_id = match &instrument_id {
                         Some(id) => *id, // Copy
                         None => decode_nautilus_instrument_id(
                             &record,
@@ -286,15 +291,17 @@
         let decoder = Decoder::from_zstd_file(path)?;
         let metadata = decoder.metadata().clone();
         let mut dbn_stream = decoder.decode_stream::<T>();
 
         let price_precision = Currency::USD().precision; // Hard coded for now
 
         Ok(std::iter::from_fn(move || {
-            dbn_stream.advance();
+            if let Err(e) = dbn_stream.advance() {
+                return Some(Err(e.into()));
+            }
             match dbn_stream.get() {
                 Some(rec) => {
                     let record = dbn::RecordRef::from(rec);
                     let instrument_id = match &instrument_id {
                         Some(id) => *id, // Copy
                         None => decode_nautilus_instrument_id(
                             &record,
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/publishers.json` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/publishers.json`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/historical.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/historical.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/live.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/live.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/loader.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/loader.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/python/types.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/types.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/symbology.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/symbology.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/databento/types.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/types.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/adapters/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/adapters/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/backtest/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/backtest/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/backtest/build.rs` & `nautilus_trader-1.193.0/nautilus_core/backtest/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/backtest/cbindgen_cython.toml` & `nautilus_trader-1.193.0/nautilus_core/backtest/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/backtest/src/engine.rs` & `nautilus_trader-1.193.0/nautilus_core/backtest/src/engine.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/backtest/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/backtest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/backtest/src/matching_engine.rs` & `nautilus_trader-1.193.0/nautilus_core/backtest/src/matching_engine.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/cli/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/cli/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/cli/src/bin/cli.rs` & `nautilus_trader-1.193.0/nautilus_core/cli/src/bin/cli.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/cli/src/database/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/cli/src/database/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/cli/src/database/postgres.rs` & `nautilus_trader-1.193.0/nautilus_core/cli/src/database/postgres.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/cli/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/cli/src/opt.rs` & `nautilus_trader-1.193.0/nautilus_core/cli/src/opt.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/build.rs` & `nautilus_trader-1.193.0/nautilus_core/common/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/cbindgen.toml` & `nautilus_trader-1.193.0/nautilus_core/common/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/cbindgen_cython.toml` & `nautilus_trader-1.193.0/nautilus_core/common/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/cache/core.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/cache/core.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/cache/database.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/cache/database.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/cache/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/clock.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/factories.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/factories.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/ffi/clock.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/ffi/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/ffi/logging.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/logging.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/ffi/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/ffi/timer.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/timer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/generators/client_order_id.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/generators/client_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/generators/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/generators/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/generators/order_list_id.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/generators/order_list_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/generators/position_id.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/generators/position_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/handlers.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/handlers.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/interface/account.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/interface/account.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/interface/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/interface/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/logging/headers.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/logging/headers.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/logging/logger.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/logging/logger.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/logging/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/logging/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/logging/writer.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/logging/writer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/msgbus/core.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/core.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/msgbus/database.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/database.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/msgbus/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/python/clock.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/python/clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/python/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/python/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/python/logging.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/python/logging.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/python/timer.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/python/timer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/python/versioning.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/python/versioning.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/runtime.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/testing.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/testing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/timer.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/timer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/common/src/xrate.rs` & `nautilus_trader-1.193.0/nautilus_core/common/src/xrate.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/build.rs` & `nautilus_trader-1.193.0/nautilus_core/core/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/cbindgen.toml` & `nautilus_trader-1.193.0/nautilus_core/core/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/cbindgen_cython.toml` & `nautilus_trader-1.193.0/nautilus_core/core/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/correctness.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/correctness.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/datetime.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/datetime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/deserialization.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/deserialization.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/equality.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/equality.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/ffi/cvec.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/cvec.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/ffi/datetime.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/datetime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/ffi/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/ffi/parsing.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/parsing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/ffi/string.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/string.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/ffi/uuid.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/uuid.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/message.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/message.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/nanos.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/nanos.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/parsing.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/parsing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/python/casing.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/python/casing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/python/datetime.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/python/datetime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/python/serialization.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/python/serialization.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/python/uuid.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/python/uuid.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/serialization.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/serialization.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/time.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/time.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/core/src/uuid.rs` & `nautilus_trader-1.193.0/nautilus_core/core/src/uuid.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/execution/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/client.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/client.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/engine.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/engine.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/matching_core.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/matching_core.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/cancel.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/cancel_all.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_all.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/cancel_batch.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_batch.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/modify.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/modify.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/query.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/query.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/submit.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/execution/src/messages/submit_list.rs` & `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit_list.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/indicators/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/ama.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ama.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/dema.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/dema.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/ema.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ema.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/hma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/hma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/rma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/rma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/sma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/sma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/vidya.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/vidya.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/average/wma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/wma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/book/imbalance.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/book/imbalance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/book/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/book/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/indicator.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/indicator.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/aroon.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/aroon.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/bias.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/bias.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/cmo.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/cmo.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/momentum/rsi.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/rsi.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/ama.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ama.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/dema.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/dema.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/ema.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ema.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/hma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/hma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/rma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/rma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/sma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/sma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/vidya.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/vidya.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/average/wma.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/wma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/book/imbalance.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/imbalance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/book/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/aroon.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/aroon.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/bias.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/bias.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/cmo.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/cmo.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/momentum/rsi.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/rsi.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/ratio/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/volatility/atr.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/atr.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/python/volatility/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/ratio/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/testing.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/testing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/volatility/atr.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/atr.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/indicators/src/volatility/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/redis/cache.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/cache.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/redis/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,21 @@
     #[pyo3(name = "add_order")]
     fn py_add_order(slf: PyRef<'_, Self>, order: PyObject, py: Python<'_>) -> PyResult<()> {
         let order_any = convert_pyobject_to_order_any(py, order)?;
         let result = get_runtime().block_on(async { slf.add_order(order_any).await });
         result.map_err(to_pyruntime_err)
     }
 
+    #[pyo3(name = "update_order")]
+    fn py_update_order(slf: PyRef<'_, Self>, order: PyObject, py: Python<'_>) -> PyResult<()> {
+        let order_any = convert_pyobject_to_order_any(py, order)?;
+        let result = get_runtime().block_on(async { slf.update_order(order_any).await });
+        result.map_err(to_pyruntime_err)
+    }
+
     #[pyo3(name = "load_order")]
     fn py_load_order(
         slf: PyRef<'_, Self>,
         order_id: ClientOrderId,
         py: Python<'_>,
     ) -> PyResult<Option<PyObject>> {
         get_runtime().block_on(async {
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/python/sql/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/redis/cache.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/cache.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/redis/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/redis/msgbus.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/msgbus.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/cache_database.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/cache_database.rs`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 #[allow(clippy::large_enum_variant)]
 #[derive(Debug, Clone)]
 pub enum DatabaseQuery {
     Add(String, Vec<u8>),
     AddCurrency(Currency),
     AddInstrument(InstrumentAny),
-    AddOrder(OrderAny),
+    AddOrder(OrderAny, bool),
 }
 
 fn get_buffer_interval() -> Duration {
     Duration::from_millis(0)
 }
 
 async fn drain_buffer(pool: &PgPool, buffer: &mut VecDeque<DatabaseQuery>) {
@@ -106,60 +106,66 @@
                 }
                 InstrumentAny::OptionsSpread(instrument) => {
                     DatabaseQueries::add_instrument(pool, "OPTIONS_SPREAD", Box::new(instrument))
                         .await
                         .unwrap()
                 }
             },
-            DatabaseQuery::AddOrder(order_any) => match order_any {
+            DatabaseQuery::AddOrder(order_any, updated) => match order_any {
                 OrderAny::Limit(order) => {
-                    DatabaseQueries::add_order(pool, "LIMIT", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "LIMIT", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
                 OrderAny::LimitIfTouched(order) => {
-                    DatabaseQueries::add_order(pool, "LIMIT_IF_TOUCHED", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "LIMIT_IF_TOUCHED", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
                 OrderAny::Market(order) => {
-                    DatabaseQueries::add_order(pool, "MARKET", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "MARKET", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
                 OrderAny::MarketIfTouched(order) => {
-                    DatabaseQueries::add_order(pool, "MARKET_IF_TOUCHED", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "MARKET_IF_TOUCHED", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
                 OrderAny::MarketToLimit(order) => {
-                    DatabaseQueries::add_order(pool, "MARKET_TO_LIMIT", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "MARKET_TO_LIMIT", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
                 OrderAny::StopLimit(order) => {
-                    DatabaseQueries::add_order(pool, "STOP_LIMIT", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "STOP_LIMIT", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
                 OrderAny::StopMarket(order) => {
-                    DatabaseQueries::add_order(pool, "STOP_MARKET", false, Box::new(order))
-                        .await
-                        .unwrap()
-                }
-                OrderAny::TrailingStopLimit(order) => {
-                    DatabaseQueries::add_order(pool, "TRAILING_STOP_LIMIT", false, Box::new(order))
-                        .await
-                        .unwrap()
-                }
-                OrderAny::TrailingStopMarket(order) => {
-                    DatabaseQueries::add_order(pool, "TRAILING_STOP_MARKET", false, Box::new(order))
+                    DatabaseQueries::add_order(pool, "STOP_MARKET", updated, Box::new(order))
                         .await
                         .unwrap()
                 }
+                OrderAny::TrailingStopLimit(order) => DatabaseQueries::add_order(
+                    pool,
+                    "TRAILING_STOP_LIMIT",
+                    updated,
+                    Box::new(order),
+                )
+                .await
+                .unwrap(),
+                OrderAny::TrailingStopMarket(order) => DatabaseQueries::add_order(
+                    pool,
+                    "TRAILING_STOP_MARKET",
+                    updated,
+                    Box::new(order),
+                )
+                .await
+                .unwrap(),
             },
         }
     }
 }
 
 impl PostgresCacheDatabase {
     pub async fn connect(
@@ -264,15 +270,22 @@
     }
 
     pub async fn load_instruments(&self) -> anyhow::Result<Vec<InstrumentAny>> {
         DatabaseQueries::load_instruments(&self.pool).await
     }
 
     pub async fn add_order(&self, order: OrderAny) -> anyhow::Result<()> {
-        let query = DatabaseQuery::AddOrder(order);
+        let query = DatabaseQuery::AddOrder(order, false);
+        self.tx.send(query).await.map_err(|err| {
+            anyhow::anyhow!("Failed to send query add_order to database message handler: {err}")
+        })
+    }
+
+    pub async fn update_order(&self, order: OrderAny) -> anyhow::Result<()> {
+        let query = DatabaseQuery::AddOrder(order, true);
         self.tx.send(query).await.map_err(|err| {
             anyhow::anyhow!("Failed to send query add_order to database message handler: {err}")
         })
     }
 
     pub async fn load_order(
         &self,
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 // Be careful about ordering and foreign key constraints when deleting data.
 pub const NAUTILUS_TABLES: [&str; 5] =
-    ["general", "instrument", "currency", "order_event", "order"];
+    ["general", "instrument", "order_event", "order", "currency"];
 
 pub mod cache_database;
 pub mod models;
 pub mod pg;
 pub mod queries;
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/general.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/general.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/instruments.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/instruments.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/orders.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/orders.rs`

 * *Files 18% similar despite different names*

```diff
@@ -13,29 +13,33 @@
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::{collections::HashMap, str::FromStr};
 
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use nautilus_model::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::{
         accepted::OrderAccepted, cancel_rejected::OrderCancelRejected, canceled::OrderCanceled,
         denied::OrderDenied, emulated::OrderEmulated, event::OrderEventAny, expired::OrderExpired,
         filled::OrderFilled, initialized::OrderInitialized, modify_rejected::OrderModifyRejected,
         pending_cancel::OrderPendingCancel, pending_update::OrderPendingUpdate,
         rejected::OrderRejected, released::OrderReleased, submitted::OrderSubmitted,
         triggered::OrderTriggered, updated::OrderUpdated,
     },
     identifiers::{
-        client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId,
+        account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 use sqlx::{postgres::PgRow, FromRow, Row};
 use ustr::Ustr;
 
 pub struct OrderEventAnyModel(pub OrderEventAny);
 pub struct OrderAcceptedModel(pub OrderAccepted);
 pub struct OrderCancelRejectedModel(pub OrderCancelRejected);
@@ -112,15 +116,15 @@
             )
         }
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderInitializedModel {
     fn from_row(row: &'r PgRow) -> Result<Self, sqlx::Error> {
-        let order_id = row.try_get::<&str, _>("id").map(UUID4::from)?;
+        let event_id = row.try_get::<&str, _>("id").map(UUID4::from)?;
         let client_order_id = row
             .try_get::<&str, _>("order_id")
             .map(ClientOrderId::from)?;
         let trader_id = row.try_get::<&str, _>("trader_id").map(TraderId::from)?;
         let strategy_id = row
             .try_get::<&str, _>("strategy_id")
             .map(StrategyId::from)?;
@@ -221,28 +225,28 @@
             .ok()
             .and_then(|x| x.map(ClientOrderId::from));
         let tags: Option<Vec<Ustr>> = row
             .try_get::<Option<serde_json::Value>, _>("tags")
             .ok()
             .and_then(|x| x.map(|x| serde_json::from_value::<Vec<String>>(x).unwrap()))
             .map(|x| x.into_iter().map(|x| Ustr::from(x.as_str())).collect());
-        let order = OrderInitialized::new(
+        let order_event = OrderInitialized::new(
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
             order_side,
             order_type,
             quantity,
             time_in_force,
             post_only,
             reduce_only,
             quote_quantity,
             reconciliation,
-            order_id,
+            event_id,
             ts_event,
             ts_init,
             price,
             trigger_price,
             trigger_type,
             limit_offset,
             trailing_offset,
@@ -257,21 +261,51 @@
             parent_order_id,
             exec_algorithm_id,
             exec_algorithm_params,
             exec_spawn_id,
             tags,
         )
         .unwrap();
-        Ok(OrderInitializedModel(order))
+        Ok(OrderInitializedModel(order_event))
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderAcceptedModel {
-    fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
-        todo!()
+    fn from_row(row: &'r PgRow) -> Result<Self, sqlx::Error> {
+        let event_id = row.try_get::<&str, _>("id").map(UUID4::from)?;
+        let trader_id = row.try_get::<&str, _>("trader_id").map(TraderId::from)?;
+        let strategy_id = row
+            .try_get::<&str, _>("strategy_id")
+            .map(StrategyId::from)?;
+        let instrument_id = row
+            .try_get::<&str, _>("instrument_id")
+            .map(InstrumentId::from)?;
+        let order_id = row
+            .try_get::<&str, _>("order_id")
+            .map(ClientOrderId::from)?;
+        let venue_order_id = row
+            .try_get::<&str, _>("venue_order_id")
+            .map(VenueOrderId::from)?;
+        let account_id = row.try_get::<&str, _>("account_id").map(AccountId::from)?;
+        let ts_event = row.try_get::<&str, _>("ts_event").map(UnixNanos::from)?;
+        let ts_init = row.try_get::<&str, _>("ts_init").map(UnixNanos::from)?;
+        let order_event = OrderAccepted::new(
+            trader_id,
+            strategy_id,
+            instrument_id,
+            order_id,
+            venue_order_id,
+            account_id,
+            event_id,
+            ts_event,
+            ts_init,
+            false,
+        )
+        .unwrap();
+        Ok(OrderAcceptedModel(order_event))
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderCancelRejectedModel {
     fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
         todo!()
     }
@@ -298,16 +332,76 @@
 impl<'r> FromRow<'r, PgRow> for OrderExpiredModel {
     fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
         todo!()
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderFilledModel {
-    fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
-        todo!()
+    fn from_row(row: &'r PgRow) -> Result<Self, sqlx::Error> {
+        let event_id = row.try_get::<&str, _>("id").map(UUID4::from)?;
+        let trader_id = row.try_get::<&str, _>("trader_id").map(TraderId::from)?;
+        let strategy_id = row
+            .try_get::<&str, _>("strategy_id")
+            .map(StrategyId::from)?;
+        let instrument_id = row
+            .try_get::<&str, _>("instrument_id")
+            .map(InstrumentId::from)?;
+        let order_id = row
+            .try_get::<&str, _>("order_id")
+            .map(ClientOrderId::from)?;
+        let venue_order_id = row
+            .try_get::<&str, _>("venue_order_id")
+            .map(VenueOrderId::from)?;
+        let account_id = row.try_get::<&str, _>("account_id").map(AccountId::from)?;
+        let trade_id = row.try_get::<&str, _>("trade_id").map(TradeId::from)?;
+        let order_side = row
+            .try_get::<&str, _>("order_side")
+            .map(|x| OrderSide::from_str(x).unwrap())?;
+        let order_type = row
+            .try_get::<&str, _>("order_type")
+            .map(|x| OrderType::from_str(x).unwrap())?;
+        let last_px = row.try_get::<&str, _>("last_px").map(Price::from)?;
+        let last_qty = row.try_get::<&str, _>("last_qty").map(Quantity::from)?;
+        let currency = row.try_get::<&str, _>("currency").map(Currency::from)?;
+        let test = row.try_get::<&str, _>("liquidity_side").unwrap();
+        println!("test: {:?}", test);
+        let liquidity_side = row
+            .try_get::<&str, _>("liquidity_side")
+            .map(|x| LiquiditySide::from_str(x).unwrap())?;
+        let ts_event = row.try_get::<&str, _>("ts_event").map(UnixNanos::from)?;
+        let ts_init = row.try_get::<&str, _>("ts_init").map(UnixNanos::from)?;
+        let position_id = row
+            .try_get::<Option<&str>, _>("position_id")
+            .map(|x| x.map(PositionId::from))?;
+        let commission = row
+            .try_get::<Option<&str>, _>("commission")
+            .map(|x| x.map(|x| Money::from_str(x).unwrap()))?;
+        let order_event = OrderFilled::new(
+            trader_id,
+            strategy_id,
+            instrument_id,
+            order_id,
+            venue_order_id,
+            account_id,
+            trade_id,
+            order_side,
+            order_type,
+            last_qty,
+            last_px,
+            currency,
+            liquidity_side,
+            event_id,
+            ts_event,
+            ts_init,
+            false,
+            position_id,
+            commission,
+        )
+        .unwrap();
+        Ok(OrderFilledModel(order_event))
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderModifyRejectedModel {
     fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
         todo!()
     }
@@ -334,16 +428,45 @@
 impl<'r> FromRow<'r, PgRow> for OrderReleasedModel {
     fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
         todo!()
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderSubmittedModel {
-    fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
-        todo!()
+    fn from_row(row: &'r PgRow) -> Result<Self, sqlx::Error> {
+        let trader_id = row.try_get::<&str, _>("trader_id").map(TraderId::from)?;
+        let strategy_id = row
+            .try_get::<&str, _>("strategy_id")
+            .map(StrategyId::from)?;
+        let instrument_id = row
+            .try_get::<&str, _>("instrument_id")
+            .map(InstrumentId::from)?;
+        let client_order_id = row
+            .try_get::<&str, _>("order_id")
+            .map(ClientOrderId::from)?;
+        let account_id = row.try_get::<&str, _>("account_id").map(AccountId::from)?;
+        let event_id = row.try_get::<&str, _>("id").map(UUID4::from)?;
+        let ts_event = row
+            .try_get::<String, _>("ts_event")
+            .map(|res| UnixNanos::from(res.as_str()))?;
+        let ts_init = row
+            .try_get::<String, _>("ts_init")
+            .map(|res| UnixNanos::from(res.as_str()))?;
+        let order_event = OrderSubmitted::new(
+            trader_id,
+            strategy_id,
+            instrument_id,
+            client_order_id,
+            account_id,
+            event_id,
+            ts_event,
+            ts_init,
+        )
+        .unwrap();
+        Ok(OrderSubmittedModel(order_event))
     }
 }
 
 impl<'r> FromRow<'r, PgRow> for OrderTriggeredModel {
     fn from_row(_row: &'r PgRow) -> Result<Self, sqlx::Error> {
         todo!()
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/models/types.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/types.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/pg.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/pg.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/src/sql/queries.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/queries.rs`

 * *Files 2% similar despite different names*

```diff
@@ -266,47 +266,55 @@
 
     pub async fn add_order_event(
         pool: &PgPool,
         order_event: Box<dyn OrderEvent>,
     ) -> anyhow::Result<()> {
         sqlx::query(r#"
             INSERT INTO "order_event" (
-                id, kind, order_id, order_type, order_side, trader_id, strategy_id, instrument_id, quantity, time_in_force,
-                post_only, reduce_only, quote_quantity, reconciliation, price, trigger_price, trigger_type, limit_offset, trailing_offset,
+                id, kind, order_id, order_type, order_side, trader_id, strategy_id, instrument_id, trade_id, currency, quantity, time_in_force, liquidity_side,
+                post_only, reduce_only, quote_quantity, reconciliation, price, last_px, last_qty, trigger_price, trigger_type, limit_offset, trailing_offset,
                 trailing_offset_type, expire_time, display_qty, emulation_trigger, trigger_instrument_id, contingency_type,
                 order_list_id, linked_order_ids, parent_order_id,
-                exec_algorithm_id, exec_spawn_id, venue_order_id, account_id, ts_event, ts_init, created_at, updated_at
+                exec_algorithm_id, exec_spawn_id, venue_order_id, account_id, position_id, commission, ts_event, ts_init, created_at, updated_at
             ) VALUES (
                 $1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13, $14, $15, $16, $17, $18, $19, $20,
-                $21, $22, $23, $24, $25, $26, $27, $28, $29, $30, $31, $32, $33, $34, CURRENT_TIMESTAMP, CURRENT_TIMESTAMP
+                $21, $22, $23, $24, $25, $26, $27, $28, $29, $30, $31, $32, $33, $34, $35, $36, $37, $38, $39, $40, $41, CURRENT_TIMESTAMP, CURRENT_TIMESTAMP
             )
             ON CONFLICT (id)
             DO UPDATE
             SET
-                kind = $2, order_id = $3, order_type = $4, order_side=$5, trader_id = $6, strategy_id = $7, instrument_id = $8, quantity = $9, time_in_force= $10,
-                post_only = $11, reduce_only = $12, quote_quantity = $13, reconciliation = $14, price = $15, trigger_price = $16, trigger_type = $17, limit_offset = $18, trailing_offset = $19,
-                trailing_offset_type = $20, expire_time = $21, display_qty = $22, emulation_trigger = $23, trigger_instrument_id = $24, contingency_type = $25,
-                order_list_id = $26, linked_order_ids = $27,
-                parent_order_id = $28, exec_algorithm_id = $29, exec_spawn_id = $30, venue_order_id = $31, account_id = $32, ts_event = $33, ts_init = $34, updated_at = CURRENT_TIMESTAMP
+                kind = $2, order_id = $3, order_type = $4, order_side=$5, trader_id = $6, strategy_id = $7, instrument_id = $8, trade_id = $9, currency = $10,
+                quantity = $11, time_in_force = $12, liquidity_side = $13,
+                post_only = $14, reduce_only = $15, quote_quantity = $16, reconciliation = $17, price = $18, last_px = $19,
+                last_qty = $20, trigger_price = $21, trigger_type = $22, limit_offset = $23, trailing_offset = $24,
+                trailing_offset_type = $25, expire_time = $26, display_qty = $27, emulation_trigger = $28, trigger_instrument_id = $29,
+                contingency_type = $30, order_list_id = $31, linked_order_ids = $32,
+                parent_order_id = $33, exec_algorithm_id = $34, exec_spawn_id = $35, venue_order_id = $36, account_id = $37, position_id = $38, commission = $39,
+                ts_event = $40, ts_init = $41, updated_at = CURRENT_TIMESTAMP
         "#)
             .bind(order_event.id().to_string())
             .bind(order_event.kind())
             .bind(order_event.client_order_id().to_string())
             .bind(order_event.order_type().map(|x| x.to_string()))
-            .bind(order_event.order_side().map(|x| format!("{:?}", x)))
+            .bind(order_event.order_side().map(|x| x.to_string()))
             .bind(order_event.trader_id().to_string())
             .bind(order_event.strategy_id().to_string())
             .bind(order_event.instrument_id().to_string())
+            .bind(order_event.trade_id().map(|x| x.to_string()))
+            .bind(order_event.currency().map(|x| x.code.as_str()))
             .bind(order_event.quantity().map(|x| x.to_string()))
-            .bind(order_event.time_in_force().map(|x| format!("{:?}", x)))
+            .bind(order_event.time_in_force().map(|x| x.to_string()))
+            .bind(order_event.liquidity_side().map(|x| x.to_string()))
             .bind(order_event.post_only())
             .bind(order_event.reduce_only())
             .bind(order_event.quote_quantity())
             .bind(order_event.reconciliation())
             .bind(order_event.price().map(|x| x.to_string()))
+            .bind(order_event.last_px().map(|x| x.to_string()))
+            .bind(order_event.last_qty().map(|x| x.to_string()))
             .bind(order_event.trigger_price().map(|x| x.to_string()))
             .bind(order_event.trigger_type().map(|x| x.to_string()))
             .bind(order_event.limit_offset().map(|x| x.to_string()))
             .bind(order_event.trailing_offset().map(|x| x.to_string()))
             .bind(order_event.trailing_offset_type().map(|x| format!("{:?}", x)))
             .bind(order_event.expire_time().map(|x| x.to_string()))
             .bind(order_event.display_qty().map(|x| x.to_string()))
@@ -316,31 +324,29 @@
             .bind(order_event.order_list_id().map(|x| x.to_string()))
             .bind(order_event.linked_order_ids().map(|x| x.iter().map(|x| x.to_string()).collect::<Vec<String>>()))
             .bind(order_event.parent_order_id().map(|x| x.to_string()))
             .bind(order_event.exec_algorithm_id().map(|x| x.to_string()))
             .bind(order_event.exec_spawn_id().map(|x| x.to_string()))
             .bind(order_event.venue_order_id().map(|x| x.to_string()))
             .bind(order_event.account_id().map(|x| x.to_string()))
+            .bind(order_event.position_id().map(|x| x.to_string()))
+            .bind(order_event.commission().map(|x| x.to_string()))
             .bind(order_event.ts_event().to_string())
             .bind(order_event.ts_init().to_string())
             .execute(pool)
             .await
             .map(|_| ())
             .map_err(|err| anyhow::anyhow!("Failed to insert into order_event table: {err}"))
     }
 
     pub async fn load_order_events(
         pool: &PgPool,
         order_id: &ClientOrderId,
     ) -> anyhow::Result<Vec<OrderEventAny>> {
-        sqlx::query_as::<_, OrderEventAnyModel>(
-            r#"
-          SELECT * FROM "order_event" event WHERE event.order_id = $1 ORDER BY event.ts_init ASC
-        "#,
-        )
+        sqlx::query_as::<_, OrderEventAnyModel>(r#"SELECT * FROM "order_event" event WHERE event.order_id = $1 ORDER BY created_at ASC"#)
         .bind(order_id.to_string())
         .fetch_all(pool)
         .await
         .map(|rows| rows.into_iter().map(|row| row.0).collect())
         .map_err(|err| anyhow::anyhow!("Failed to load order events: {err}"))
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs` & `nautilus_trader-1.193.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs`

 * *Files 14% similar despite different names*

```diff
@@ -60,24 +60,31 @@
 #[cfg(target_os = "linux")] // Databases only supported on Linux
 mod tests {
     use std::time::Duration;
 
     use nautilus_core::equality::entirely_equal;
     use nautilus_model::{
         enums::{CurrencyType, OrderSide},
-        identifiers::{client_order_id::ClientOrderId, instrument_id::InstrumentId},
+        events::order::event::OrderEventAny,
+        identifiers::{
+            account_id::AccountId, client_order_id::ClientOrderId, instrument_id::InstrumentId,
+            stubs::account_id, trade_id::TradeId, venue_order_id::VenueOrderId,
+        },
         instruments::{
             any::InstrumentAny,
             stubs::{
                 crypto_future_btcusdt, crypto_perpetual_ethusdt, currency_pair_ethusdt,
                 equity_aapl, futures_contract_es, options_contract_appl,
             },
             Instrument,
         },
-        orders::{any::OrderAny, stubs::TestOrderStubs},
+        orders::{
+            any::OrderAny,
+            stubs::{TestOrderEventStubs, TestOrderStubs},
+        },
         types::{currency::Currency, price::Price, quantity::Quantity},
     };
     use serial_test::serial;
 
     use crate::get_pg_cache_database;
 
     #[tokio::test]
@@ -234,29 +241,31 @@
             ]
         );
     }
 
     #[tokio::test]
     #[serial]
     async fn test_add_order() {
+        let client_order_id_1 = ClientOrderId::new("O-19700101-0000-000-001-1").unwrap();
+        let client_order_id_2 = ClientOrderId::new("O-19700101-0000-000-001-2").unwrap();
         let instrument = currency_pair_ethusdt();
         let pg_cache = get_pg_cache_database().await.unwrap();
         let market_order = TestOrderStubs::market_order(
             instrument.id(),
             OrderSide::Buy,
             Quantity::from("1.0"),
-            Some(ClientOrderId::new("O-19700101-0000-000-001-1").unwrap()),
+            Some(client_order_id_1),
             None,
         );
         let limit_order = TestOrderStubs::limit_order(
             instrument.id(),
             OrderSide::Sell,
             Price::from("100.0"),
             Quantity::from("1.0"),
-            Some(ClientOrderId::new("O-19700101-0000-000-001-2").unwrap()),
+            Some(client_order_id_2),
             None,
         );
         pg_cache
             .add_order(OrderAny::Market(market_order.clone()))
             .await
             .unwrap();
         pg_cache
@@ -271,8 +280,82 @@
         let limit_order_result = pg_cache
             .load_order(&limit_order.client_order_id)
             .await
             .unwrap();
         entirely_equal(market_order_result.unwrap(), OrderAny::Market(market_order));
         entirely_equal(limit_order_result.unwrap(), OrderAny::Limit(limit_order));
     }
+
+    #[tokio::test]
+    #[serial]
+    async fn test_update_order_for_open_order() {
+        let client_order_id_1 = ClientOrderId::new("O-19700101-0000-000-002-1").unwrap();
+        let instrument = currency_pair_ethusdt();
+        let account = account_id();
+        let pg_cache = get_pg_cache_database().await.unwrap();
+        // Add the target currency of order
+        pg_cache
+            .add_currency(instrument.quote_currency)
+            .await
+            .unwrap();
+        // 1. create the order
+        let mut market_order = TestOrderStubs::market_order(
+            instrument.id(),
+            OrderSide::Buy,
+            Quantity::from("1.0"),
+            Some(client_order_id_1),
+            None,
+        );
+        pg_cache
+            .add_order(OrderAny::Market(market_order.clone()))
+            .await
+            .unwrap();
+        let submitted_event = TestOrderEventStubs::order_submitted(&market_order, account).unwrap();
+        market_order
+            .apply(OrderEventAny::Submitted(submitted_event))
+            .unwrap();
+        pg_cache
+            .update_order(OrderAny::Market(market_order.clone()))
+            .await
+            .unwrap();
+        let accepted_event = TestOrderEventStubs::order_accepted(
+            &market_order,
+            account,
+            VenueOrderId::new("001").unwrap(),
+        )
+        .unwrap();
+        market_order
+            .apply(OrderEventAny::Accepted(accepted_event))
+            .unwrap();
+        pg_cache
+            .update_order(OrderAny::Market(market_order.clone()))
+            .await
+            .unwrap();
+        let order_filled = TestOrderEventStubs::order_filled(
+            &market_order,
+            &instrument,
+            None,
+            Some(TradeId::new("T-19700101-0000-000-001-1").unwrap()),
+            None,
+            Some(Price::from("100.0")),
+            Some(Quantity::from("1.0")),
+            None,
+            None,
+            Some(AccountId::new("SIM-001").unwrap()),
+        )
+        .unwrap();
+        market_order
+            .apply(OrderEventAny::Filled(order_filled))
+            .unwrap();
+        pg_cache
+            .update_order(OrderAny::Market(market_order.clone()))
+            .await
+            .unwrap();
+        tokio::time::sleep(Duration::from_secs(2)).await;
+        // assert
+        let market_order_result = pg_cache
+            .load_order(&market_order.client_order_id)
+            .await
+            .unwrap();
+        entirely_equal(market_order_result.unwrap(), OrderAny::Market(market_order));
+    }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/model/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/build.rs` & `nautilus_trader-1.193.0/nautilus_core/model/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/cbindgen.toml` & `nautilus_trader-1.193.0/nautilus_core/model/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/cbindgen_cython.toml` & `nautilus_trader-1.193.0/nautilus_core/model/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/currencies.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/currencies.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/bar.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/delta.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/deltas.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/deltas.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/depth.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/order.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/quote.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/data/trade.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/data/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/account/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/account/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/account/state.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/account/state.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/account/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/account/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/accepted.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/accepted.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -140,14 +144,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -156,14 +168,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -176,14 +192,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -244,14 +268,22 @@
         Some(self.venue_order_id)
     }
 
     fn account_id(&self) -> Option<AccountId> {
         Some(self.account_id)
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/cancel_rejected.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/cancel_rejected.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -146,14 +150,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         Some(self.reason)
     }
@@ -162,14 +174,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -182,14 +198,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -250,14 +274,22 @@
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         self.account_id
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        todo!()
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/canceled.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/expired.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,47 +17,51 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
-pub struct OrderCanceled {
+pub struct OrderExpired {
     pub trader_id: TraderId,
     pub strategy_id: StrategyId,
     pub instrument_id: InstrumentId,
     pub client_order_id: ClientOrderId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
     pub account_id: Option<AccountId>,
 }
 
-impl OrderCanceled {
+impl OrderExpired {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         event_id: UUID4,
@@ -78,54 +82,55 @@
             reconciliation: u8::from(reconciliation),
             venue_order_id,
             account_id,
         })
     }
 }
 
-impl Debug for OrderCanceled {
+impl Debug for OrderExpired {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f,
+        write!(
+            f,
             "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
-            stringify!(OrderCanceled),
+            stringify!(OrderExpired),
             self.trader_id,
             self.strategy_id,
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or_else(|| "None".to_string(), |venue_order_id| format!("{venue_order_id}")),
             self.account_id.map_or_else(|| "None".to_string(), |account_id| format!("{account_id}")),
             self.event_id,
             self.ts_event,
             self.ts_init
         )
     }
 }
 
-impl Display for OrderCanceled {
+impl Display for OrderExpired {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
-            stringify!(OrderCanceled),
+            stringify!(OrderExpired),
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
             self.account_id.map_or("None".to_string(), |account_id| format!("{account_id}")),
             self.ts_event
         )
     }
 }
 
-impl OrderEvent for OrderCanceled {
+impl OrderEvent for OrderExpired {
     fn id(&self) -> UUID4 {
         self.event_id
     }
 
     fn kind(&self) -> &str {
-        stringify!(OrderCanceled)
+        stringify!(OrderExpired)
     }
 
     fn order_type(&self) -> Option<OrderType> {
         None
     }
 
     fn order_side(&self) -> Option<OrderSide> {
@@ -140,14 +145,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -156,14 +169,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -176,14 +193,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -244,21 +269,43 @@
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         self.account_id
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
-mod tests {}
+mod tests {
+
+    use rstest::rstest;
+
+    use crate::events::order::{expired::OrderExpired, stubs::*};
+
+    #[rstest]
+    fn test_order_cancel_rejected(order_expired: OrderExpired) {
+        let display = format!("{order_expired}");
+        assert_eq!(
+            display,
+            "OrderExpired(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
+        );
+    }
+}
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/denied.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/denied.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -129,14 +133,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         Some(self.reason)
     }
@@ -145,14 +157,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -165,14 +181,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -233,14 +257,22 @@
         None
     }
 
     fn account_id(&self) -> Option<AccountId> {
         None
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/emulated.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/emulated.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -125,14 +129,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -141,14 +153,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -161,14 +177,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -229,14 +253,22 @@
         None
     }
 
     fn account_id(&self) -> Option<AccountId> {
         None
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/event.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/event.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/expired.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_update.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,116 +17,119 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
-pub struct OrderExpired {
+pub struct OrderPendingUpdate {
     pub trader_id: TraderId,
     pub strategy_id: StrategyId,
     pub instrument_id: InstrumentId,
     pub client_order_id: ClientOrderId,
+    pub account_id: AccountId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
-    pub account_id: Option<AccountId>,
 }
 
-impl OrderExpired {
+impl OrderPendingUpdate {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
+        account_id: AccountId,
         event_id: UUID4,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
         reconciliation: bool,
         venue_order_id: Option<VenueOrderId>,
-        account_id: Option<AccountId>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
+            account_id,
             event_id,
             ts_event,
             ts_init,
             reconciliation: u8::from(reconciliation),
             venue_order_id,
-            account_id,
         })
     }
 }
 
-impl Debug for OrderExpired {
+impl Debug for OrderPendingUpdate {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(
-            f,
+        write!(f,
             "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
-            stringify!(OrderExpired),
+            stringify!(OrderPendingUpdate),
             self.trader_id,
             self.strategy_id,
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or_else(|| "None".to_string(), |venue_order_id| format!("{venue_order_id}")),
-            self.account_id.map_or_else(|| "None".to_string(), |account_id| format!("{account_id}")),
+            self.account_id,
             self.event_id,
             self.ts_event,
             self.ts_init
         )
     }
 }
 
-impl Display for OrderExpired {
+impl Display for OrderPendingUpdate {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
-            stringify!(OrderExpired),
+            stringify!(OrderPendingUpdate),
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
-            self.account_id.map_or("None".to_string(), |account_id| format!("{account_id}")),
+            self.account_id,
             self.ts_event
         )
     }
 }
 
-impl OrderEvent for OrderExpired {
+impl OrderEvent for OrderPendingUpdate {
     fn id(&self) -> UUID4 {
         self.event_id
     }
 
     fn kind(&self) -> &str {
-        stringify!(OrderExpired)
+        stringify!(OrderPendingUpdate)
     }
 
     fn order_type(&self) -> Option<OrderType> {
         None
     }
 
     fn order_side(&self) -> Option<OrderSide> {
@@ -141,14 +144,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -157,14 +168,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -177,14 +192,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -242,15 +265,23 @@
     }
 
     fn venue_order_id(&self) -> Option<VenueOrderId> {
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
-        self.account_id
+        Some(self.account_id)
+    }
+
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
     }
 
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
@@ -258,22 +289,21 @@
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
-mod tests {
-
+mod test {
     use rstest::rstest;
 
-    use crate::events::order::{expired::OrderExpired, stubs::*};
+    use crate::events::order::{pending_update::OrderPendingUpdate, stubs::order_pending_update};
 
     #[rstest]
-    fn test_order_cancel_rejected(order_expired: OrderExpired) {
-        let display = format!("{order_expired}");
+    fn test_order_pending_update_display(order_pending_update: OrderPendingUpdate) {
+        let display = format!("{order_pending_update}");
         assert_eq!(
             display,
-            "OrderExpired(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
+            "OrderPendingUpdate(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
         );
     }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/filled.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/filled.rs`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        Some(self.trade_id)
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        Some(self.currency)
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -279,14 +287,18 @@
         Some(self.last_qty)
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        Some(self.liquidity_side)
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -299,14 +311,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        Some(self.last_px)
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        Some(self.last_qty)
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -367,14 +387,22 @@
         Some(self.venue_order_id)
     }
 
     fn account_id(&self) -> Option<AccountId> {
         Some(self.account_id)
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        self.position_id
+    }
+
+    fn commission(&self) -> Option<Money> {
+        self.commission
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/initialized.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/initialized.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,27 @@
 
 use derive_builder::Builder;
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
     orders::any::OrderAny,
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, PartialEq, Eq, Builder, Serialize, Deserialize)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -395,14 +399,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -411,14 +423,18 @@
         Some(self.quantity)
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         Some(self.time_in_force)
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         Some(self.post_only)
     }
 
     fn reduce_only(&self) -> Option<bool> {
         Some(self.reduce_only)
     }
@@ -431,14 +447,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         self.price
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         self.trigger_price
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         self.trigger_type
     }
@@ -499,14 +523,22 @@
         None
     }
 
     fn account_id(&self) -> Option<AccountId> {
         None
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,25 @@
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 pub mod accepted;
 pub mod cancel_rejected;
 pub mod canceled;
 pub mod denied;
 pub mod emulated;
@@ -51,23 +55,28 @@
     fn id(&self) -> UUID4;
     fn kind(&self) -> &str;
     fn order_type(&self) -> Option<OrderType>;
     fn order_side(&self) -> Option<OrderSide>;
     fn trader_id(&self) -> TraderId;
     fn strategy_id(&self) -> StrategyId;
     fn instrument_id(&self) -> InstrumentId;
+    fn trade_id(&self) -> Option<TradeId>;
+    fn currency(&self) -> Option<Currency>;
     fn client_order_id(&self) -> ClientOrderId;
     fn reason(&self) -> Option<Ustr>;
     fn quantity(&self) -> Option<Quantity>;
     fn time_in_force(&self) -> Option<TimeInForce>;
+    fn liquidity_side(&self) -> Option<LiquiditySide>;
     fn post_only(&self) -> Option<bool>;
     fn reduce_only(&self) -> Option<bool>;
     fn quote_quantity(&self) -> Option<bool>;
     fn reconciliation(&self) -> bool;
     fn price(&self) -> Option<Price>;
+    fn last_px(&self) -> Option<Price>;
+    fn last_qty(&self) -> Option<Quantity>;
     fn trigger_price(&self) -> Option<Price>;
     fn trigger_type(&self) -> Option<TriggerType>;
     fn limit_offset(&self) -> Option<Price>;
     fn trailing_offset(&self) -> Option<Price>;
     fn trailing_offset_type(&self) -> Option<TrailingOffsetType>;
     fn expire_time(&self) -> Option<UnixNanos>;
     fn display_qty(&self) -> Option<Quantity>;
@@ -77,10 +86,12 @@
     fn order_list_id(&self) -> Option<OrderListId>;
     fn linked_order_ids(&self) -> Option<Vec<ClientOrderId>>;
     fn parent_order_id(&self) -> Option<ClientOrderId>;
     fn exec_algorithm_id(&self) -> Option<ExecAlgorithmId>;
     fn exec_spawn_id(&self) -> Option<ClientOrderId>;
     fn venue_order_id(&self) -> Option<VenueOrderId>;
     fn account_id(&self) -> Option<AccountId>;
+    fn position_id(&self) -> Option<PositionId>;
+    fn commission(&self) -> Option<Money>;
     fn ts_event(&self) -> UnixNanos;
     fn ts_init(&self) -> UnixNanos;
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/modify_rejected.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/modify_rejected.rs`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -145,14 +149,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         Some(self.reason)
     }
@@ -161,14 +173,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -181,14 +197,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -249,14 +273,22 @@
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         self.account_id
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/pending_cancel.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_cancel.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -140,14 +144,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -156,14 +168,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -176,14 +192,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -244,14 +268,22 @@
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         Some(self.account_id)
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/pending_update.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/canceled.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,115 +17,119 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
-pub struct OrderPendingUpdate {
+pub struct OrderCanceled {
     pub trader_id: TraderId,
     pub strategy_id: StrategyId,
     pub instrument_id: InstrumentId,
     pub client_order_id: ClientOrderId,
-    pub account_id: AccountId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
+    pub account_id: Option<AccountId>,
 }
 
-impl OrderPendingUpdate {
+impl OrderCanceled {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
-        account_id: AccountId,
         event_id: UUID4,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
         reconciliation: bool,
         venue_order_id: Option<VenueOrderId>,
+        account_id: Option<AccountId>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
-            account_id,
             event_id,
             ts_event,
             ts_init,
             reconciliation: u8::from(reconciliation),
             venue_order_id,
+            account_id,
         })
     }
 }
 
-impl Debug for OrderPendingUpdate {
+impl Debug for OrderCanceled {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f,
             "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
-            stringify!(OrderPendingUpdate),
+            stringify!(OrderCanceled),
             self.trader_id,
             self.strategy_id,
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or_else(|| "None".to_string(), |venue_order_id| format!("{venue_order_id}")),
-            self.account_id,
+            self.account_id.map_or_else(|| "None".to_string(), |account_id| format!("{account_id}")),
             self.event_id,
             self.ts_event,
             self.ts_init
         )
     }
 }
 
-impl Display for OrderPendingUpdate {
+impl Display for OrderCanceled {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
-            stringify!(OrderPendingUpdate),
+            stringify!(OrderCanceled),
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
-            self.account_id,
+            self.account_id.map_or("None".to_string(), |account_id| format!("{account_id}")),
             self.ts_event
         )
     }
 }
 
-impl OrderEvent for OrderPendingUpdate {
+impl OrderEvent for OrderCanceled {
     fn id(&self) -> UUID4 {
         self.event_id
     }
 
     fn kind(&self) -> &str {
-        stringify!(OrderPendingUpdate)
+        stringify!(OrderCanceled)
     }
 
     fn order_type(&self) -> Option<OrderType> {
         None
     }
 
     fn order_side(&self) -> Option<OrderSide> {
@@ -140,14 +144,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        todo!()
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -156,14 +168,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -176,14 +192,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -241,15 +265,23 @@
     }
 
     fn venue_order_id(&self) -> Option<VenueOrderId> {
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
-        Some(self.account_id)
+        self.account_id
+    }
+
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
     }
 
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
@@ -257,21 +289,8 @@
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
-mod test {
-    use rstest::rstest;
-
-    use crate::events::order::{pending_update::OrderPendingUpdate, stubs::order_pending_update};
-
-    #[rstest]
-    fn test_order_pending_update_display(order_pending_update: OrderPendingUpdate) {
-        let display = format!("{order_pending_update}");
-        assert_eq!(
-            display,
-            "OrderPendingUpdate(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
-        );
-    }
-}
+mod tests {}
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/rejected.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/rejected.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -140,14 +144,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         Some(self.reason)
     }
@@ -156,14 +168,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -176,14 +192,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -244,14 +268,22 @@
         None
     }
 
     fn account_id(&self) -> Option<AccountId> {
         Some(self.account_id)
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/released.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/released.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -129,14 +133,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -145,14 +157,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        todo!()
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -165,14 +181,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -233,14 +257,22 @@
         None
     }
 
     fn account_id(&self) -> Option<AccountId> {
         None
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/submitted.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/submitted.rs`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -131,14 +135,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -147,14 +159,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -167,14 +183,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -235,14 +259,22 @@
         None
     }
 
     fn account_id(&self) -> Option<AccountId> {
         Some(self.account_id)
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/triggered.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/triggered.rs`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -144,14 +148,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -160,14 +172,18 @@
         None
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -180,14 +196,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         None
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         None
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -248,14 +272,22 @@
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         self.account_id
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/order/updated.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/updated.rs`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 use derive_builder::Builder;
 use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
     events::order::OrderEvent,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
-        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
-        trader_id::TraderId, venue_order_id::VenueOrderId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
-    types::{price::Price, quantity::Quantity},
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 #[repr(C)]
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
@@ -156,14 +160,22 @@
         self.strategy_id
     }
 
     fn instrument_id(&self) -> InstrumentId {
         self.instrument_id
     }
 
+    fn trade_id(&self) -> Option<TradeId> {
+        None
+    }
+
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
+
     fn client_order_id(&self) -> ClientOrderId {
         self.client_order_id
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
@@ -172,14 +184,18 @@
         Some(self.quantity)
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
+
     fn post_only(&self) -> Option<bool> {
         None
     }
 
     fn reduce_only(&self) -> Option<bool> {
         None
     }
@@ -192,14 +208,22 @@
         false
     }
 
     fn price(&self) -> Option<Price> {
         self.price
     }
 
+    fn last_px(&self) -> Option<Price> {
+        None
+    }
+
+    fn last_qty(&self) -> Option<Quantity> {
+        None
+    }
+
     fn trigger_price(&self) -> Option<Price> {
         self.trigger_price
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
@@ -260,14 +284,22 @@
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         self.account_id
     }
 
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
+
+    fn commission(&self) -> Option<Money> {
+        None
+    }
+
     fn ts_event(&self) -> UnixNanos {
         self.ts_event
     }
 
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/position/changed.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/changed.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/position/closed.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/closed.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/position/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/position/opened.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/opened.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/events/position/state.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/state.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/bar.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/delta.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/deltas.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/deltas.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/depth.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/order.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/quote.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/data/trade.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/events/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/events/order.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/account_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/account_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/client_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/component_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/component_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/position_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/position_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/symbol.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/symbol.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/venue.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/instruments/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/instruments/synthetic.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/synthetic.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/orderbook/book.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/book.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/orderbook/level.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/level.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/orderbook/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/currency.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/currency.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/money.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/money.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/price.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/price.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/ffi/types/quantity.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/quantity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/account_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/account_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/client_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/client_order_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/component_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/component_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/instrument_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/instrument_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/macros.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/macros.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/order_list_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/order_list_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/position_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/position_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/strategy_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/strategy_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/symbol.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/symbol.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/trade_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trade_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/trader_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trader_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/venue.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/identifiers/venue_order_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/any.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/any.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/crypto_future.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_future.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/crypto_perpetual.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_perpetual.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/currency_pair.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/currency_pair.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/equity.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/equity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/futures_contract.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_contract.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/futures_spread.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_spread.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/options_contract.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_contract.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/options_spread.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_spread.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/instruments/synthetic.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/synthetic.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/macros.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/macros.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/aggregation.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/aggregation.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/analysis.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/analysis.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/book.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/book.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/display.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/display.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/error.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/error.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/ladder.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/ladder.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/level.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/level.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orderbook/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/any.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/any.rs`

 * *Files 1% similar despite different names*

```diff
@@ -101,26 +101,35 @@
 
     #[must_use]
     pub fn from_trailing_stop_market(order: StopMarketOrder) -> Self {
         Self::StopMarket(order)
     }
 
     pub fn from_events(events: Vec<OrderEventAny>) -> anyhow::Result<Self> {
+        println!("from events");
+        println!("events: {:?}", events);
         if events.is_empty() {
             anyhow::bail!("No events provided");
-        } else if events.len() == 1 {
-            let init_event = events.first().unwrap();
-            match init_event {
-                OrderEventAny::Initialized(init) => Ok(init.to_owned().into()),
-                _ => {
-                    anyhow::bail!("First event must be OrderInitialized");
+        }
+        // pop the first event
+        let init_event = events.first().unwrap();
+        match init_event {
+            OrderEventAny::Initialized(init) => {
+                let mut order = Self::from(init.clone());
+                // apply the rest of the events
+                for event in events.into_iter().skip(1) {
+                    // apply event to order
+                    println!("applying event: {:?}", event);
+                    order.apply(event).unwrap();
                 }
+                Ok(order)
+            }
+            _ => {
+                anyhow::bail!("First event must be OrderInitialized");
             }
-        } else {
-            anyhow::bail!("Only one event can be provided");
         }
     }
 }
 
 impl PartialEq for OrderAny {
     fn eq(&self, other: &Self) -> bool {
         self.client_order_id() == other.client_order_id()
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/base.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/base.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/default.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/default.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/limit_if_touched.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit_if_touched.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/list.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/list.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/market.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/market_if_touched.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_if_touched.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/market_to_limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_to_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/stop_limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/stop_market.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/stubs.rs`

 * *Files 18% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 use std::str::FromStr;
 
 use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
 
 use super::{limit::LimitOrder, stop_market::StopMarketOrder};
 use crate::{
     enums::{LiquiditySide, OrderSide, TimeInForce, TriggerType},
-    events::order::filled::OrderFilled,
+    events::order::{accepted::OrderAccepted, filled::OrderFilled, submitted::OrderSubmitted},
     identifiers::{
+        account_id::AccountId,
         client_order_id::ClientOrderId,
         instrument_id::InstrumentId,
         position_id::PositionId,
         strategy_id::StrategyId,
         stubs::{strategy_id_ema_cross, trader_id},
         trade_id::TradeId,
+        venue_order_id::VenueOrderId,
     },
     instruments::Instrument,
     orders::{base::Order, market::MarketOrder},
     types::{money::Money, price::Price, quantity::Quantity},
 };
 
 // Test Event Stubs
@@ -45,32 +47,35 @@
         strategy_id: Option<StrategyId>,
         trade_id: Option<TradeId>,
         position_id: Option<PositionId>,
         last_px: Option<Price>,
         last_qty: Option<Quantity>,
         commission: Option<Money>,
         ts_filled_ns: Option<UnixNanos>,
-    ) -> OrderFilled {
+        account_id: Option<AccountId>,
+    ) -> anyhow::Result<OrderFilled> {
         let trader_id = trader_id();
         let strategy_id = strategy_id.unwrap_or(order.strategy_id());
         let instrument_id = order.instrument_id();
         let venue_order_id = order.venue_order_id().unwrap_or_default();
-        let account_id = order.account_id().unwrap_or_default();
+        let account_id = account_id
+            .or(order.account_id())
+            .unwrap_or(AccountId::from("SIM-001"));
         let trade_id = trade_id.unwrap_or(
             TradeId::new(order.client_order_id().as_str().replace('O', "E").as_str()).unwrap(),
         );
         let liquidity_side = order.liquidity_side().unwrap_or(LiquiditySide::Maker);
         let event = UUID4::new();
         let position_id = position_id
             .or_else(|| order.position_id())
             .unwrap_or(PositionId::new("1").unwrap());
         let commission = commission.unwrap_or(Money::from_str("2 USD").unwrap());
         let last_px = last_px.unwrap_or(Price::from_str("1.0").unwrap());
         let last_qty = last_qty.unwrap_or(order.quantity());
-        OrderFilled::new(
+        Ok(OrderFilled::new(
             trader_id,
             strategy_id,
             instrument_id,
             order.client_order_id(),
             venue_order_id,
             account_id,
             trade_id,
@@ -83,15 +88,60 @@
             event,
             ts_filled_ns.unwrap_or_default(),
             UnixNanos::default(),
             false,
             Some(position_id),
             Some(commission),
         )
-        .unwrap()
+        .unwrap())
+    }
+
+    pub fn order_submitted<T: Order>(
+        order: &T,
+        account_id: AccountId,
+    ) -> anyhow::Result<OrderSubmitted> {
+        let trader_id = trader_id();
+        let strategy_id = order.strategy_id();
+        let instrument_id = order.instrument_id();
+        let client_order_id = order.client_order_id();
+        Ok(OrderSubmitted::new(
+            trader_id,
+            strategy_id,
+            instrument_id,
+            client_order_id,
+            account_id,
+            UUID4::new(),
+            UnixNanos::default(),
+            UnixNanos::default(),
+        )
+        .unwrap())
+    }
+
+    pub fn order_accepted<T: Order>(
+        order: &T,
+        account_id: AccountId,
+        venue_order_id: VenueOrderId,
+    ) -> anyhow::Result<OrderAccepted> {
+        let trader_id = trader_id();
+        let strategy_id = order.strategy_id();
+        let instrument_id = order.instrument_id();
+        let client_order_id = order.client_order_id();
+        Ok(OrderAccepted::new(
+            trader_id,
+            strategy_id,
+            instrument_id,
+            client_order_id,
+            venue_order_id,
+            account_id,
+            UUID4::new(),
+            UnixNanos::default(),
+            UnixNanos::default(),
+            false,
+        )
+        .unwrap())
     }
 }
 
 pub struct TestOrderStubs;
 
 impl TestOrderStubs {
     #[must_use]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/trailing_stop_limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/orders/trailing_stop_market.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/polymorphism.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/polymorphism.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/position.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/position.rs`

 * *Files 3% similar despite different names*

```diff
@@ -578,26 +578,30 @@
             None,
             Some(TradeId::new("1").unwrap()),
             None,
             Some(Price::from("1.00001")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let fill2 = TestOrderEventStubs::order_filled::<MarketOrder, CurrencyPair>(
             &order2,
             &audusd_sim,
             None,
             Some(TradeId::new("1").unwrap()),
             None,
             Some(Price::from("1.00002")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(audusd_sim, fill1).unwrap();
         position.apply(&fill2);
     }
 
     #[rstest]
     fn test_position_filled_with_buy_order(audusd_sim: CurrencyPair) {
         let order = TestOrderStubs::market_order(
@@ -613,15 +617,17 @@
             None,
             None,
             None,
             Some(Price::from("1.00001")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let last_price = Price::from_str("1.0005").unwrap();
         let position = Position::new(audusd_sim, fill).unwrap();
         assert_eq!(position.symbol(), audusd_sim.id.symbol);
         assert_eq!(position.venue(), audusd_sim.id.venue);
         assert!(!position.is_opposite_side(fill.order_side));
         assert_eq!(position, position); // equality operator test
         assert!(position.closing_order_id.is_none());
@@ -679,15 +685,17 @@
             None,
             None,
             None,
             Some(Price::from("1.00001")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let last_price = Price::from_str("1.00050").unwrap();
         let position = Position::new(audusd_sim, fill).unwrap();
         assert_eq!(position.symbol(), audusd_sim.id.symbol);
         assert_eq!(position.venue(), audusd_sim.id.venue);
         assert!(!position.is_opposite_side(fill.order_side));
         assert_eq!(position, position); // equality operator test
         assert!(position.closing_order_id.is_none());
@@ -743,15 +751,17 @@
             None,
             None,
             None,
             Some(Price::from("1.00001")),
             Some(Quantity::from(50_000)),
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let last_price = Price::from_str("1.00048").unwrap();
         let position = Position::new(audusd_sim, fill).unwrap();
         assert_eq!(position.quantity, Quantity::from(50_000));
         assert_eq!(position.peak_qty, Quantity::from(50_000));
         assert_eq!(position.side, PositionSide::Long);
         assert_eq!(position.signed_qty, 50000.0);
         assert_eq!(position.avg_px_open, 1.00001);
@@ -799,26 +809,30 @@
             None,
             Some(TradeId::new("1").unwrap()),
             None,
             Some(Price::from("1.00001")),
             Some(Quantity::from(50_000)),
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let fill2 = TestOrderEventStubs::order_filled::<MarketOrder, CurrencyPair>(
             &order,
             &audusd_sim,
             None,
             Some(TradeId::new("2").unwrap()),
             None,
             Some(Price::from("1.00002")),
             Some(Quantity::from(50_000)),
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let last_price = Price::from_str("1.0005").unwrap();
         let mut position = Position::new(audusd_sim, fill1).unwrap();
         position.apply(&fill2);
 
         assert_eq!(position.quantity, Quantity::from(100_000));
         assert_eq!(position.peak_qty, Quantity::from(100_000));
         assert_eq!(position.side, PositionSide::Short);
@@ -864,15 +878,17 @@
             Some(StrategyId::new("S-001").unwrap()),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-1").unwrap()),
             Some(Price::from("1.00001")),
             None,
             None,
             Some(UnixNanos::from(1_000_000_000)),
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(audusd_sim, fill).unwrap();
 
         let fill2 = OrderFilled::new(
             order.trader_id,
             StrategyId::new("S-001").unwrap(),
             order.instrument_id,
             order.client_order_id,
@@ -954,39 +970,45 @@
             None,
             None,
             Some(PositionId::new("P-19700101-0000-000-001-1").unwrap()),
             Some(Price::from("1.0")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(audusd_sim, fill1).unwrap();
         // create closing from order from different venue but same strategy
         let fill2 = TestOrderEventStubs::order_filled(
             &order2,
             &audusd_sim,
             Some(StrategyId::new("S-001").unwrap()),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-19700101-0000-000-001-1").unwrap()),
             Some(Price::from("1.00001")),
             Some(Quantity::from(50_000)),
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let fill3 = TestOrderEventStubs::order_filled(
             &order2,
             &audusd_sim,
             Some(StrategyId::new("S-001").unwrap()),
             Some(TradeId::new("2").unwrap()),
             Some(PositionId::new("P-19700101-0000-000-001-1").unwrap()),
             Some(Price::from("1.00003")),
             Some(Quantity::from(50_000)),
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let last = Price::from("1.0005");
         position.apply(&fill2);
         position.apply(&fill3);
 
         assert_eq!(
             position.quantity,
             Quantity::zero(audusd_sim.price_precision)
@@ -1045,27 +1067,31 @@
             None,
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-19700101-0000-000-001-1").unwrap()),
             Some(Price::from("1.0")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(audusd_sim, fill1).unwrap();
         let fill2 = TestOrderEventStubs::order_filled(
             &order2,
             &audusd_sim,
             None,
             Some(TradeId::new("2").unwrap()),
             Some(PositionId::new("P-19700101-0000-000-001-1").unwrap()),
             Some(Price::from("1.0")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let last = Price::from("1.0005");
         position.apply(&fill2);
 
         assert_eq!(
             position.quantity,
             Quantity::zero(audusd_sim.price_precision)
         );
@@ -1131,37 +1157,43 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("1.0")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let fill2 = TestOrderEventStubs::order_filled(
             &order2,
             &audusd_sim,
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("2").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("1.00001")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let fill3 = TestOrderEventStubs::order_filled(
             &order3,
             &audusd_sim,
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("3").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("1.0001")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(audusd_sim, fill1).unwrap();
         let last = Price::from("1.0005");
         position.apply(&fill2);
         position.apply(&fill3);
 
         assert_eq!(
             position.quantity,
@@ -1219,15 +1251,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(price1),
             None,
             Some(commission1),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(currency_pair_ethusdt, fill1).unwrap();
         let quantity2 = Quantity::from(17);
         let order2 = TestOrderStubs::market_order(
             currency_pair_ethusdt.id,
             OrderSide::Buy,
             quantity2,
             None,
@@ -1242,15 +1276,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("2").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(price2),
             None,
             Some(commission2),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill2);
         assert_eq!(position.quantity, Quantity::from(29));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from_str("-0.28830000 USDT").unwrap())
         );
         assert_eq!(position.avg_px_open, 99.413_793_103_448_27);
@@ -1271,15 +1307,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("3").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(price3),
             None,
             Some(commission3),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill3);
         assert_eq!(position.quantity, Quantity::from(20));
         assert_eq!(position.realized_pnl, Some(Money::from("13.89666207 USDT")));
         assert_eq!(position.avg_px_open, 99.413_793_103_448_27);
         let quantity4 = Quantity::from("4");
         let price4 = Price::from("105.0");
         let order4 = TestOrderStubs::market_order(
@@ -1297,15 +1335,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("4").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(price4),
             None,
             Some(commission4),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill4);
         assert_eq!(position.quantity, Quantity::from("16"));
         assert_eq!(position.realized_pnl, Some(Money::from("36.19948966 USDT")));
         assert_eq!(position.avg_px_open, 99.413_793_103_448_27);
         let quantity5 = Quantity::from("3");
         let price5 = Price::from("103.0");
         let order5 = TestOrderStubs::market_order(
@@ -1323,15 +1363,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("5").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(price5),
             None,
             Some(commission5),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill5);
         assert_eq!(position.quantity, Quantity::from("19"));
         assert_eq!(position.realized_pnl, Some(Money::from("36.16858966 USDT")));
         assert_eq!(position.avg_px_open, 99.980_036_297_640_65);
         assert_eq!(
             format!("{position}"),
             "Position(LONG 19.00000 ETHUSDT.BINANCE, id=P-123456)"
@@ -1351,15 +1393,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("5").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("1.00001")),
             None,
             Some(commission1),
             Some(UnixNanos::from(1_000_000_000)),
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(audusd_sim, fill1).unwrap();
 
         let fill2 = OrderFilled::new(
             order.trader_id,
             order.strategy_id,
             order.instrument_id,
             order.client_order_id,
@@ -1470,15 +1514,17 @@
             None,
             Some(TradeId::from("1")),
             Some(PositionId::from("P-19700101-0000-000-001-1")),
             Some(Price::from("10000.0")),
             None,
             Some(commission1),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(currency_pair_btcusdt, fill1).unwrap();
         let order2 = TestOrderStubs::market_order(
             currency_pair_btcusdt.id,
             OrderSide::Buy,
             Quantity::from(17),
             None,
             None,
@@ -1496,15 +1542,17 @@
             None,
             Some(TradeId::from("2")),
             Some(PositionId::from("P-19700101-0000-000-001-1")),
             Some(Price::from("9999.0")),
             None,
             Some(commission2),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill2);
         assert_eq!(position.quantity, Quantity::from(29));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from_str("-289.98300000 USDT").unwrap())
         );
         assert_eq!(position.avg_px_open, 9_999.413_793_103_447);
@@ -1528,15 +1576,17 @@
             None,
             Some(TradeId::from("3")),
             Some(PositionId::from("P-19700101-0000-000-001-1")),
             Some(Price::from("10001.0")),
             None,
             Some(commission3),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill3);
         assert_eq!(position.quantity, Quantity::from(20));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from_str("-365.71613793 USDT").unwrap())
         );
         assert_eq!(position.avg_px_open, 9_999.413_793_103_447);
@@ -1560,15 +1610,17 @@
             None,
             Some(TradeId::from("4")),
             Some(PositionId::from("P-19700101-0000-000-001-1")),
             Some(Price::from("10003.0")),
             None,
             Some(commission4),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill4);
         assert_eq!(position.quantity, Quantity::from(23));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from_str("-395.72513793 USDT").unwrap())
         );
         assert_eq!(position.avg_px_open, 9_999.881_559_220_39);
@@ -1592,15 +1644,17 @@
             None,
             Some(TradeId::from("5")),
             Some(PositionId::from("P-19700101-0000-000-001-1")),
             Some(Price::from("10005.0")),
             None,
             Some(commission5),
             None,
-        );
+            None,
+        )
+        .unwrap();
         position.apply(&fill5);
         assert_eq!(position.quantity, Quantity::from(19));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from_str("-415.27137481 USDT").unwrap())
         );
         assert_eq!(position.avg_px_open, 9_999.881_559_220_39);
@@ -1627,15 +1681,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("10500.0")),
             None,
             None,
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill).unwrap();
         let result = position.calculate_pnl(10500.0, 10500.0, Quantity::from("100000.0"));
         assert_eq!(result, Money::from("0 USDT"));
     }
 
     #[rstest]
     fn test_calculate_pnl_for_long_position_win(currency_pair_btcusdt: CurrencyPair) {
@@ -1659,15 +1715,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("10500.0")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill).unwrap();
         let pnl = position.calculate_pnl(10500.0, 10510.0, Quantity::from("12.0"));
         assert_eq!(pnl, Money::from("120 USDT"));
         assert_eq!(position.realized_pnl, Some(Money::from("-126 USDT")));
         assert_eq!(
             position.unrealized_pnl(Price::from("10510.0")),
             Money::from("120.0 USDT")
@@ -1701,15 +1759,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("10500.0")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill).unwrap();
         let pnl = position.calculate_pnl(10500.0, 10480.5, Quantity::from("10.0"));
         assert_eq!(pnl, Money::from("-195 USDT"));
         assert_eq!(position.realized_pnl, Some(Money::from("-126 USDT")));
         assert_eq!(
             position.unrealized_pnl(Price::from("10480.50")),
             Money::from("-234.0 USDT")
@@ -1743,15 +1803,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("10500.0")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill).unwrap();
         let pnl = position.calculate_pnl(10500.0, 10390.0, Quantity::from("10.15"));
         assert_eq!(pnl, Money::from("1116.5 USDT"));
         assert_eq!(
             position.unrealized_pnl(Price::from("10390.0")),
             Money::from("1116.5 USDT")
         );
@@ -1785,15 +1847,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("10500.0")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill).unwrap();
         let pnl = position.calculate_pnl(10500.0, 10670.5, Quantity::from("10.0"));
         assert_eq!(pnl, Money::from("-1705 USDT"));
         assert_eq!(
             position.unrealized_pnl(Price::from("10670.5")),
             Money::from("-1705 USDT")
         );
@@ -1823,15 +1887,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("10000.0")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(xbtusd_bitmex, fill).unwrap();
         let pnl = position.calculate_pnl(10000.0, 11000.0, Quantity::from("100000.0"));
         assert_eq!(pnl, Money::from("-0.90909091 BTC"));
         assert_eq!(
             position.unrealized_pnl(Price::from("11000.0")),
             Money::from("-0.90909091 BTC")
         );
@@ -1860,15 +1926,17 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             Some(Price::from("375.95")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(ethusdt_bitmex, fill).unwrap();
 
         assert_eq!(
             position.unrealized_pnl(Price::from("370.00")),
             Money::from("4.27745208 ETH")
         );
         assert_eq!(
@@ -1906,15 +1974,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("10500.00")),
             None,
             Some(commission1),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let commission2 = calculate_commission(
             currency_pair_btcusdt,
             order2.quantity,
             Price::from("10500.0"),
             None,
         )
         .unwrap();
@@ -1924,15 +1994,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("2").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("10500.00")),
             None,
             Some(commission2),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let mut position = Position::new(currency_pair_btcusdt, fill1).unwrap();
         position.apply(&fill2);
         let pnl = position.unrealized_pnl(Price::from("11505.60"));
         assert_eq!(pnl, Money::from("4022.40000000 USDT"));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from("-42.00000000 USDT"))
@@ -1965,15 +2037,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("10505.60")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(currency_pair_btcusdt, fill).unwrap();
         let pnl = position.unrealized_pnl(Price::from("10407.15"));
         assert_eq!(pnl, Money::from("582.03640000 USDT"));
         assert_eq!(
             position.realized_pnl,
             Some(Money::from("-62.10910720 USDT"))
         );
@@ -2001,15 +2075,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("10500.00")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
 
         let position = Position::new(xbtusd_bitmex, fill).unwrap();
         let pnl = position.unrealized_pnl(Price::from("11505.60"));
         assert_eq!(pnl, Money::from("0.83238969 BTC"));
         assert_eq!(position.realized_pnl, Some(Money::from("-0.00714286 BTC")));
         assert_eq!(position.commissions(), vec![Money::from("0.00714286 BTC")]);
     }
@@ -2032,15 +2108,17 @@
             Some(StrategyId::from("S-001")),
             Some(TradeId::new("1").unwrap()),
             Some(PositionId::new("P-123456").unwrap()),
             Some(Price::from("15500.00")),
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(xbtusd_bitmex, fill).unwrap();
         let pnl = position.unrealized_pnl(Price::from("12506.65"));
 
         assert_eq!(pnl, Money::from("19.30166700 BTC"));
         assert_eq!(position.realized_pnl, Some(Money::from("-0.06048387 BTC")));
         assert_eq!(position.commissions(), vec![Money::from("0.06048387 BTC")]);
     }
@@ -2070,12 +2148,14 @@
             None,
             None,
             Some(PositionId::from("P-123456")),
             None,
             None,
             Some(commission),
             None,
-        );
+            None,
+        )
+        .unwrap();
         let position = Position::new(audusd_sim, fill).unwrap();
         assert_eq!(position.signed_qty, expected);
     }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/common.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/common.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/bar.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/delta.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/deltas.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/deltas.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/depth.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/order.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/quote.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/data/trade.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/enums.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/account/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/account/state.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/state.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/accepted.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/accepted.rs`

 * *Files 5% similar despite different names*

```diff
@@ -70,18 +70,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderAccepted)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs`

 * *Files 1% similar despite different names*

```diff
@@ -76,18 +76,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderCancelRejected)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/canceled.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/canceled.rs`

 * *Files 3% similar despite different names*

```diff
@@ -70,18 +70,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderCanceled)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/denied.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/denied.rs`

 * *Files 6% similar despite different names*

```diff
@@ -70,18 +70,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderDenied)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/emulated.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/emulated.rs`

 * *Files 5% similar despite different names*

```diff
@@ -64,18 +64,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderEmulated)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/expired.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/expired.rs`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderExpired)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/filled.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/filled.rs`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderFilled)
-    }
-
     #[getter]
     #[pyo3(name = "is_buy")]
     fn py_is_buy(&self) -> bool {
         self.is_buy()
     }
 
     #[getter]
@@ -248,14 +244,15 @@
         dict.set_item("last_px", self.last_px.to_string())?;
         dict.set_item("currency", self.currency.code.to_string())?;
         dict.set_item("liquidity_side", self.liquidity_side.to_string())?;
         dict.set_item("event_id", self.event_id.to_string())?;
         dict.set_item("ts_event", self.ts_event.as_u64())?;
         dict.set_item("ts_init", self.ts_init.as_u64())?;
         dict.set_item("reconciliation", self.reconciliation)?;
+        dict.set_item("info", PyDict::new(py))?;
         match self.position_id {
             Some(position_id) => dict.set_item("position_id", position_id.to_string())?,
             None => dict.set_item("position_id", py.None())?,
         }
         match self.commission {
             Some(commission) => dict.set_item("commission", commission.to_string())?,
             None => dict.set_item("commission", py.None())?,
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/initialized.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/initialized.rs`

 * *Files 3% similar despite different names*

```diff
@@ -140,18 +140,14 @@
 
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderInitiliazed)
-    }
-
     #[pyo3(name = "to_dict")]
     fn py_to_dict(&self, py: Python<'_>) -> PyResult<PyObject> {
         let dict = PyDict::new(py);
         dict.set_item("type", stringify!(OrderInitiliazed));
         dict.set_item("trader_id", self.trader_id.to_string())?;
         dict.set_item("strategy_id", self.strategy_id.to_string())?;
         dict.set_item("instrument_id", self.instrument_id.to_string())?;
@@ -161,15 +157,21 @@
         dict.set_item("quantity", self.quantity.to_string())?;
         dict.set_item("time_in_force", self.time_in_force.to_string())?;
         dict.set_item("post_only", self.post_only)?;
         dict.set_item("reduce_only", self.reduce_only)?;
         dict.set_item("quote_quantity", self.quote_quantity)?;
         dict.set_item("reconciliation", self.reconciliation)?;
         // TODO remove options as in legacy cython only
-        dict.set_item("options", PyDict::new(py))?;
+        let options = PyDict::new(py);
+        if self.order_type == OrderType::StopMarket {
+            options.set_item("trigger_type", self.trigger_type.map(|x| x.to_string()))?;
+            options.set_item("trigger_price", self.trigger_price.map(|x| x.to_string()))?;
+            options.set_item("expire_time_ns", self.expire_time.map(|x| x.to_string()))?;
+        }
+        dict.set_item("options", options)?;
         dict.set_item("event_id", self.event_id.to_string())?;
         dict.set_item("ts_event", self.ts_event.as_u64())?;
         dict.set_item("ts_init", self.ts_init.as_u64())?;
         match self.price {
             Some(price) => dict.set_item("price", price.to_string())?,
             None => dict.set_item("price", py.None())?,
         }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         OrderEventAny::Updated(event) => Ok(event.into_py(py)),
         OrderEventAny::PartiallyFilled(event) => Ok(event.into_py(py)),
         OrderEventAny::Filled(event) => Ok(event.into_py(py)),
     }
 }
 
 pub fn pyobject_to_order_event(py: Python, order_event: PyObject) -> PyResult<OrderEventAny> {
-    match order_event.getattr(py, "type_str")?.extract::<&str>(py)? {
+    let class = order_event.getattr(py, "__class__")?;
+    match class.getattr(py, "__name__")?.extract::<&str>(py)? {
         stringify!(OrderAccepted) => Ok(OrderEventAny::Accepted(
             order_event.extract::<OrderAccepted>(py)?,
         )),
         stringify!(OrderCancelRejected) => Ok(OrderEventAny::CancelRejected(
             order_event.extract::<OrderCancelRejected>(py)?,
         )),
         stringify!(OrderCanceled) => Ok(OrderEventAny::Canceled(
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/modify_rejected.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/modify_rejected.rs`

 * *Files 2% similar despite different names*

```diff
@@ -76,18 +76,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderModifyRejected)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/pending_cancel.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_update.rs`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 use nautilus_core::{
     python::{serialization::from_dict_pyo3, to_pyvalue_err},
     uuid::UUID4,
 };
 use pyo3::{basic::CompareOp, prelude::*, types::PyDict};
 
 use crate::{
-    events::order::pending_cancel::OrderPendingCancel,
+    events::order::pending_update::OrderPendingUpdate,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, instrument_id::InstrumentId,
         strategy_id::StrategyId, trader_id::TraderId, venue_order_id::VenueOrderId,
     },
 };
 
 #[pymethods]
-impl OrderPendingCancel {
+impl OrderPendingUpdate {
     #[allow(clippy::too_many_arguments)]
     #[new]
     fn py_new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
@@ -70,28 +70,24 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderPendingCancel)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
     fn py_to_dict(&self, py: Python<'_>) -> PyResult<PyObject> {
         let dict = PyDict::new(py);
-        dict.set_item("type", stringify!(OrderPendingCancel));
+        dict.set_item("type", stringify!(OrderPendingUpdate));
         dict.set_item("trader_id", self.trader_id.to_string())?;
         dict.set_item("strategy_id", self.strategy_id.to_string())?;
         dict.set_item("instrument_id", self.instrument_id.to_string())?;
         dict.set_item("client_order_id", self.client_order_id.to_string())?;
         dict.set_item("account_id", self.account_id.to_string())?;
         dict.set_item("event_id", self.event_id.to_string())?;
         dict.set_item("ts_event", self.ts_event.as_u64())?;
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/pending_update.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/triggered.rs`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 use nautilus_core::{
     python::{serialization::from_dict_pyo3, to_pyvalue_err},
     uuid::UUID4,
 };
 use pyo3::{basic::CompareOp, prelude::*, types::PyDict};
 
 use crate::{
-    events::order::pending_update::OrderPendingUpdate,
+    events::order::triggered::OrderTriggered,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, instrument_id::InstrumentId,
         strategy_id::StrategyId, trader_id::TraderId, venue_order_id::VenueOrderId,
     },
 };
 
 #[pymethods]
-impl OrderPendingUpdate {
+impl OrderTriggered {
     #[allow(clippy::too_many_arguments)]
     #[new]
     fn py_new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
-        account_id: AccountId,
         event_id: UUID4,
         ts_event: u64,
         ts_init: u64,
         reconciliation: bool,
         venue_order_id: Option<VenueOrderId>,
+        account_id: Option<AccountId>,
     ) -> PyResult<Self> {
         Self::new(
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
-            account_id,
             event_id,
             ts_event.into(),
             ts_init.into(),
             reconciliation,
             venue_order_id,
+            account_id,
         )
         .map_err(to_pyvalue_err)
     }
 
     fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> Py<PyAny> {
         match op {
             CompareOp::Eq => self.eq(other).into_py(py),
@@ -70,37 +70,36 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderPendingUpdate)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
     fn py_to_dict(&self, py: Python<'_>) -> PyResult<PyObject> {
         let dict = PyDict::new(py);
-        dict.set_item("type", stringify!(OrderPendingUpdate));
+        dict.set_item("type", stringify!(OrderTriggered));
         dict.set_item("trader_id", self.trader_id.to_string())?;
         dict.set_item("strategy_id", self.strategy_id.to_string())?;
         dict.set_item("instrument_id", self.instrument_id.to_string())?;
         dict.set_item("client_order_id", self.client_order_id.to_string())?;
-        dict.set_item("account_id", self.account_id.to_string())?;
         dict.set_item("event_id", self.event_id.to_string())?;
         dict.set_item("ts_event", self.ts_event.as_u64())?;
         dict.set_item("ts_init", self.ts_init.as_u64())?;
         dict.set_item("reconciliation", self.reconciliation)?;
         match self.venue_order_id {
             Some(venue_order_id) => dict.set_item("venue_order_id", venue_order_id.to_string())?,
-            None => dict.set_item("venue_order_id", py.None())?,
+            None => dict.set_item("venue_order_id", "None")?,
+        }
+        match self.account_id {
+            Some(account_id) => dict.set_item("account_id", account_id.to_string())?,
+            None => dict.set_item("account_id", "None")?,
         }
         Ok(dict.into())
     }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/rejected.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/rejected.rs`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderRejected)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/released.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/released.rs`

 * *Files 3% similar despite different names*

```diff
@@ -67,18 +67,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderReleased)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/submitted.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/submitted.rs`

 * *Files 5% similar despite different names*

```diff
@@ -66,18 +66,14 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderSubmitted)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/triggered.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/updated.rs`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,55 @@
 use nautilus_core::{
     python::{serialization::from_dict_pyo3, to_pyvalue_err},
     uuid::UUID4,
 };
 use pyo3::{basic::CompareOp, prelude::*, types::PyDict};
 
 use crate::{
-    events::order::triggered::OrderTriggered,
+    events::order::updated::OrderUpdated,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, instrument_id::InstrumentId,
         strategy_id::StrategyId, trader_id::TraderId, venue_order_id::VenueOrderId,
     },
+    types::{price::Price, quantity::Quantity},
 };
 
 #[pymethods]
-impl OrderTriggered {
+impl OrderUpdated {
     #[allow(clippy::too_many_arguments)]
     #[new]
     fn py_new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
+        quantity: Quantity,
         event_id: UUID4,
         ts_event: u64,
         ts_init: u64,
         reconciliation: bool,
         venue_order_id: Option<VenueOrderId>,
         account_id: Option<AccountId>,
+        price: Option<Price>,
+        trigger_price: Option<Price>,
     ) -> PyResult<Self> {
         Self::new(
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
+            quantity,
             event_id,
             ts_event.into(),
             ts_init.into(),
             reconciliation,
             venue_order_id,
             account_id,
+            price,
+            trigger_price,
         )
         .map_err(to_pyvalue_err)
     }
 
     fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> Py<PyAny> {
         match op {
             CompareOp::Eq => self.eq(other).into_py(py),
@@ -70,40 +77,45 @@
         format!("{:?}", self)
     }
 
     fn __str__(&self) -> String {
         self.to_string()
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderTriggered)
-    }
-
     #[staticmethod]
     #[pyo3(name = "from_dict")]
     fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
         from_dict_pyo3(py, values)
     }
 
     #[pyo3(name = "to_dict")]
     fn py_to_dict(&self, py: Python<'_>) -> PyResult<PyObject> {
         let dict = PyDict::new(py);
-        dict.set_item("type", stringify!(OrderTriggered));
+        dict.set_item("type", stringify!(OrderUpdated));
         dict.set_item("trader_id", self.trader_id.to_string())?;
         dict.set_item("strategy_id", self.strategy_id.to_string())?;
         dict.set_item("instrument_id", self.instrument_id.to_string())?;
         dict.set_item("client_order_id", self.client_order_id.to_string())?;
+        dict.set_item("quantity", self.quantity.to_string())?;
         dict.set_item("event_id", self.event_id.to_string())?;
         dict.set_item("ts_event", self.ts_event.as_u64())?;
         dict.set_item("ts_init", self.ts_init.as_u64())?;
         dict.set_item("reconciliation", self.reconciliation)?;
         match self.venue_order_id {
             Some(venue_order_id) => dict.set_item("venue_order_id", venue_order_id.to_string())?,
-            None => dict.set_item("venue_order_id", "None")?,
+            None => dict.set_item("venue_order_id", py.None())?,
         }
         match self.account_id {
             Some(account_id) => dict.set_item("account_id", account_id.to_string())?,
-            None => dict.set_item("account_id", "None")?,
+            None => dict.set_item("account_id", py.None())?,
+        }
+        match self.price {
+            Some(price) => dict.set_item("price", price.to_string())?,
+            None => dict.set_item("price", py.None())?,
+        }
+        match self.trigger_price {
+            Some(trigger_price) => dict.set_item("trigger_price", trigger_price.to_string())?,
+            None => dict.set_item("trigger_price", py.None())?,
         }
         Ok(dict.into())
     }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/events/order/updated.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit_if_touched.rs`

 * *Files 20% similar despite different names*

```diff
@@ -9,117 +9,122 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-use nautilus_core::{
-    python::{serialization::from_dict_pyo3, to_pyvalue_err},
-    uuid::UUID4,
-};
-use pyo3::{basic::CompareOp, prelude::*, types::PyDict};
+use std::collections::HashMap;
+
+use nautilus_core::{python::to_pyruntime_err, uuid::UUID4};
+use pyo3::prelude::*;
+use ustr::Ustr;
 
 use crate::{
-    events::order::updated::OrderUpdated,
+    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TriggerType},
+    events::order::initialized::OrderInitialized,
     identifiers::{
-        account_id::AccountId, client_order_id::ClientOrderId, instrument_id::InstrumentId,
-        strategy_id::StrategyId, trader_id::TraderId, venue_order_id::VenueOrderId,
+        client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
+        trader_id::TraderId,
     },
+    orders::{
+        base::{str_hashmap_to_ustr, Order},
+        limit_if_touched::LimitIfTouchedOrder,
+    },
+    python::events::order::{order_event_to_pyobject, pyobject_to_order_event},
     types::{price::Price, quantity::Quantity},
 };
 
 #[pymethods]
-impl OrderUpdated {
-    #[allow(clippy::too_many_arguments)]
+impl LimitIfTouchedOrder {
     #[new]
+    #[allow(clippy::too_many_arguments)]
     fn py_new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
+        order_side: OrderSide,
         quantity: Quantity,
-        event_id: UUID4,
-        ts_event: u64,
+        price: Price,
+        trigger_price: Price,
+        trigger_type: TriggerType,
+        time_in_force: TimeInForce,
+        post_only: bool,
+        reduce_only: bool,
+        quote_quantity: bool,
+        init_id: UUID4,
         ts_init: u64,
-        reconciliation: bool,
-        venue_order_id: Option<VenueOrderId>,
-        account_id: Option<AccountId>,
-        price: Option<Price>,
-        trigger_price: Option<Price>,
+        expire_time: Option<u64>,
+        display_qty: Option<Quantity>,
+        emulation_trigger: Option<TriggerType>,
+        trigger_instrument_id: Option<InstrumentId>,
+        contingency_type: Option<ContingencyType>,
+        order_list_id: Option<OrderListId>,
+        linked_order_ids: Option<Vec<ClientOrderId>>,
+        parent_order_id: Option<ClientOrderId>,
+        exec_algorithm_id: Option<ExecAlgorithmId>,
+        exec_algorithm_params: Option<HashMap<String, String>>,
+        exec_spawn_id: Option<ClientOrderId>,
+        tags: Option<Vec<String>>,
     ) -> PyResult<Self> {
-        Self::new(
+        let exec_algorithm_params = exec_algorithm_params.map(str_hashmap_to_ustr);
+        Ok(Self::new(
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
+            order_side,
             quantity,
-            event_id,
-            ts_event.into(),
-            ts_init.into(),
-            reconciliation,
-            venue_order_id,
-            account_id,
             price,
             trigger_price,
+            trigger_type,
+            time_in_force,
+            expire_time.map(std::convert::Into::into),
+            post_only,
+            reduce_only,
+            quote_quantity,
+            display_qty,
+            emulation_trigger,
+            trigger_instrument_id,
+            contingency_type,
+            order_list_id,
+            linked_order_ids,
+            parent_order_id,
+            exec_algorithm_id,
+            exec_algorithm_params,
+            exec_spawn_id,
+            tags.map(|vec| vec.into_iter().map(|s| Ustr::from(s.as_str())).collect()),
+            init_id,
+            ts_init.into(),
         )
-        .map_err(to_pyvalue_err)
-    }
-
-    fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> Py<PyAny> {
-        match op {
-            CompareOp::Eq => self.eq(other).into_py(py),
-            CompareOp::Ne => self.ne(other).into_py(py),
-            _ => py.NotImplemented(),
-        }
-    }
-
-    fn __repr__(&self) -> String {
-        format!("{:?}", self)
-    }
-
-    fn __str__(&self) -> String {
-        self.to_string()
+        .unwrap())
     }
 
-    fn type_str(&self) -> &str {
-        stringify!(OrderUpdated)
+    #[getter]
+    #[pyo3(name = "order_type")]
+    fn py_order_type(&self) -> OrderType {
+        self.order_type
+    }
+
+    #[getter]
+    #[pyo3(name = "events")]
+    fn py_events(&self, py: Python<'_>) -> PyResult<Vec<PyObject>> {
+        self.events()
+            .into_iter()
+            .map(|event| order_event_to_pyobject(py, event.clone()))
+            .collect()
     }
 
     #[staticmethod]
-    #[pyo3(name = "from_dict")]
-    fn py_from_dict(py: Python<'_>, values: Py<PyDict>) -> PyResult<Self> {
-        from_dict_pyo3(py, values)
+    #[pyo3(name = "create")]
+    fn py_create(init: OrderInitialized) -> PyResult<Self> {
+        Ok(LimitIfTouchedOrder::from(init))
     }
 
-    #[pyo3(name = "to_dict")]
-    fn py_to_dict(&self, py: Python<'_>) -> PyResult<PyObject> {
-        let dict = PyDict::new(py);
-        dict.set_item("type", stringify!(OrderUpdated));
-        dict.set_item("trader_id", self.trader_id.to_string())?;
-        dict.set_item("strategy_id", self.strategy_id.to_string())?;
-        dict.set_item("instrument_id", self.instrument_id.to_string())?;
-        dict.set_item("client_order_id", self.client_order_id.to_string())?;
-        dict.set_item("quantity", self.quantity.to_string())?;
-        dict.set_item("event_id", self.event_id.to_string())?;
-        dict.set_item("ts_event", self.ts_event.as_u64())?;
-        dict.set_item("ts_init", self.ts_init.as_u64())?;
-        dict.set_item("reconciliation", self.reconciliation)?;
-        match self.venue_order_id {
-            Some(venue_order_id) => dict.set_item("venue_order_id", venue_order_id.to_string())?,
-            None => dict.set_item("venue_order_id", py.None())?,
-        }
-        match self.account_id {
-            Some(account_id) => dict.set_item("account_id", account_id.to_string())?,
-            None => dict.set_item("account_id", py.None())?,
-        }
-        match self.price {
-            Some(price) => dict.set_item("price", price.to_string())?,
-            None => dict.set_item("price", py.None())?,
-        }
-        match self.trigger_price {
-            Some(trigger_price) => dict.set_item("trigger_price", trigger_price.to_string())?,
-            None => dict.set_item("trigger_price", py.None())?,
-        }
-        Ok(dict.into())
+    #[pyo3(name = "apply")]
+    fn py_apply(&mut self, event: PyObject, py: Python<'_>) -> PyResult<()> {
+        let event_any = pyobject_to_order_event(py, event).unwrap();
+        self.apply(event_any).map(|_| ()).map_err(to_pyruntime_err)
     }
 }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/identifiers/instrument_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/instrument_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/identifiers/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/identifiers/trade_id.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/trade_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/crypto_future.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_future.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/currency_pair.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/currency_pair.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/equity.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/equity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/futures_contract.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_contract.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/futures_spread.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_spread.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/options_contract.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_contract.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/instruments/options_spread.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_spread.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/macros.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/macros.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orderbook/book.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/book.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orderbook/level.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/level.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orderbook/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/limit_if_touched.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs`

 * *Files 4% similar despite different names*

```diff
@@ -16,43 +16,46 @@
 use std::collections::HashMap;
 
 use nautilus_core::{python::to_pyruntime_err, uuid::UUID4};
 use pyo3::prelude::*;
 use ustr::Ustr;
 
 use crate::{
-    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TriggerType},
+    enums::{ContingencyType, OrderSide, OrderType, TimeInForce, TrailingOffsetType, TriggerType},
     events::order::initialized::OrderInitialized,
     identifiers::{
         client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
         instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
         trader_id::TraderId,
     },
     orders::{
         base::{str_hashmap_to_ustr, Order},
-        limit_if_touched::LimitIfTouchedOrder,
+        trailing_stop_limit::TrailingStopLimitOrder,
     },
     python::events::order::{order_event_to_pyobject, pyobject_to_order_event},
     types::{price::Price, quantity::Quantity},
 };
 
 #[pymethods]
-impl LimitIfTouchedOrder {
+impl TrailingStopLimitOrder {
     #[new]
     #[allow(clippy::too_many_arguments)]
     fn py_new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
         quantity: Quantity,
         price: Price,
         trigger_price: Price,
         trigger_type: TriggerType,
+        limit_offset: Price,
+        trailing_offset: Price,
+        trailing_offset_type: TrailingOffsetType,
         time_in_force: TimeInForce,
         post_only: bool,
         reduce_only: bool,
         quote_quantity: bool,
         init_id: UUID4,
         ts_init: u64,
         expire_time: Option<u64>,
@@ -75,14 +78,17 @@
             instrument_id,
             client_order_id,
             order_side,
             quantity,
             price,
             trigger_price,
             trigger_type,
+            limit_offset,
+            trailing_offset,
+            trailing_offset_type,
             time_in_force,
             expire_time.map(std::convert::Into::into),
             post_only,
             reduce_only,
             quote_quantity,
             display_qty,
             emulation_trigger,
@@ -115,15 +121,15 @@
             .map(|event| order_event_to_pyobject(py, event.clone()))
             .collect()
     }
 
     #[staticmethod]
     #[pyo3(name = "create")]
     fn py_create(init: OrderInitialized) -> PyResult<Self> {
-        Ok(LimitIfTouchedOrder::from(init))
+        Ok(TrailingStopLimitOrder::from(init))
     }
 
     #[pyo3(name = "apply")]
     fn py_apply(&mut self, event: PyObject, py: Python<'_>) -> PyResult<()> {
         let event_any = pyobject_to_order_event(py, event).unwrap();
         self.apply(event_any).map(|_| ()).map_err(to_pyruntime_err)
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/market.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/market_if_touched.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_if_touched.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/market_to_limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_to_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/stop_limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/stop_market.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs`

 * *Files 13% similar despite different names*

```diff
@@ -25,39 +25,36 @@
     identifiers::{
         client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
         instrument_id::InstrumentId, order_list_id::OrderListId, strategy_id::StrategyId,
         trader_id::TraderId,
     },
     orders::{
         base::{str_hashmap_to_ustr, Order},
-        trailing_stop_limit::TrailingStopLimitOrder,
+        trailing_stop_market::TrailingStopMarketOrder,
     },
     python::events::order::{order_event_to_pyobject, pyobject_to_order_event},
     types::{price::Price, quantity::Quantity},
 };
 
 #[pymethods]
-impl TrailingStopLimitOrder {
+impl TrailingStopMarketOrder {
     #[new]
     #[allow(clippy::too_many_arguments)]
     fn py_new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
         quantity: Quantity,
-        price: Price,
         trigger_price: Price,
         trigger_type: TriggerType,
-        limit_offset: Price,
         trailing_offset: Price,
         trailing_offset_type: TrailingOffsetType,
         time_in_force: TimeInForce,
-        post_only: bool,
         reduce_only: bool,
         quote_quantity: bool,
         init_id: UUID4,
         ts_init: u64,
         expire_time: Option<u64>,
         display_qty: Option<Quantity>,
         emulation_trigger: Option<TriggerType>,
@@ -75,23 +72,20 @@
         Ok(Self::new(
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
             order_side,
             quantity,
-            price,
             trigger_price,
             trigger_type,
-            limit_offset,
             trailing_offset,
             trailing_offset_type,
             time_in_force,
             expire_time.map(std::convert::Into::into),
-            post_only,
             reduce_only,
             quote_quantity,
             display_qty,
             emulation_trigger,
             trigger_instrument_id,
             contingency_type,
             order_list_id,
@@ -121,15 +115,15 @@
             .map(|event| order_event_to_pyobject(py, event.clone()))
             .collect()
     }
 
     #[staticmethod]
     #[pyo3(name = "create")]
     fn py_create(init: OrderInitialized) -> PyResult<Self> {
-        Ok(TrailingStopLimitOrder::from(init))
+        Ok(TrailingStopMarketOrder::from(init))
     }
 
     #[pyo3(name = "apply")]
     fn py_apply(&mut self, event: PyObject, py: Python<'_>) -> PyResult<()> {
         let event_any = pyobject_to_order_event(py, event).unwrap();
         self.apply(event_any).map(|_| ()).map_err(to_pyruntime_err)
     }
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/position.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/position.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/types/balance.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/balance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/types/currency.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/currency.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/types/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/types/money.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/money.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/types/price.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/price.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/python/types/quantity.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/quantity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/stubs.rs`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,17 @@
         None,
         None,
         None,
         Some(Price::from("1.0002")),
         None,
         None,
         None,
-    );
+        None,
+    )
+    .unwrap();
     Position::new(audusd_sim, order_filled).unwrap()
 }
 
 #[fixture]
 pub fn test_position_short(audusd_sim: CurrencyPair) -> Position {
     let order = TestOrderStubs::market_order(
         audusd_sim.id,
@@ -94,15 +96,17 @@
         None,
         None,
         None,
         Some(Price::from("22000.0")),
         None,
         None,
         None,
-    );
+        None,
+    )
+    .unwrap();
     Position::new(audusd_sim, order_filled).unwrap()
 }
 
 #[must_use]
 pub fn stub_order_book_mbp_appl_xnas() -> OrderBook {
     stub_order_book_mbp(
         InstrumentId::from("AAPL.XNAS"),
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/balance.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/balance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/currency.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/currency.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/fixed.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/fixed.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/money.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/money.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/price.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/price.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/quantity.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/quantity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/types/stubs.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/types/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/model/src/venues.rs` & `nautilus_trader-1.193.0/nautilus_core/model/src/venues.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/network/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/benches/test_client.rs` & `nautilus_trader-1.193.0/nautilus_core/network/benches/test_client.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/benches/test_server.rs` & `nautilus_trader-1.193.0/nautilus_core/network/benches/test_server.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/http.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/http.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/clock.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/gcra.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/gcra.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/nanos.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/nanos.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/ratelimiter/quota.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/quota.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/socket.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/socket.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/src/websocket.rs` & `nautilus_trader-1.193.0/nautilus_core/network/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/LICENSE` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/README.md` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/compat.rs` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/compat.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/connect.rs` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/connect.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/stream.rs` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/stream.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/network/tokio-tungstenite/src/tls.rs` & `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/tls.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/persistence/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/benches/bench_persistence.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/benches/bench_persistence.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/bar.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/delta.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/depth.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/quote.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/arrow/trade.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/backend/kmerge_batch.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/kmerge_batch.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/backend/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/backend/session.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/session.rs`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         };
         self.runtime.block_on(self.session_ctx.register_parquet(
             table_name,
             file_path,
             parquet_options,
         ))?;
 
-        let default_query = format!("SELECT * FROM {}", &table_name);
+        let default_query = format!("SELECT * FROM {} ORDER BY ts_init", &table_name);
         let sql_query = sql_query.unwrap_or(&default_query);
         let query = self.runtime.block_on(self.session_ctx.sql(sql_query))?;
 
         let batch_stream = self.runtime.block_on(query.execute_stream())?;
 
         self.add_batch_stream::<T>(batch_stream);
         Ok(())
```

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/backend/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/backend/session.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/session.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/backend/transformer.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/transformer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/bar.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/delta.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/mod.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/quote.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/src/python/wranglers/trade.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/tests/test_catalog.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_catalog.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/persistence/tests/test_util.rs` & `nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_util.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/pyo3/Cargo.toml` & `nautilus_trader-1.193.0/nautilus_core/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_core/pyo3/src/lib.rs` & `nautilus_trader-1.193.0/nautilus_core/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/betting.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/betting.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/cash.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/cash.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/margin.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/accounts/margin.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/calculators.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/calculators.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/error.py` & `nautilus_trader-1.193.0/nautilus_trader/accounting/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/factory.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/factory.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/manager.pxd` & `nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/accounting/manager.pyx` & `nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/_template/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/_template/core.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/core.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/_template/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/_template/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/_template/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/common.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/config.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/constants.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/data_types.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data_types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/factories.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/orderbook.pxd` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/orderbook.pyx` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/common.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/core.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/core.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/requests.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/requests.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/parsing/streaming.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/streaming.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/betfair/sockets.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/sockets.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/constants.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/credentials.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/credentials.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/schemas/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/symbol.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/symbol.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/types.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/common/urls.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/urls.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/config.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/factories.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/http/wallet.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/futures/types.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/endpoint.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/endpoint.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/error.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/http/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/http/wallet.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/websocket/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/binance/websocket/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/constants.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/credentials.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/credentials.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/error.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/parsing.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/parsing.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/symbol.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/symbol.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/common/urls.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/urls.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/config.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/factories.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/asset.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/asset.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/errors.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/errors.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/market.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/http/user.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/account/balance.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/balance.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/common.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/instrument.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/instrument.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/kline.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/kline.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/market/trades.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/trades.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/position.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/position.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/trade.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/trade.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/schemas/ws.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/ws.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/websocket/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/bybit/websocket/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/common.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/config.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/constants.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/factories.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/loaders.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/loaders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/publishers.json` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/publishers.json`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/databento/types.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/env.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/env.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/account.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/common.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/connection.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/connection.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/contract.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/contract.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/error.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/order.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/common.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/config.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,22 +291,28 @@
         price = (
             None if ib_order.lmtPrice == UNSET_DOUBLE else instrument.make_price(ib_order.lmtPrice)
         )
         expire_time = (
             timestring_to_timestamp(ib_order.goodTillDate) if ib_order.tif == "GTD" else None
         )
 
-        # TODO: Testing for advanced Open orders
+        mapped_order_type_info = ib_to_nautilus_order_type[ib_order.orderType]
+        if isinstance(mapped_order_type_info, tuple):
+            order_type, time_in_force = mapped_order_type_info
+        else:
+            order_type = mapped_order_type_info
+            time_in_force = ib_to_nautilus_time_in_force[ib_order.tif]
+
         order_status = OrderStatusReport(
             account_id=self.account_id,
             instrument_id=instrument.id,
             venue_order_id=VenueOrderId(str(ib_order.orderId)),
             order_side=ib_to_nautilus_order_side[ib_order.action],
-            order_type=ib_to_nautilus_order_type[ib_order.orderType],
-            time_in_force=ib_to_nautilus_time_in_force[ib_order.tif],
+            order_type=order_type,
+            time_in_force=time_in_force,
             order_status=order_status,
             quantity=total_qty,
             filled_qty=Quantity.from_int(0),
             avg_px=Decimal(0),
             report_id=UUID4(),
             ts_accepted=ts_init,
             ts_last=ts_init,
@@ -494,17 +500,21 @@
             self._log.debug(f"Received {position_status!r}")
             report.append(position_status)
 
         return report
 
     def _transform_order_to_ib_order(self, order: Order) -> IBOrder:
         ib_order = IBOrder()
+        time_in_force = order.time_in_force
         for key, field, fn in MAP_ORDER_FIELDS:
             if value := getattr(order, key, None):
-                setattr(ib_order, field, fn(value))
+                if key == "order_type" and time_in_force == TimeInForce.AT_THE_CLOSE:
+                    setattr(ib_order, field, fn((value, time_in_force)))
+                else:
+                    setattr(ib_order, field, fn(value))
 
         if self._cache.instrument(order.instrument_id).is_inverse:
             ib_order.cashQty = int(ib_order.totalQuantity)
             ib_order.totalQuantity = 0
 
         if isinstance(order, TrailingStopLimitOrder | TrailingStopMarketOrder):
             ib_order.auxPrice = float(order.trailing_offset)
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/factories.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/gateway.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/gateway.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/historic/client.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,16 @@
 
         timestamps = [unix_nanos_to_dt(tick.ts_event) for tick in ticks]
         min_timestamp = min(timestamps)
         max_timestamp = max(timestamps)
 
         if min_timestamp.floor("S") == max_timestamp.floor("S"):
             max_timestamp = max_timestamp.floor("S") + pd.Timedelta(seconds=1)
-
+        if len(ticks) <= 50:
+            max_timestamp = max_timestamp.floor("S") + pd.Timedelta(minutes=1)
         if max_timestamp >= end_date_time:
             return None, False
 
         return max_timestamp, True
 
     async def _fetch_instruments_if_not_cached(self, contracts: list[IBContract]) -> None:
         """
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,38 +36,41 @@
 
 MAP_TIME_IN_FORCE: dict[int, str] = {
     TimeInForce.DAY: "DAY",
     TimeInForce.GTC: "GTC",
     TimeInForce.IOC: "IOC",
     TimeInForce.GTD: "GTD",
     TimeInForce.AT_THE_OPEN: "OPG",
+    TimeInForce.AT_THE_CLOSE: "DAY",
     TimeInForce.FOK: "FOK",
     # unsupported: 'DTC',
 }
 
 MAP_ORDER_ACTION: dict[int, str] = {
     OrderSide.BUY: "BUY",
     OrderSide.SELL: "SELL",
 }
 
 ORDER_SIDE_TO_ORDER_ACTION: dict[str, str] = {
     "BOT": "BUY",
     "SLD": "SELL",
 }
 
-MAP_ORDER_TYPE: dict[int, str] = {
+MAP_ORDER_TYPE: dict[int | tuple[int, int], str] = {
     OrderType.LIMIT: "LMT",
     OrderType.LIMIT_IF_TOUCHED: "LIT",
     OrderType.MARKET: "MKT",
     OrderType.MARKET_IF_TOUCHED: "MIT",
     OrderType.MARKET_TO_LIMIT: "MTL",
     OrderType.STOP_LIMIT: "STP LMT",
     OrderType.STOP_MARKET: "STP",
     OrderType.TRAILING_STOP_LIMIT: "TRAIL LIMIT",
     OrderType.TRAILING_STOP_MARKET: "TRAIL",
+    (OrderType.MARKET, TimeInForce.AT_THE_CLOSE): "MOC",
+    (OrderType.LIMIT, TimeInForce.AT_THE_CLOSE): "LOC",
 }
 
 
 MAP_ORDER_FIELDS: set[tuple[str, str, Callable]] = {
     # ref: (nautilus_order_field, ib_order_field, value_fn)
     ("client_order_id", "orderRef", lambda x: x.value),
     ("display_qty", "displaySize", lambda x: x.as_double()),
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/interactive_brokers/web.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/web.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/config.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pxd`

 * *Files 21% similar despite different names*

```diff
@@ -9,31 +9,21 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.config import LiveExecClientConfig
+from cpython.datetime cimport datetime
 
+from nautilus_trader.indicators.base.indicator cimport Indicator
 
-class SandboxExecutionClientConfig(LiveExecClientConfig, frozen=True, kw_only=True):
-    """
-    Configuration for ``SandboxExecClient`` instances.
-
-    Parameters
-    ----------
-    venue : str
-        The venue to generate a sandbox execution client for
-    currency: str
-        The currency for this venue
-    balance : int
-        The starting balance for this venue
-    bar_execution: bool
-        If bars should be processed by the matching engine(s) (and move the market).
-
-    """
-
-    venue: str
-    currency: str
-    balance: int
-    bar_execution: bool = True
+
+cdef class VolumeWeightedAveragePrice(Indicator):
+    cdef int _day
+    cdef double _price_volume
+    cdef double _volume_total
+
+    cdef readonly double value
+    """The current value.\n\n:returns: `double`"""
+
+    cpdef void update_raw(self, double price, double volume, datetime timestamp)
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import asyncio
-from decimal import Decimal
 from typing import ClassVar
 
 import pandas as pd
 
+from nautilus_trader.adapters.sandbox.config import SandboxExecutionClientConfig
 from nautilus_trader.backtest.exchange import SimulatedExchange
 from nautilus_trader.backtest.execution_client import BacktestExecClient
 from nautilus_trader.backtest.models import FillModel
 from nautilus_trader.backtest.models import LatencyModel
 from nautilus_trader.backtest.models import MakerTakerFeeModel
 from nautilus_trader.cache.cache import Cache
 from nautilus_trader.common.component import LiveClock
@@ -35,23 +35,23 @@
 from nautilus_trader.execution.reports import PositionStatusReport
 from nautilus_trader.live.execution_client import LiveExecutionClient
 from nautilus_trader.model.data import Bar
 from nautilus_trader.model.data import OrderBookDelta
 from nautilus_trader.model.data import OrderBookDeltas
 from nautilus_trader.model.data import QuoteTick
 from nautilus_trader.model.data import TradeTick
-from nautilus_trader.model.enums import AccountType
-from nautilus_trader.model.enums import OmsType
+from nautilus_trader.model.enums import account_type_from_str
+from nautilus_trader.model.enums import book_type_from_str
+from nautilus_trader.model.enums import oms_type_from_str
 from nautilus_trader.model.identifiers import ClientId
 from nautilus_trader.model.identifiers import ClientOrderId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Venue
 from nautilus_trader.model.identifiers import VenueOrderId
 from nautilus_trader.model.instruments import Instrument
-from nautilus_trader.model.objects import AccountBalance
 from nautilus_trader.model.objects import Currency
 from nautilus_trader.model.objects import Money
 from nautilus_trader.portfolio.base import PortfolioFacade
 
 
 class SandboxExecutionClient(LiveExecutionClient):
     """
@@ -77,65 +77,67 @@
     def __init__(
         self,
         loop: asyncio.AbstractEventLoop,
         portfolio: PortfolioFacade,
         msgbus: MessageBus,
         cache: Cache,
         clock: LiveClock,
-        venue: str,
-        currency: str,
-        balance: int,
-        oms_type: OmsType = OmsType.NETTING,
-        account_type: AccountType = AccountType.MARGIN,
-        default_leverage: Decimal = Decimal(10),
-        bar_execution: bool = True,
+        config: SandboxExecutionClientConfig,
     ) -> None:
-        self._currency = Currency.from_str(currency)
-        money = Money(value=balance, currency=self._currency)
-        self.balance = AccountBalance(total=money, locked=Money(0, money.currency), free=money)
+        sandbox_venue = Venue(config.venue)
+        oms_type = oms_type_from_str(config.oms_type)
+        account_type = account_type_from_str(config.account_type)
+        base_currency = Currency.from_str(config.base_currency) if config.base_currency else None
+
         self.test_clock = TestClock()
-        self._account_type = account_type
-        sandbox_venue = Venue(venue)
+
         super().__init__(
             loop=loop,
-            client_id=ClientId(venue),
+            client_id=ClientId(config.venue),
             venue=sandbox_venue,
             oms_type=oms_type,
             account_type=account_type,
-            base_currency=self._currency,
+            base_currency=base_currency,
             instrument_provider=InstrumentProvider(),
             msgbus=msgbus,
             cache=cache,
             clock=clock,
             config=None,
         )
         self.exchange = SimulatedExchange(
             venue=sandbox_venue,
             oms_type=oms_type,
-            account_type=self._account_type,
-            base_currency=self._currency,
-            starting_balances=[self.balance.free],
-            default_leverage=default_leverage,
-            leverages={},
+            account_type=account_type,
+            starting_balances=[Money.from_str(b) for b in config.starting_balances],
+            base_currency=base_currency,
+            default_leverage=config.default_leverage,
+            leverages=config.leverages or {},
             instruments=self.INSTRUMENTS,
             modules=[],
             portfolio=portfolio,
             msgbus=self._msgbus,
             cache=cache,
+            clock=self.test_clock,
             fill_model=FillModel(),
             fee_model=MakerTakerFeeModel(),
             latency_model=LatencyModel(0),
-            clock=self.test_clock,
-            bar_execution=bar_execution,
-            frozen_account=True,  # <-- Freezing account
+            book_type=book_type_from_str(config.book_type),
+            frozen_account=config.frozen_account,
+            bar_execution=config.bar_execution,
+            reject_stop_orders=config.reject_stop_orders,
+            support_gtd_orders=config.support_gtd_orders,
+            support_contingent_orders=config.support_contingent_orders,
+            use_position_ids=config.use_position_ids,
+            use_random_ids=config.use_random_ids,
+            use_reduce_only=config.use_reduce_only,
         )
         self._client = BacktestExecClient(
             exchange=self.exchange,
             msgbus=msgbus,
-            cache=self._cache,
+            cache=cache,
             clock=self.test_clock,
         )
         self.exchange.register_client(self._client)
         self.exchange.initialize_account()
 
     def connect(self) -> None:
         """
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/sandbox/factory.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,35 +44,32 @@
 
         Parameters
         ----------
         loop : asyncio.AbstractEventLoop
             The event loop for the client.
         name : str
             The custom client ID.
-        config : dict[str, object]
-            The configuration for the client.
         portfolio : PortfolioFacade
             The read-only portfolio for the client.
         msgbus : MessageBus
             The message bus for the client.
         cache : Cache
             The cache for the client.
         clock : LiveClock
             The clock for the client.
+        config : dict[str, object]
+            The configuration for the client.
 
         Returns
         -------
         SandboxExecutionClient
 
         """
         exec_client = SandboxExecutionClient(
             loop=loop,
             clock=clock,
             portfolio=portfolio,
             msgbus=msgbus,
             cache=cache,
-            venue=name or config.venue,
-            balance=config.balance,
-            currency=config.currency,
-            bar_execution=config.bar_execution,
+            config=config,
         )
         return exec_client
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/tardis/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/adapters/tardis/loaders.py` & `nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/loaders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/analyzer.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/reporter.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/reporter.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistic.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistic.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/expectancy.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/expectancy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/long_ratio.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/long_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/loser_avg.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/loser_max.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_max.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/loser_min.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_min.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/profit_factor.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/profit_factor.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_avg.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_avg_loss.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_loss.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_avg_win.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_win.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/returns_volatility.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_volatility.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/risk_return_ratio.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/risk_return_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/sharpe_ratio.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sharpe_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/sortino_ratio.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sortino_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/win_rate.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/win_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/winner_avg.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/winner_max.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_max.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/analysis/statistics/winner_min.py` & `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_min.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/__main__.py` & `nautilus_trader-1.193.0/nautilus_trader/backtest/__main__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/auction.py` & `nautilus_trader-1.193.0/nautilus_trader/backtest/auction.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/config.py` & `nautilus_trader-1.193.0/nautilus_trader/backtest/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/data_client.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/data_client.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/engine.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/engine.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/exchange.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/exchange.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/execution_client.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/execution_client.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/matching_engine.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/matching_engine.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/models.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/models.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/models.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/models.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/modules.pxd` & `nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/modules.pyx` & `nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/node.py` & `nautilus_trader-1.193.0/nautilus_trader/backtest/node.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/backtest/results.py` & `nautilus_trader-1.193.0/nautilus_trader/backtest/results.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/cache/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/cache/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/cache/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/cache.pxd` & `nautilus_trader-1.193.0/nautilus_trader/cache/cache.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/cache.pyx` & `nautilus_trader-1.193.0/nautilus_trader/cache/cache.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/config.py` & `nautilus_trader-1.193.0/nautilus_trader/cache/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/database.pxd` & `nautilus_trader-1.193.0/nautilus_trader/cache/database.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/database.pyx` & `nautilus_trader-1.193.0/nautilus_trader/cache/database.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/facade.pxd` & `nautilus_trader-1.193.0/nautilus_trader/cache/facade.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/facade.pyx` & `nautilus_trader-1.193.0/nautilus_trader/cache/facade.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/postgres/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/cache/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/cache/postgres/adapter.py` & `nautilus_trader-1.193.0/nautilus_trader/cache/postgres/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,18 @@
         instrument_pyo3 = self._backing.load_instrument(instrument_id_pyo3)
         return transform_instrument_from_pyo3(instrument_pyo3)
 
     def add_order(self, order: Order):
         order_pyo3 = transform_order_to_pyo3(order)
         self._backing.add_order(order_pyo3)
 
+    def update_order(self, order: Order):
+        order_pyo3 = transform_order_to_pyo3(order)
+        self._backing.update_order(order_pyo3)
+
     def load_order(self, client_order_id: ClientOrderId):
         order_id_pyo3 = nautilus_pyo3.ClientOrderId.from_str(str(client_order_id))
         order_pyo3 = self._backing.load_order(order_id_pyo3)
         if order_pyo3:
             return transform_order_from_pyo3(order_pyo3)
         return None
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/common/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/actor.pxd` & `nautilus_trader-1.193.0/nautilus_trader/common/actor.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/actor.pyx` & `nautilus_trader-1.193.0/nautilus_trader/common/actor.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/component.pxd` & `nautilus_trader-1.193.0/nautilus_trader/common/component.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/component.pyx` & `nautilus_trader-1.193.0/nautilus_trader/common/component.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/config.py` & `nautilus_trader-1.193.0/nautilus_trader/common/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/executor.py` & `nautilus_trader-1.193.0/nautilus_trader/common/executor.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/factories.pxd` & `nautilus_trader-1.193.0/nautilus_trader/common/factories.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/factories.pyx` & `nautilus_trader-1.193.0/nautilus_trader/common/factories.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/functions.py` & `nautilus_trader-1.193.0/nautilus_trader/common/functions.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/generators.pxd` & `nautilus_trader-1.193.0/nautilus_trader/common/generators.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/generators.pyx` & `nautilus_trader-1.193.0/nautilus_trader/common/generators.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/messages.pxd` & `nautilus_trader-1.193.0/nautilus_trader/common/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/messages.pyx` & `nautilus_trader-1.193.0/nautilus_trader/common/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/common/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/common/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/config/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/asynchronous.py` & `nautilus_trader-1.193.0/nautilus_trader/core/asynchronous.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/correctness.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/correctness.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/correctness.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/correctness.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/data.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/data.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/data.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/data.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/datetime.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/datetime.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/datetime.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/datetime.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/fsm.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/fsm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/fsm.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/fsm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/includes/algorithms.h` & `nautilus_trader-1.193.0/nautilus_trader/core/includes/algorithms.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/includes/backtest.h` & `nautilus_trader-1.193.0/nautilus_trader/core/includes/backtest.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/includes/common.h` & `nautilus_trader-1.193.0/nautilus_trader/core/includes/common.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/includes/core.h` & `nautilus_trader-1.193.0/nautilus_trader/core/includes/core.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/includes/model.h` & `nautilus_trader-1.193.0/nautilus_trader/core/includes/model.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/inspect.py` & `nautilus_trader-1.193.0/nautilus_trader/core/inspect.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/message.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/message.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/message.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/message.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/nautilus_pyo3.pyi` & `nautilus_trader-1.193.0/nautilus_trader/core/nautilus_pyo3.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -707,15 +707,15 @@
     NOT_HALTED = "NOT_HALTED"
     GENERAL = "GENERAL"
     VOLATILITY = "VOLATILITY"
 
 class OmsType(Enum):
     UNSPECIFIED = "UNSPECIFIED"
     NETTING = "NETTING"
-    HEDGING = "HEDGIN"
+    HEDGING = "HEDGING"
 
 class OptionKind(Enum):
     CALL = "CALL"
     PUT = "PUT"
 
 class OrderSide(Enum):
     NO_ORDER_SIDE = "NO_ORDER_SIDE"
@@ -2290,14 +2290,15 @@
         database: str | None = None,
     )-> PostgresCacheDatabase: ...
     def load(self) -> dict[str,str]: ...
     def add(self, key: str, value: bytes) -> None: ...
     def add_currency(self,currency: Currency) -> None: ...
     def add_instrument(self, instrument: object) -> None: ...
     def add_order(self, instrument: object) -> None: ...
+    def update_order(self, order: object) -> None: ...
     def load_currency(self, code: str) -> Currency | None: ...
     def load_currencies(self) -> list[Currency]: ...
     def load_instrument(self, instrument_id: InstrumentId) -> Instrument | None: ...
     def load_instruments(self) -> list[Instrument]: ...
     def load_order(self, order_id: ClientOrderId) -> Order | None: ...
     def flush_db(self) -> None: ...
     def truncate(self, table: str) -> None: ...
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/algorithms.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/algorithms.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/backtest.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/backtest.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/common.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/common.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/core.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/core.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/model.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/rust/model.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/stats.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/stats.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/stats.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/stats.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/string.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/string.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/uuid.pxd` & `nautilus_trader-1.193.0/nautilus_trader/core/uuid.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/core/uuid.pyx` & `nautilus_trader-1.193.0/nautilus_trader/core/uuid.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/aggregation.pxd` & `nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/aggregation.pyx` & `nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/client.pxd` & `nautilus_trader-1.193.0/nautilus_trader/data/client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/client.pyx` & `nautilus_trader-1.193.0/nautilus_trader/data/client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/config.py` & `nautilus_trader-1.193.0/nautilus_trader/data/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/engine.pxd` & `nautilus_trader-1.193.0/nautilus_trader/data/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/engine.pyx` & `nautilus_trader-1.193.0/nautilus_trader/data/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/messages.pxd` & `nautilus_trader-1.193.0/nautilus_trader/data/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/data/messages.pyx` & `nautilus_trader-1.193.0/nautilus_trader/data/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/algorithms/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/algorithms/blank.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/blank.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/algorithms/twap.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/twap.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/blank.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/blank.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_bracket.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_long_only.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_long_only.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/ema_cross_twap.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_twap.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/market_maker.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/market_maker.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/orderbook_imbalance.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 import datetime
 from decimal import Decimal
 
 from nautilus_trader.config import NonNegativeFloat
 from nautilus_trader.config import PositiveFloat
 from nautilus_trader.config import StrategyConfig
 from nautilus_trader.core import nautilus_pyo3
-from nautilus_trader.core.nautilus_pyo3 import BookImbalanceRatio
 from nautilus_trader.core.rust.common import LogColor
 from nautilus_trader.model.book import OrderBook
 from nautilus_trader.model.data import QuoteTick
-from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.enums import book_type_from_str
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.trading.strategy import Strategy
 
@@ -99,33 +97,33 @@
         self.trigger_min_size = config.trigger_min_size
         self.trigger_imbalance_ratio = config.trigger_imbalance_ratio
         self.min_seconds_between_triggers = config.min_seconds_between_triggers
         self._last_trigger_timestamp: datetime.datetime | None = None
         self.instrument: Instrument | None = None
         if self.config.use_quote_ticks:
             assert self.config.book_type == "L1_MBP"
-        self.book_type: BookType = book_type_from_str(self.config.book_type)
+        self.book_type: nautilus_pyo3.BookType = nautilus_pyo3.BookType(self.config.book_type)
 
         # We need to initialize the Rust pyo3 objects
         pyo3_instrument_id = nautilus_pyo3.InstrumentId.from_str(self.instrument_id.value)
         self.book = nautilus_pyo3.OrderBook(self.book_type, pyo3_instrument_id)
-        self.imbalance = BookImbalanceRatio()
+        self.imbalance = nautilus_pyo3.BookImbalanceRatio()
 
     def on_start(self) -> None:
         """
         Actions to be performed on strategy start.
         """
         self.instrument = self.cache.instrument(self.instrument_id)
         if self.instrument is None:
             self.log.error(f"Could not find instrument for {self.instrument_id}")
             self.stop()
             return
 
         if self.config.use_quote_ticks:
-            self.book_type = BookType.L1_MBP
+            self.book_type = nautilus_pyo3.BookType.L1_MBP
             self.subscribe_quote_ticks(self.instrument.id)
         else:
             self.book_type = book_type_from_str(self.config.book_type)
             self.subscribe_order_book_deltas(
                 self.instrument.id,
                 self.book_type,
                 managed=False,  # <-- Manually applying deltas to book
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/signal_strategy.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/signal_strategy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/subscribe.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/subscribe.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/talib_strategy.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/talib_strategy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/examples/strategies/volatility_market_maker.py` & `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/volatility_market_maker.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/algorithm.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/algorithm.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/client.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/client.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/config.py` & `nautilus_trader-1.193.0/nautilus_trader/execution/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/emulator.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/emulator.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/engine.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/engine.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/manager.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/manager.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/manager.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/manager.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/matching_core.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/matching_core.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/messages.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/messages.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/reports.py` & `nautilus_trader-1.193.0/nautilus_trader/execution/reports.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/trailing.pxd` & `nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/execution/trailing.pyx` & `nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/amat.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/amat.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/aroon.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/aroon.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/atr.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/atr.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/ama.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/ama.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/dema.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/dema.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/ema.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/ema.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/hma.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/hma.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/ma_factory.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ma_factory.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/moving_average.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/moving_average.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/rma.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/rma.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/sma.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/sma.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/vidya.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/vidya.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/wma.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/average/wma.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/base/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/base/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/base/indicator.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/base/indicator.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/bias.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/bias.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/bollinger_bands.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/bollinger_bands.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/cci.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/cci.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/cmo.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/cmo.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/dm.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/dm.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/donchian_channel.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/donchian_channel.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/efficiency_ratio.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/efficiency_ratio.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enum.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enum.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_channel.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_channel.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_position.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/keltner_position.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/kvo.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/kvo.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/linear_regression.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/linear_regression.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/macd.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/macd.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/obv.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/obv.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/pressure.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/pressure.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/psl.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/psl.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/roc.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/roc.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/rsi.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/rsi.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/rvi.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/rvi.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/spread_analyzer.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/spread_analyzer.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/stochastics.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/stochastics.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/swings.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/swings.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/ta_lib/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/ta_lib/common.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/ta_lib/manager.py` & `nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/manager.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/vhf.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/vhf.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/volatility_ratio.pxd` & `nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/volatility_ratio.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/vwap.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from cpython.datetime cimport datetime
+cimport numpy as np
 
-from nautilus_trader.indicators.base.indicator cimport Indicator
+from nautilus_trader.model.objects cimport Price
+from nautilus_trader.model.tick_scheme.base cimport TickScheme
 
 
-cdef class VolumeWeightedAveragePrice(Indicator):
-    cdef int _day
-    cdef double _price_volume
-    cdef double _volume_total
+cdef class TieredTickScheme(TickScheme):
+    cdef list tiers
+    cdef int max_ticks_per_tier
+    cdef int price_precision
+    cdef int tick_count
 
-    cdef readonly double value
-    """The current value.\n\n:returns: `double`"""
+    cdef readonly np.ndarray ticks
 
-    cpdef void update_raw(self, double price, double volume, datetime timestamp)
+    cpdef _build_ticks(self)
+
+    cpdef int find_tick_index(self, double value)
+    cpdef Price next_ask_price(self, double value, int n=*)
+    cpdef Price next_bid_price(self, double value, int n=*)
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/indicators/vwap.pyx` & `nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/live/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/__main__.py` & `nautilus_trader-1.193.0/nautilus_trader/live/__main__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/config.py` & `nautilus_trader-1.193.0/nautilus_trader/live/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/data_client.py` & `nautilus_trader-1.193.0/nautilus_trader/live/data_client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/data_engine.py` & `nautilus_trader-1.193.0/nautilus_trader/live/data_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/execution_client.py` & `nautilus_trader-1.193.0/nautilus_trader/live/execution_client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/execution_engine.py` & `nautilus_trader-1.193.0/nautilus_trader/live/execution_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/factories.py` & `nautilus_trader-1.193.0/nautilus_trader/live/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/node.py` & `nautilus_trader-1.193.0/nautilus_trader/live/node.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/node_builder.py` & `nautilus_trader-1.193.0/nautilus_trader/live/node_builder.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/live/risk_engine.py` & `nautilus_trader-1.193.0/nautilus_trader/live/risk_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/book.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/book.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/book.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/book.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/currencies.py` & `nautilus_trader-1.193.0/nautilus_trader/model/currencies.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/data.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/data.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/data.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/data.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/enums.py` & `nautilus_trader-1.193.0/nautilus_trader/model/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/account.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/events/account.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/account.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/events/account.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/order.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/events/order.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/order.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/events/order.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/position.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/events/position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/events/position.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/events/position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/functions.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/functions.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/functions.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/functions.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/identifiers.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/identifiers.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/betting.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/betting.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/cfd.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/cfd.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/commodity.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/commodity.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_future.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_future.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_perpetual.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/crypto_perpetual.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/currency_pair.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/currency_pair.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/equity.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/equity.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_contract.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_contract.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_spread.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/futures_spread.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_contract.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_contract.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_spread.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/options_spread.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/synthetic.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/instruments/synthetic.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/objects.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/objects.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/objects.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/objects.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/limit.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/limit.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/limit_if_touched.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/limit_if_touched.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/list.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/list.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/market.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/market.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/market_if_touched.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/market_if_touched.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/market_to_limit.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/market_to_limit.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_limit.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_limit.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_market.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/stop_market.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -335,18 +335,18 @@
             strategy_id=init.strategy_id,
             instrument_id=init.instrument_id,
             client_order_id=init.client_order_id,
             order_side=init.side,
             quantity=init.quantity,
             trigger_price=Price.from_str_c(init.options["trigger_price"]),
             trigger_type=trigger_type_from_str(init.options["trigger_type"]),
-            time_in_force=init.time_in_force,
-            expire_time_ns=init.options["expire_time_ns"],
             init_id=init.id,
             ts_init=init.ts_init,
+            time_in_force=init.time_in_force,
+            expire_time_ns=init.options["expire_time_ns"] if init.options["expire_time_ns"] is not None else 0,
             reduce_only=init.reduce_only,
             quote_quantity=init.quote_quantity,
             emulation_trigger=init.emulation_trigger,
             trigger_instrument_id=init.trigger_instrument_id,
             contingency_type=init.contingency_type,
             order_list_id=init.order_list_id,
             linked_order_ids=init.linked_order_ids,
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_limit.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_limit.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_market.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/trailing_stop_market.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/unpacker.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/orders/unpacker.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/position.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/position.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd` & `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-cimport numpy as np
+from __future__ import annotations
 
-from nautilus_trader.model.objects cimport Price
-from nautilus_trader.model.tick_scheme.base cimport TickScheme
+from dataclasses import dataclass
 
+from nautilus_trader.core.data import Data
+from nautilus_trader.model.identifiers import ClientId
+from nautilus_trader.model.instruments import Instrument
 
-cdef class TieredTickScheme(TickScheme):
-    cdef list tiers
-    cdef int max_ticks_per_tier
-    cdef int price_precision
-    cdef int tick_count
 
-    cdef readonly np.ndarray ticks
+@dataclass(frozen=True)
+class CatalogDataResult:
+    """
+    Represents a catalog data query result.
+    """
 
-    cpdef _build_ticks(self)
-
-    cpdef int find_tick_index(self, double value)
-    cpdef Price next_ask_price(self, double value, int n=*)
-    cpdef Price next_bid_price(self, double value, int n=*)
+    data_cls: type
+    data: list[Data]
+    instrument: Instrument | None = None
+    client_id: ClientId | None = None
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx` & `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/model/venues.py` & `nautilus_trader-1.193.0/nautilus_trader/model/venues.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/base.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/base.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/parquet.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/parquet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/singleton.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/singleton.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/catalog/types.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from __future__ import annotations
-
-from dataclasses import dataclass
-
-from nautilus_trader.core.data import Data
-from nautilus_trader.model.identifiers import ClientId
-from nautilus_trader.model.instruments import Instrument
-
-
-@dataclass(frozen=True)
-class CatalogDataResult:
-    """
-    Represents a catalog data query result.
-    """
-
-    data_cls: type
-    data: list[Data]
-    instrument: Instrument | None = None
-    client_id: ClientId | None = None
+from nautilus_trader.config import ActorConfig
+from nautilus_trader.examples.strategies.signal_strategy import SignalStrategy
+from nautilus_trader.examples.strategies.signal_strategy import SignalStrategyConfig
+from nautilus_trader.trading.controller import Controller
+
+
+class ControllerConfig(ActorConfig, frozen=True):
+    pass
+
+
+class MyController(Controller):
+    def start(self):
+        """
+        Dynamically add a new strategy after startup.
+        """
+        instruments = self.cache.instruments()
+        strategy_config = SignalStrategyConfig(instrument_id=instruments[0].id)
+        strategy = SignalStrategy(strategy_config)
+        self.create_strategy(strategy)
```

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/config.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/funcs.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/funcs.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/loaders.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/loaders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/wranglers.pxd` & `nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/wranglers.pyx` & `nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/wranglers_v2.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers_v2.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/persistence/writer.py` & `nautilus_trader-1.193.0/nautilus_trader/persistence/writer.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/portfolio/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/portfolio/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/portfolio/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/portfolio/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/portfolio/portfolio.pxd` & `nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/portfolio/portfolio.pyx` & `nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/risk/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/config.py` & `nautilus_trader-1.193.0/nautilus_trader/risk/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/engine.pxd` & `nautilus_trader-1.193.0/nautilus_trader/risk/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/engine.pyx` & `nautilus_trader-1.193.0/nautilus_trader/risk/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/sizing.pxd` & `nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/risk/sizing.pyx` & `nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/account_state.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/account_state.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/component_events.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/component_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/instruments.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/instruments.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/order_events.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/order_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/implementations/position_events.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/position_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/schema.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/arrow/serializer.py` & `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/serializer.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/base.pxd` & `nautilus_trader-1.193.0/nautilus_trader/serialization/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/base.pyx` & `nautilus_trader-1.193.0/nautilus_trader/serialization/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/serializer.pxd` & `nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/serialization/serializer.pyx` & `nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/system/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/system/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/system/config.py` & `nautilus_trader-1.193.0/nautilus_trader/system/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/system/kernel.py` & `nautilus_trader-1.193.0/nautilus_trader/system/kernel.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/functions.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/functions.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/actors.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/actors.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/cache_database.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/cache_database.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/data.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/engines.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/engines.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/exec_clients.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/exec_clients.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/mocks/strategies.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/strategies.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/providers.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/accounting_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/accounting_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/data_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/data_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/events_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/events_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/instruments_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/instruments_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/orders_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/orders_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/rust/types_pyo3.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/types_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/commands.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/commands.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/component.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/component.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/config.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/data.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/events.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/execution.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/identifiers.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/identifiers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/test_kit/stubs/persistence.py` & `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/persistence.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/__init__.pxd` & `nautilus_trader-1.193.0/nautilus_trader/trading/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/__init__.py` & `nautilus_trader-1.193.0/nautilus_trader/trading/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/config.py` & `nautilus_trader-1.193.0/nautilus_trader/trading/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/controller.py` & `nautilus_trader-1.193.0/nautilus_trader/trading/controller.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/filters.py` & `nautilus_trader-1.193.0/nautilus_trader/trading/filters.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/strategy.pxd` & `nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/strategy.pyx` & `nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/nautilus_trader/trading/trader.py` & `nautilus_trader-1.193.0/nautilus_trader/trading/trader.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.192.0/pyproject.toml` & `nautilus_trader-1.193.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautilus_trader"
-version = "1.192.0"
+version = "1.193.0"
 description = "A high-performance algorithmic trading platform and event-driven backtester"
 authors = ["Nautech Systems <info@nautechsystems.io>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://nautilustrader.io"
 repository = "https://github.com/nautechsystems/nautilus_trader"
 classifiers = [
@@ -55,22 +55,22 @@
 numpy = "^1.26.4"  # Build dependency
 toml = "^0.10.2"  # Build dependency
 click = "^8.1.7"
 fsspec = "==2023.6.0"  # Pinned due breaking changes
 msgspec = "^0.18.6"
 pandas = "^2.2.2"
 pyarrow = ">=16.1.0"
-pytz = ">=2023.4.0"
+pytz = ">=2024.1.0"
 tqdm = "^4.66.4"
 uvloop = {version = "^0.19.0", markers = "sys_platform != 'win32'"}
 
 async-timeout = {version = "^4.0.3", optional = true}
 betfair_parser = {version = "==0.12.0", optional = true}  # Pinned for stability
 defusedxml = {version = "^0.7.1", optional = true}
-docker = {version = "^7.0.0", optional = true}
+docker = {version = "^7.1.0", optional = true}
 nautilus_ibapi = {version = "==10.19.2", optional = true}  # Pinned for stability
 
 [tool.poetry.extras]
 betfair = ["betfair_parser"]
 docker = ["docker"]
 ib = ["nautilus_ibapi", "async-timeout", "defusedxml"]
 
@@ -79,15 +79,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 docformatter = "^1.7.5"
 mypy = "^1.10.0"
 pandas-stubs = "^2.2.2"
 pre-commit = "^3.7.1"
-ruff = "^0.4.4"
+ruff = "^0.4.5"
 types-pytz = "^2023.3"
 types-requests = "^2.31"
 types-toml = "^0.10.2"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `nautilus_trader-1.192.0/PKG-INFO` & `nautilus_trader-1.193.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus_trader
-Version: 1.192.0
+Version: 1.193.0
 Summary: A high-performance algorithmic trading platform and event-driven backtester
 Home-page: https://nautilustrader.io
 License: LGPL-3.0-or-later
 Author: Nautech Systems
 Author-email: info@nautechsystems.io
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -26,22 +26,22 @@
 Provides-Extra: docker
 Provides-Extra: ib
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; extra == "ib"
 Requires-Dist: betfair_parser (==0.12.0) ; extra == "betfair"
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cython (==3.0.10)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0) ; extra == "ib"
-Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "docker"
+Requires-Dist: docker (>=7.1.0,<8.0.0) ; extra == "docker"
 Requires-Dist: fsspec (==2023.6.0)
 Requires-Dist: msgspec (>=0.18.6,<0.19.0)
 Requires-Dist: nautilus_ibapi (==10.19.2) ; extra == "ib"
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pyarrow (>=16.1.0)
-Requires-Dist: pytz (>=2023.4.0)
+Requires-Dist: pytz (>=2024.1.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Requires-Dist: uvloop (>=0.19.0,<0.20.0) ; sys_platform != "win32"
 Project-URL: Repository, https://github.com/nautechsystems/nautilus_trader
 Description-Content-Type: text/markdown
 
 # <img src="https://github.com/nautechsystems/nautilus_trader/blob/develop/docs/_images/nautilus-trader-logo.png" width="500">
@@ -58,15 +58,14 @@
 | `master`  | ![version](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnautechsystems%2Fnautilus_trader%2Fmaster%2Fversion.json)  | [![build](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml)  |
 | `nightly` | ![version](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnautechsystems%2Fnautilus_trader%2Fnightly%2Fversion.json) | [![build](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml/badge.svg?branch=nightly)](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml) |
 | `develop` | ![version](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnautechsystems%2Fnautilus_trader%2Fdevelop%2Fversion.json) | [![build](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml/badge.svg?branch=develop)](https://github.com/nautechsystems/nautilus_trader/actions/workflows/build.yml) |
 
 | Platform           | Rust    | Python |
 | :----------------- | :------ | :----- |
 | `Linux (x86_64)`   | 1.78.0+ | 3.10+  |
-| `macOS (x86_64)`   | 1.78.0+ | 3.10+  |
 | `macOS (arm64)`    | 1.78.0+ | 3.10+  |
 | `Windows (x86_64)` | 1.78.0+ | 3.10+  |
 
 - **Website:** https://nautilustrader.io
 - **Docs:** https://docs.nautilustrader.io
 - **Support:** [support@nautilustrader.io](mailto:support@nautilustrader.io)
```

