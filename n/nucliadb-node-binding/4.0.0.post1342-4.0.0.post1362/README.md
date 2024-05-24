# Comparing `tmp/nucliadb_node_binding-4.0.0.post1342.tar.gz` & `tmp/nucliadb_node_binding-4.0.0.post1362.tar.gz`

## Comparing `nucliadb_node_binding-4.0.0.post1342.tar` & `nucliadb_node_binding-4.0.0.post1362.tar`

### file list

```diff
@@ -1,349 +1,349 @@
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43324 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18147 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    19055 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1496 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    11343 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13965 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2300 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12999 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3394 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2489 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      332 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8294 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11334 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    19577 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1553 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13111 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14260 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11809 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    15700 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11202 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/indexes.rs
--rw-r--r--   0     1001      127    10055 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1168 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    28646 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    27248 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     7048 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/tests.rs
--rw-r--r--   0     1001      127     1890 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10199 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8386 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     9372 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     2508 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
--rw-r--r--   0     1001      127     6862 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5554 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0     1001      127     5337 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127     2484 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/config.rs
--rw-r--r--   0     1001      127    12340 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24377 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    15068 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1741 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14194 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2513 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127     8419 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2607 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    23110 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     7189 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2264 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127      940 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    18009 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15340 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2933 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10092 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3435 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2152 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3523 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    43269 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17239 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     7990 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9523 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2340 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127     8473 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/audit.rs
--rw-r--r--   0     1001      127    46350 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127    13228 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1271 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    95906 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    17860 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    62254 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    24308 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    50492 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127    10160 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     3063 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     5462 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2944 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2023 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8450 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2557 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     5683 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/Cargo.toml
--rw-r--r--   0     1001      127     1017 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/.cargo/config.toml
--rw-r--r--   0     1001      127     1553 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/Makefile
--rw-r--r--   0     1001      127       52 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/README.md
--rwxr-xr-x   0     1001      127      978 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/cov.sh
--rw-r--r--   0     1001      127     1642 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/audit.proto
--rw-r--r--   0     1001      127     1938 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/dataset.proto
--rw-r--r--   0     1001      127     4424 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/knowledgebox.proto
--rw-r--r--   0     1001      127      129 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/migrations.proto
--rw-r--r--   0     1001      127    10792 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/nodereader.proto
--rw-r--r--   0     1001      127     4554 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/noderesources.proto
--rw-r--r--   0     1001      127     2907 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/nodewriter.proto
--rw-r--r--   0     1001      127       13 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/.gitignore
--rw-r--r--   0     1001      127      106 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/MANIFEST.in
--rw-r--r--   0     1001      127       93 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/README.rst
--rw-r--r--   0     1001      127        0 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/__init__.py
--rw-r--r--   0     1001      127     5729 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/audit_pb2.py
--rw-r--r--   0     1001      127    11478 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi
--rw-r--r--   0     1001      127     5708 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py
--rw-r--r--   0     1001      127    14374 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi
--rw-r--r--   0     1001      127    13093 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py
--rw-r--r--   0     1001      127    30463 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi
--rw-r--r--   0     1001      127     1152 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py
--rw-r--r--   0     1001      127      844 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi
--rw-r--r--   0     1001      127    22792 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py
--rw-r--r--   0     1001      127    60294 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi
--rw-r--r--   0     1001      127    27532 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py
--rw-r--r--   0     1001      127    12923 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi
--rw-r--r--   0     1001      127    14299 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py
--rw-r--r--   0     1001      127    35337 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi
--rw-r--r--   0     1001      127     7995 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py
--rw-r--r--   0     1001      127    13432 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi
--rw-r--r--   0     1001      127    20793 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py
--rw-r--r--   0     1001      127     9143 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/py.typed
--rw-r--r--   0     1001      127     5175 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2.py
--rw-r--r--   0     1001      127     9274 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi
--rw-r--r--   0     1001      127     6379 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py
--rw-r--r--   0     1001      127     3969 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi
--rw-r--r--   0     1001      127    35561 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/resources_pb2.py
--rw-r--r--   0     1001      127    95697 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi
--rw-r--r--   0     1001      127     2192 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py
--rw-r--r--   0     1001      127     2533 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi
--rw-r--r--   0     1001      127     4407 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py
--rw-r--r--   0     1001      127     2145 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi
--rw-r--r--   0     1001      127    12447 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2.py
--rw-r--r--   0     1001      127    28142 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi
--rw-r--r--   0     1001      127    13970 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py
--rw-r--r--   0     1001      127    11812 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi
--rw-r--r--   0     1001      127     6683 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/utils_pb2.py
--rw-r--r--   0     1001      127    18303 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi
--rw-r--r--   0     1001      127    32011 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2.py
--rw-r--r--   0     1001      127    78244 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi
--rw-r--r--   0     1001      127    39118 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py
--rw-r--r--   0     1001      127    20858 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi
--rw-r--r--   0     1001      127       96 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/setup.cfg
--rw-r--r--   0     1001      127      761 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/setup.py
--rw-r--r--   0     1001      127      708 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/reader.proto
--rw-r--r--   0     1001      127     1863 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/replication.proto
--rw-r--r--   0     1001      127    12098 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/resources.proto
--rw-r--r--   0     1001      127      558 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/standalone.proto
--rw-r--r--   0     1001      127     3469 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/train.proto
--rw-r--r--   0     1001      127     2301 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/utils.proto
--rw-r--r--   0     1001      127    12100 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/writer.proto
--rw-r--r--   0     1001      127     1461 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1621 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/src/update.rs
--rw-r--r--   0     1001      127    12085 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-05-23 08:58:52.000000 nucliadb_node_binding-4.0.0.post1342/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1342/PKG-INFO
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    43269 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17239 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    19055 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1496 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    11343 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13965 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2300 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12999 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3394 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2489 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      332 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8294 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11334 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    19577 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1553 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13111 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14260 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11563 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    15700 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11202 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/indexes.rs
+-rw-r--r--   0     1001      127    10055 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1168 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    28646 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    27248 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     7048 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/tests.rs
+-rw-r--r--   0     1001      127     1890 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10199 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8386 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     9372 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     2508 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
+-rw-r--r--   0     1001      127     6862 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5554 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0     1001      127     5337 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2340 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127     8473 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/audit.rs
+-rw-r--r--   0     1001      127    46350 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127    13228 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1271 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    95906 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    17860 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    62254 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    24308 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    50492 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127    10160 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     7990 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9523 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10092 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3435 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2152 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3523 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127     2484 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/config.rs
+-rw-r--r--   0     1001      127    12340 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24377 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    15068 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1741 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14194 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2513 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127     8419 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2607 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    23110 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     7189 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127    10472 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2264 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127      940 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    18009 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15340 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2933 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43324 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18147 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     3063 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     5462 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2944 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2023 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8450 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2557 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     5683 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/Cargo.toml
+-rw-r--r--   0     1001      127     1017 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/.cargo/config.toml
+-rw-r--r--   0     1001      127     1553 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/Makefile
+-rw-r--r--   0     1001      127       52 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/README.md
+-rwxr-xr-x   0     1001      127      978 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/cov.sh
+-rw-r--r--   0     1001      127     1642 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/audit.proto
+-rw-r--r--   0     1001      127     1938 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/dataset.proto
+-rw-r--r--   0     1001      127     4424 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/knowledgebox.proto
+-rw-r--r--   0     1001      127      129 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/migrations.proto
+-rw-r--r--   0     1001      127    10792 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/nodereader.proto
+-rw-r--r--   0     1001      127     4554 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/noderesources.proto
+-rw-r--r--   0     1001      127     2907 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/nodewriter.proto
+-rw-r--r--   0     1001      127       13 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/.gitignore
+-rw-r--r--   0     1001      127      106 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/MANIFEST.in
+-rw-r--r--   0     1001      127       93 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/README.rst
+-rw-r--r--   0     1001      127        0 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/__init__.py
+-rw-r--r--   0     1001      127     5729 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/audit_pb2.py
+-rw-r--r--   0     1001      127    11478 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi
+-rw-r--r--   0     1001      127     5708 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py
+-rw-r--r--   0     1001      127    14374 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi
+-rw-r--r--   0     1001      127    13093 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py
+-rw-r--r--   0     1001      127    30463 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi
+-rw-r--r--   0     1001      127     1152 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py
+-rw-r--r--   0     1001      127      844 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi
+-rw-r--r--   0     1001      127    22792 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py
+-rw-r--r--   0     1001      127    60294 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi
+-rw-r--r--   0     1001      127    27532 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py
+-rw-r--r--   0     1001      127    12923 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    14299 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py
+-rw-r--r--   0     1001      127    35337 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi
+-rw-r--r--   0     1001      127     7995 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py
+-rw-r--r--   0     1001      127    13432 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi
+-rw-r--r--   0     1001      127    20793 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py
+-rw-r--r--   0     1001      127     9143 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/py.typed
+-rw-r--r--   0     1001      127     5175 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2.py
+-rw-r--r--   0     1001      127     9274 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi
+-rw-r--r--   0     1001      127     6379 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py
+-rw-r--r--   0     1001      127     3969 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    35561 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/resources_pb2.py
+-rw-r--r--   0     1001      127    95697 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi
+-rw-r--r--   0     1001      127     2192 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py
+-rw-r--r--   0     1001      127     2533 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi
+-rw-r--r--   0     1001      127     4407 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py
+-rw-r--r--   0     1001      127     2145 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    12447 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2.py
+-rw-r--r--   0     1001      127    28142 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi
+-rw-r--r--   0     1001      127    13970 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py
+-rw-r--r--   0     1001      127    11812 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi
+-rw-r--r--   0     1001      127     6683 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/utils_pb2.py
+-rw-r--r--   0     1001      127    18303 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi
+-rw-r--r--   0     1001      127    32011 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2.py
+-rw-r--r--   0     1001      127    78244 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi
+-rw-r--r--   0     1001      127    39118 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py
+-rw-r--r--   0     1001      127    20858 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi
+-rw-r--r--   0     1001      127       96 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/setup.cfg
+-rw-r--r--   0     1001      127      761 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/setup.py
+-rw-r--r--   0     1001      127      708 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/reader.proto
+-rw-r--r--   0     1001      127     1863 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/replication.proto
+-rw-r--r--   0     1001      127    12098 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/resources.proto
+-rw-r--r--   0     1001      127      558 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/standalone.proto
+-rw-r--r--   0     1001      127     3469 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/train.proto
+-rw-r--r--   0     1001      127     2301 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/utils.proto
+-rw-r--r--   0     1001      127    12100 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/writer.proto
+-rw-r--r--   0     1001      127     1461 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1621 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/src/update.rs
+-rw-r--r--   0     1001      127    12085 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-05-24 07:50:19.000000 nucliadb_node_binding-4.0.0.post1362/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.0.post1362/PKG-INFO
```

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 use std::collections::HashMap;
 use std::path::{Path, PathBuf};
 use std::sync::Arc;
 
 use nucliadb_core::protos::ReleaseChannel;
 use nucliadb_core::tantivy_replica::TantivyReplicaState;
 use nucliadb_core::tracing::{debug, error, info, warn};
-use nucliadb_core::{node_error, IndexFiles, NodeResult, RawReplicaState};
+use nucliadb_core::{IndexFiles, NodeResult, RawReplicaState};
 use nucliadb_protos::{noderesources, replication};
 use tokio::fs::File;
 use tokio::io::AsyncReadExt;
 use tokio_stream::wrappers::ReceiverStream;
 use tonic::Response;
 
 use crate::cache::ShardWriterCache;
@@ -51,27 +51,20 @@
             node_id,
         }
     }
 }
 
 async fn stream_file(
     chunk_size: u64,
-    shard_path: &Path,
     generation_id: &str,
     rel_filepath: &Path,
     file: std::fs::File,
     sender: &tokio::sync::mpsc::Sender<Result<replication::ReplicateShardResponse, tonic::Status>>,
 ) -> NodeResult<()> {
-    let filepath = shard_path.join(rel_filepath);
-
-    if !filepath.exists() {
-        return Err(node_error!("This file can not be streamed because it does not exist"));
-    }
-
-    debug!("Streaming file {}", filepath.to_string_lossy());
+    debug!("Streaming file {}", rel_filepath.to_string_lossy());
     let mut total = 0;
     let mut chunk = 1;
     let mut file = File::from_std(file);
     let filesize = file.metadata().await?.len();
 
     loop {
         let vec_size = min(chunk_size, filesize - total);
@@ -123,15 +116,15 @@
     chunk_size: u64,
     shard_path: &Path,
     generation_id: &str,
     _index_prefix: PathBuf,
     sender: &tokio::sync::mpsc::Sender<Result<replication::ReplicateShardResponse, tonic::Status>>,
 ) -> NodeResult<()> {
     for (segment_path, segment_file) in replica_state.files {
-        stream_file(chunk_size, shard_path, generation_id, &PathBuf::from(segment_path), segment_file, sender).await?;
+        stream_file(chunk_size, generation_id, &PathBuf::from(segment_path), segment_file, sender).await?;
     }
     for (metadata_file, data) in replica_state.metadata_files {
         stream_data(shard_path, generation_id, &PathBuf::from(metadata_file), data, sender).await?;
     }
     Ok(())
 }
 
@@ -142,15 +135,15 @@
     generation_id: &str,
     index_prefix: PathBuf,
     sender: &tokio::sync::mpsc::Sender<Result<replication::ReplicateShardResponse, tonic::Status>>,
 ) -> NodeResult<()> {
     let metadata_bytes = replica_state.metadata_as_bytes();
 
     for (rel_path, segment_file) in replica_state.files {
-        stream_file(chunk_size, shard_path, generation_id, &index_prefix.join(rel_path), segment_file, sender).await?;
+        stream_file(chunk_size, generation_id, &index_prefix.join(rel_path), segment_file, sender).await?;
     }
 
     stream_data(shard_path, generation_id, &index_prefix.join(&replica_state.metadata_path), metadata_bytes, sender)
         .await?;
     Ok(())
 }
 
@@ -180,15 +173,15 @@
             }
         };
     }
 
     // top level additional files
     for filename in ["metadata.json", "versions.json", "indexes.json"] {
         let file = std::fs::File::open(shard_path.join(filename))?;
-        stream_file(chunk_size, &shard_path, generation_id, &PathBuf::from(filename), file, &sender).await?;
+        stream_file(chunk_size, generation_id, &PathBuf::from(filename), file, &sender).await?;
     }
     Ok(())
 }
 
 #[tonic::async_trait]
 impl replication::replication_service_server::ReplicationService for ReplicationServiceGRPCDriver {
     type ReplicateShardStream = ReceiverStream<Result<replication::ReplicateShardResponse, tonic::Status>>;
```

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/indexes.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/indexes.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/tests.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_node/tests/test_vectorsets.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_node/tests/test_vectorsets.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/config.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/config.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/audit.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/audit.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-4.0.0.post1362/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/Cargo.toml` & `nucliadb_node_binding-4.0.0.post1362/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "4.0.0-post1342"
+version = "4.0.0-post1362"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-4.0.0.post1342/.cargo/config.toml` & `nucliadb_node_binding-4.0.0.post1362/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/CHANGELOG.md` & `nucliadb_node_binding-4.0.0.post1362/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/Makefile` & `nucliadb_node_binding-4.0.0.post1362/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/cov.sh` & `nucliadb_node_binding-4.0.0.post1362/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/audit.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/audit.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/dataset.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/dataset.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/knowledgebox.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/knowledgebox.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/nodereader.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/nodereader.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/noderesources.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/noderesources.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/nodewriter.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/nodewriter.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/audit_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/resources_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/utils_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/python/setup.py` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/python/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/reader.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/reader.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/replication.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/replication.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/resources.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/resources.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/standalone.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/standalone.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/train.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/train.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/utils.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/utils.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/nucliadb_protos/writer.proto` & `nucliadb_node_binding-4.0.0.post1362/nucliadb_protos/writer.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/pyproject.toml` & `nucliadb_node_binding-4.0.0.post1362/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/src/collect_garbage.rs` & `nucliadb_node_binding-4.0.0.post1362/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/src/errors.rs` & `nucliadb_node_binding-4.0.0.post1362/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/src/lib.rs` & `nucliadb_node_binding-4.0.0.post1362/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/src/reader.rs` & `nucliadb_node_binding-4.0.0.post1362/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/src/update.rs` & `nucliadb_node_binding-4.0.0.post1362/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/src/writer.rs` & `nucliadb_node_binding-4.0.0.post1362/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/tests/__init__.py` & `nucliadb_node_binding-4.0.0.post1362/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/tests/conftest.py` & `nucliadb_node_binding-4.0.0.post1362/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.0.post1342/tests/integration/test_indexing.py` & `nucliadb_node_binding-4.0.0.post1362/tests/integration/test_indexing.py`

 * *Files identical despite different names*

