# Comparing `tmp/faststream-0.5.7.tar.gz` & `tmp/faststream-0.5.8.tar.gz`

## Comparing `faststream-0.5.7.tar` & `faststream-0.5.8.tar`

### file list

```diff
@@ -1,341 +1,352 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.7/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.7/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.7/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.7/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.7/SECURITY.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/security.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/types.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/message.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20122 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/security.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    65013 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/opentelemetry/__init__.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/opentelemetry/middleware.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10542 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/message.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/parser.py
--rw-r--r--   0        0        0    22411 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/security.py
--rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    29093 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    72613 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   118913 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/opentelemetry/__init__.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/opentelemetry/middleware.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/message.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/parser.py
--rw-r--r--   0        0        0    12421 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/security.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27010 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/opentelemetry/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/opentelemetry/middleware.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/consts.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/middleware.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/provider.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    21894 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    31096 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/opentelemetry/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/opentelemetry/middleware.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/message.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/parser.py
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/security.py
--rw-r--r--   0        0        0     7003 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/opentelemetry/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/opentelemetry/middleware.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21342 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/testing/app.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.7/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.7/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.7/README.md
--rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 faststream-0.5.7/pyproject.toml
--rw-r--r--   0        0        0    23654 2020-02-02 00:00:00.000000 faststream-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.8/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.8/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.8/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.8/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.8/SECURITY.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/security.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/types.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13590 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    68318 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0   102616 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/factory.py
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    23352 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/security.py
+-rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    76258 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   120064 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/factory.py
+-rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/log/logging.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/annotations.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/message.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/parser.py
+-rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/security.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36834 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/__init__.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/bucket_declarer.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/obj_storage_declarer.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/object_builder.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/kv_watch.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/obj_watch.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     9767 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/factory.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/subscription.py
+-rw-r--r--   0        0        0    31761 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/consts.py
+-rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/provider.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    21894 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    31321 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/factory.py
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/message.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/security.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27863 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/factory.py
+-rw-r--r--   0        0        0    21757 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/testing/app.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.8/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.8/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.8/README.md
+-rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 faststream-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0    23801 2020-02-02 00:00:00.000000 faststream-0.5.8/PKG-INFO
```

### Comparing `faststream-0.5.7/.pre-commit-config.yaml` & `faststream-0.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.secrets.baseline` & `faststream-0.5.8/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/CITATION.cff` & `faststream-0.5.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/CODE_OF_CONDUCT.md` & `faststream-0.5.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/CONTRIBUTING.md` & `faststream-0.5.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/SECURITY.md` & `faststream-0.5.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.8/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/dependabot.yml` & `faststream-0.5.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.8/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/codeql.yml` & `faststream-0.5.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/dependency-review.yaml` & `faststream-0.5.8/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/deploy-docs.yaml` & `faststream-0.5.8/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/publish_coverage.yml` & `faststream-0.5.8/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/publish_pypi.yml` & `faststream-0.5.8/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/test.yaml` & `faststream-0.5.8/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/.github/workflows/update_release_notes.yaml` & `faststream-0.5.8/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e02_1_basic_publisher.py` & `faststream-0.5.8/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e02_2_basic_publisher.py` & `faststream-0.5.8/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e02_3_basic_publisher.py` & `faststream-0.5.8/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e03_miltiple_pubsub.py` & `faststream-0.5.8/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e04_msg_filter.py` & `faststream-0.5.8/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e07_ack_immediately.py` & `faststream-0.5.8/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e09_testing_mocks.py` & `faststream-0.5.8/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e10_middlewares.py` & `faststream-0.5.8/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/e11_settings.py` & `faststream-0.5.8/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/fastapi_integration/testing.py` & `faststream-0.5.8/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/howto/structlogs.py` & `faststream-0.5.8/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/kafka/testing.py` & `faststream-0.5.8/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/nats/e03_publisher.py` & `faststream-0.5.8/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/nats/e04_js_basic.py` & `faststream-0.5.8/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/nats/e05_basic_and_js.py` & `faststream-0.5.8/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/rabbit/direct.py` & `faststream-0.5.8/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/rabbit/fanout.py` & `faststream-0.5.8/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/rabbit/header.py` & `faststream-0.5.8/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/rabbit/topic.py` & `faststream-0.5.8/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/redis/channel_sub_pattern.py` & `faststream-0.5.8/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/redis/rpc.py` & `faststream-0.5.8/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/router/basic_publish.py` & `faststream-0.5.8/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/serialization/avro/avro.py` & `faststream-0.5.8/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/serialization/msgpack/pack.py` & `faststream-0.5.8/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.8/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/__init__.py` & `faststream-0.5.8/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/_compat.py` & `faststream-0.5.8/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/app.py` & `faststream-0.5.8/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/exceptions.py` & `faststream-0.5.8/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/security.py` & `faststream-0.5.8/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/types.py` & `faststream-0.5.8/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/abc.py` & `faststream-0.5.8/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/generate.py` & `faststream-0.5.8/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/message.py` & `faststream-0.5.8/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/proto.py` & `faststream-0.5.8/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/site.py` & `faststream-0.5.8/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/utils.py` & `faststream-0.5.8/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.8/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/channels.py` & `faststream-0.5.8/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/info.py` & `faststream-0.5.8/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/main.py` & `faststream-0.5.8/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/message.py` & `faststream-0.5.8/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/operations.py` & `faststream-0.5.8/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/security.py` & `faststream-0.5.8/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/servers.py` & `faststream-0.5.8/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/utils.py` & `faststream-0.5.8/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.8/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.8/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.8/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.8/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.8/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.8/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.8/faststream/broker/acknowledgement_watcher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/message.py` & `faststream-0.5.8/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/router.py` & `faststream-0.5.8/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/schemas.py` & `faststream-0.5.8/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/types.py` & `faststream-0.5.8/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/utils.py` & `faststream-0.5.8/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/core/abc.py` & `faststream-0.5.8/faststream/broker/core/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/core/logging.py` & `faststream-0.5.8/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/core/usecase.py` & `faststream-0.5.8/faststream/broker/core/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         self.running = False
         self.graceful_timeout = graceful_timeout
 
         self._connection_kwargs = connection_kwargs
         self._connection = None
         self._producer = None
 
+        # TODO: remove useless middleware filter
         if not is_test_env():
             self._middlewares = (
                 CriticalLogMiddleware(self.logger, log_level),
                 *self._middlewares,
             )
 
         # TODO: move this context to Handlers' extra_context to support multiple brokers
```

### Comparing `faststream-0.5.7/faststream/broker/fastapi/context.py` & `faststream-0.5.8/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.8/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/fastapi/route.py` & `faststream-0.5.8/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/fastapi/router.py` & `faststream-0.5.8/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/middlewares/base.py` & `faststream-0.5.8/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/middlewares/logging.py` & `faststream-0.5.8/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/publisher/fake.py` & `faststream-0.5.8/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/publisher/proto.py` & `faststream-0.5.8/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/publisher/usecase.py` & `faststream-0.5.8/faststream/broker/publisher/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing_extensions import Annotated, Doc, override
 
 from faststream.asyncapi.abc import AsyncAPIOperation
 from faststream.asyncapi.message import get_response_schema
 from faststream.asyncapi.utils import to_camelcase
 from faststream.broker.publisher.proto import PublisherProto
 from faststream.broker.types import (
-    BrokerMiddleware,
     MsgType,
     P_HandlerParams,
     T_HandlerReturn,
 )
 from faststream.broker.wrapper.call import HandlerCallWrapper
 
 if TYPE_CHECKING:
```

### Comparing `faststream-0.5.7/faststream/broker/subscriber/call_item.py` & `faststream-0.5.8/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/subscriber/proto.py` & `faststream-0.5.8/faststream/broker/subscriber/proto.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,14 @@
     _broker_dependencies: Iterable["Depends"]
     _broker_middlewares: Iterable["BrokerMiddleware[MsgType]"]
     _producer: Optional["ProducerProto"]
 
     @abstractmethod
     def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None: ...
 
-    @staticmethod
-    @abstractmethod
-    def create() -> "SubscriberProto[MsgType]":
-        """Abstract factory to create a real Subscriber."""
-        ...
-
     @abstractmethod
     def get_log_context(
         self,
         msg: Optional["StreamMessage[MsgType]"],
         /,
     ) -> Dict[str, str]: ...
```

### Comparing `faststream-0.5.7/faststream/broker/subscriber/usecase.py` & `faststream-0.5.8/faststream/broker/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 )
 
 from typing_extensions import Self, override
 
 from faststream.asyncapi.abc import AsyncAPIOperation
 from faststream.asyncapi.message import parse_handler_params
 from faststream.asyncapi.utils import to_camelcase
-from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.subscriber.call_item import HandlerItem
 from faststream.broker.subscriber.proto import SubscriberProto
 from faststream.broker.types import (
     MsgType,
     P_HandlerParams,
     T_HandlerReturn,
 )
@@ -36,14 +35,15 @@
 from faststream.utils.functions import sync_fake_context, to_async
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.middlewares import BaseMiddleware
+    from faststream.broker.publisher.proto import BasePublisherProto, ProducerProto
     from faststream.broker.types import (
         AsyncCallable,
         BrokerMiddleware,
         CustomCallable,
         Filter,
         SubscriberMiddleware,
     )
@@ -89,14 +89,15 @@
     _broker_dependencies: Iterable["Depends"]
     _call_options: Optional["_CallOptions"]
 
     def __init__(
         self,
         *,
         no_ack: bool,
+        no_reply: bool,
         retry: Union[bool, int],
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
         # AsyncAPI information
         title_: Optional[str],
@@ -104,14 +105,15 @@
         include_in_schema: bool,
     ) -> None:
         """Initialize a new instance of the class."""
         self.calls = []
 
         self._default_parser = default_parser
         self._default_decoder = default_decoder
+        self._no_reply = no_reply
         # Watcher args
         self._no_ack = no_ack
         self._retry = retry
 
         self._call_options = None
         self.running = False
         self.lock = sync_fake_context()
@@ -135,15 +137,15 @@
         self._broker_middlewares = (*self._broker_middlewares, middleware)
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         logger: Optional["LoggerProto"],
-        producer: Optional[ProducerProto],
+        producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
         extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
@@ -334,15 +336,15 @@
                     result_msg = await h.call(
                         message=message,
                         # consumer middlewares
                         _extra_middlewares=(m.consume_scope for m in middlewares),
                     )
 
                     for p in chain(
-                        self._make_response_publisher(message),
+                        self.__get_reponse_publisher(message),
                         h.handler._publishers,
                     ):
                         await p.publish(
                             result_msg,
                             correlation_id=message.correlation_id,
                             # publisher middlewares
                             _extra_middlewares=(m.publish_scope for m in middlewares),
@@ -354,14 +356,24 @@
             for m in middlewares:
                 stack.push_async_exit(m.__aexit__)
 
             raise AssertionError(f"There is no suitable handler for {msg=}")
 
         return None
 
+    def __get_reponse_publisher(
+        self,
+        message: "StreamMessage[MsgType]",
+    ) -> Iterable["BasePublisherProto"]:
+        if not message.reply_to or self._no_reply:
+            return ()
+
+        else:
+            return self._make_response_publisher(message)
+
     def get_log_context(
         self,
         message: Optional["StreamMessage[MsgType]"],
     ) -> Dict[str, str]:
         """Generate log context."""
         return {
             "message_id": getattr(message, "message_id", ""),
```

### Comparing `faststream-0.5.7/faststream/broker/wrapper/call.py` & `faststream-0.5.8/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/broker/wrapper/proto.py` & `faststream-0.5.8/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/main.py` & `faststream-0.5.8/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/docs/app.py` & `faststream-0.5.8/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/supervisors/basereload.py` & `faststream-0.5.8/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.8/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/supervisors/utils.py` & `faststream-0.5.8/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.8/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/utils/imports.py` & `faststream-0.5.8/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/utils/logs.py` & `faststream-0.5.8/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/cli/utils/parser.py` & `faststream-0.5.8/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/annotations.py` & `faststream-0.5.8/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/client.py` & `faststream-0.5.8/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/message.py` & `faststream-0.5.8/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/parser.py` & `faststream-0.5.8/faststream/confluent/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """A class to parse Kafka messages."""
 
     @staticmethod
     async def parse_message(
         message: "Message",
     ) -> "StreamMessage[Message]":
         """Parses a Kafka message."""
-        headers = _parse_msg_headers(message.headers())
+        headers = _parse_msg_headers(message.headers() or ())
 
         body = message.value()
         offset = message.offset()
         _, timestamp = message.timestamp()
 
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
 
@@ -49,15 +49,15 @@
         batch_headers: List[Dict[str, str]] = []
 
         first = message[0]
         last = message[-1]
 
         for m in message:
             body.append(m.value())
-            batch_headers.append(_parse_msg_headers(m.headers()))
+            batch_headers.append(_parse_msg_headers(m.headers() or ()))
 
         headers = next(iter(batch_headers), {})
 
         _, first_timestamp = first.timestamp()
 
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
```

### Comparing `faststream-0.5.7/faststream/confluent/router.py` & `faststream-0.5.8/faststream/kafka/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,35 @@
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
+from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
-from faststream.confluent.broker.registrator import KafkaRegistrator
+from faststream.kafka.broker.registrator import KafkaRegistrator
 
 if TYPE_CHECKING:
-    from confluent_kafka import Message
+    from aiokafka import ConsumerRecord, TopicPartition
+    from aiokafka.abc import ConsumerRebalanceListener
+    from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
-    from faststream.confluent.message import KafkaMessage
+    from faststream.kafka.message import KafkaMessage
     from faststream.types import SendableMessage
 
 
 class KafkaPublisher(ArgsContainer):
     """Delayed KafkaPublisher registration object.
 
     Just a copy of `KafkaRegistrator.publisher(...)` arguments.
@@ -44,30 +47,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -121,41 +128,50 @@
             description=description,
             schema=schema,
             include_in_schema=include_in_schema,
         )
 
 
 class KafkaRoute(SubscriberRoute):
-    """Class to store delaied KafkaBroker subscriber registration."""
+    """Class to store delayed KafkaBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
             Union[
                 Callable[..., "SendableMessage"],
                 Callable[..., Awaitable["SendableMessage"]],
             ],
-            Doc("Message handler function."),
+            Doc(
+                "Message handler function "
+                "to wrap the same with `@broker.subscriber(...)` way."
+            ),
         ],
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         publishers: Annotated[
             Iterable[KafkaPublisher],
             Doc("Kafka publishers to broadcast the handler result."),
         ] = (),
+        batch: Annotated[
+            bool,
+            Doc("Whether to consume messages in batches or not."),
+        ] = False,
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -163,180 +179,213 @@
         value_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
-        fetch_max_wait_ms: Annotated[
-            int,
-            Doc("""
-            The maximum amount of time in milliseconds
-            the server will block before answering the fetch request if
-            there isn't sufficient data to immediately satisfy the
-            requirement given by `fetch_min_bytes`.
-            """),
-        ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
+        fetch_max_wait_ms: Annotated[
+            int,
+            Doc(
+                """
+            The maximum amount of time in milliseconds
+            the server will block before answering the fetch request if
+            there isn't sufficient data to immediately satisfy the
+            requirement given by `fetch_min_bytes`.
+            """
+            ),
+        ] = 500,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[str],
-            Doc("""
+            Sequence["AbstractPartitionAssignor"],
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
-        ] = ("roundrobin",),
+            """
+            ),
+        ] = (RoundRobinPartitionAssignor,),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -352,41 +401,84 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
-        batch: Annotated[
-            bool,
-            Doc("Whether to consume messages in batches or not."),
-        ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc(
+                """
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """
+            ),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc(
+                """
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """
+            ),
+        ] = None,
+        partitions: Annotated[
+            Optional[Iterable["TopicPartition"]],
+            Doc(
+                """
+            A topic and partition tuple. You can't use 'topics' and 'partitions' in the same time.
+            """
+            ),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
-            Doc("Parser to map original **Message** object to FastStream one."),
+            Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware[KafkaMessage]"],
@@ -407,14 +499,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -451,36 +549,40 @@
             consumer_timeout_ms=consumer_timeout_ms,
             max_poll_records=max_poll_records,
             exclude_internal_topics=exclude_internal_topics,
             isolation_level=isolation_level,
             max_records=max_records,
             batch_timeout_ms=batch_timeout_ms,
             batch=batch,
+            listener=listener,
+            pattern=pattern,
+            partitions=partitions,
             # basic args
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
+            no_reply=no_reply,
             # AsyncAPI args
             title=title,
             description=description,
             include_in_schema=include_in_schema,
             # FastDepends args
             retry=retry,
             no_ack=no_ack,
         )
 
 
 class KafkaRouter(
     KafkaRegistrator,
     BrokerRouter[
         Union[
-            "Message",
-            Tuple["Message", ...],
+            "ConsumerRecord",
+            Tuple["ConsumerRecord", ...],
         ]
     ],
 ):
     """Includable to KafkaBroker router."""
 
     def __init__(
         self,
@@ -498,23 +600,23 @@
             Doc(
                 "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
         ] = (),
         middlewares: Annotated[
             Iterable[
                 Union[
-                    "BrokerMiddleware[Message]",
-                    "BrokerMiddleware[Tuple[Message, ...]]",
+                    "BrokerMiddleware[ConsumerRecord]",
+                    "BrokerMiddleware[Tuple[ConsumerRecord, ...]]",
                 ]
             ],
             Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
-            Doc("Parser to map original **Message** object to FastStream one."),
+            Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
             Optional[bool],
```

### Comparing `faststream-0.5.7/faststream/confluent/security.py` & `faststream-0.5.8/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/testing.py` & `faststream-0.5.8/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/broker/broker.py` & `faststream-0.5.8/faststream/confluent/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/broker/logging.py` & `faststream-0.5.8/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/broker/registrator.py` & `faststream-0.5.8/faststream/confluent/broker/registrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
 from faststream.confluent.publisher.asyncapi import AsyncAPIPublisher
-from faststream.confluent.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.confluent.subscriber.factory import create_subscriber
 from faststream.exceptions import SetupError
 
 if TYPE_CHECKING:
     from confluent_kafka import Message
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
@@ -62,20 +62,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -85,178 +87,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -272,28 +307,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             Literal[True],
             Doc("Whether to consume messages in batches or not."),
         ],
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -327,14 +365,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -354,20 +398,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -377,178 +423,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -564,28 +643,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             Literal[False],
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -619,14 +701,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -646,20 +734,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -669,178 +759,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -856,28 +979,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -911,14 +1037,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -941,20 +1073,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -964,178 +1098,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -1151,28 +1318,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -1206,14 +1376,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -1230,15 +1406,15 @@
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
     ]:
         if not auto_commit and not group_id:
             raise SetupError("You should install `group_id` with manual commit mode")
 
         subscriber = super().subscriber(
-            AsyncAPISubscriber.create(
+            create_subscriber(
                 *topics,
                 batch=batch,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
                 connection_data={
                     "key_deserializer": key_deserializer,
@@ -1260,14 +1436,15 @@
                     "max_poll_records": max_poll_records,
                     "exclude_internal_topics": exclude_internal_topics,
                     "isolation_level": isolation_level,
                 },
                 is_manual=not auto_commit,
                 # subscriber args
                 no_ack=no_ack,
+                no_reply=no_reply,
                 retry=retry,
                 broker_middlewares=self._middlewares,
                 broker_dependencies=self._dependencies,
                 # AsyncAPI
                 title_=title,
                 description_=description,
                 include_in_schema=self._solve_include_in_schema(include_in_schema),
@@ -1297,30 +1474,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -1367,30 +1548,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -1437,30 +1622,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -1510,30 +1699,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
```

### Comparing `faststream-0.5.7/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.8/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.8/faststream/confluent/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,20 +410,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -433,178 +435,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -620,28 +655,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             Literal[False],
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -675,14 +713,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -825,20 +869,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -848,178 +894,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -1035,28 +1114,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             Literal[True],
             Doc("Whether to consume messages in batches or not."),
         ],
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -1232,20 +1314,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -1255,178 +1339,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -1442,28 +1559,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -1497,14 +1617,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -1650,20 +1776,22 @@
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -1673,178 +1801,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence[str],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -1860,28 +2021,31 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
@@ -1915,14 +2079,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -2092,14 +2262,15 @@
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
             no_ack=no_ack,
+            no_reply=no_reply,
             title=title,
             description=description,
             include_in_schema=include_in_schema,
             # FastAPI args
             response_model=response_model,
             response_model_include=response_model_include,
             response_model_exclude=response_model_exclude,
```

### Comparing `faststream-0.5.7/faststream/confluent/opentelemetry/middleware.py` & `faststream-0.5.8/faststream/confluent/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/opentelemetry/provider.py` & `faststream-0.5.8/faststream/confluent/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.8/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/publisher/producer.py` & `faststream-0.5.8/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/publisher/usecase.py` & `faststream-0.5.8/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/schemas/params.py` & `faststream-0.5.8/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.8/faststream/kafka/subscriber/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,210 +1,189 @@
 from typing import (
     TYPE_CHECKING,
-    Dict,
     Iterable,
     Literal,
     Optional,
     Tuple,
     Union,
     overload,
 )
 
-from typing_extensions import override
-
-from faststream.asyncapi.schema import (
-    Channel,
-    ChannelBinding,
-    CorrelationId,
-    Message,
-    Operation,
-)
-from faststream.asyncapi.schema.bindings import kafka
-from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import MsgType
-from faststream.confluent.subscriber.usecase import (
-    BatchSubscriber,
-    DefaultSubscriber,
-    LogicSubscriber,
+from faststream.exceptions import SetupError
+from faststream.kafka.subscriber.asyncapi import (
+    AsyncAPIBatchSubscriber,
+    AsyncAPIDefaultSubscriber,
 )
 
 if TYPE_CHECKING:
-    from confluent_kafka import Message as ConfluentMsg
+    from aiokafka import ConsumerRecord, TopicPartition
+    from aiokafka.abc import ConsumerRebalanceListener
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import BrokerMiddleware
     from faststream.types import AnyDict
 
 
-class AsyncAPISubscriber(LogicSubscriber[MsgType]):
-    """A class to handle logic and async API operations."""
-
-    def get_name(self) -> str:
-        return f'{",".join(self.topics)}:{self.call_name}'
-
-    def get_schema(self) -> Dict[str, Channel]:
-        channels = {}
-
-        payloads = self.get_payloads()
-
-        for t in self.topics:
-            handler_name = self.title_ or f"{t}:{self.call_name}"
-
-            channels[handler_name] = Channel(
-                description=self.description,
-                subscribe=Operation(
-                    message=Message(
-                        title=f"{handler_name}:Message",
-                        payload=resolve_payloads(payloads),
-                        correlationId=CorrelationId(
-                            location="$message.header#/correlation_id"
-                        ),
-                    ),
-                ),
-                bindings=ChannelBinding(
-                    kafka=kafka.ChannelBinding(topic=t),
-                ),
-            )
-
-        return channels
-
-    @overload  # type: ignore[override]
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: Literal[True],
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        connection_data: "AnyDict",
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConfluentMsg, ...]]"],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> "AsyncAPIBatchSubscriber": ...
-
-    @overload
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: Literal[False],
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        connection_data: "AnyDict",
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[ConfluentMsg]"],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> "AsyncAPIDefaultSubscriber": ...
-
-    @overload
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: bool,
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        connection_data: "AnyDict",
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable[
-            "BrokerMiddleware[Union[ConfluentMsg, Tuple[ConfluentMsg, ...]]]"
-        ],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> Union[
-        "AsyncAPIDefaultSubscriber",
-        "AsyncAPIBatchSubscriber",
-    ]: ...
-
-    @override
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: bool,
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        connection_data: "AnyDict",
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable[
-            "BrokerMiddleware[Union[ConfluentMsg, Tuple[ConfluentMsg, ...]]]"
-        ],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> Union[
-        "AsyncAPIDefaultSubscriber",
-        "AsyncAPIBatchSubscriber",
-    ]:
-        if batch:
-            return AsyncAPIBatchSubscriber(
-                *topics,
-                batch_timeout_ms=batch_timeout_ms,
-                max_records=max_records,
-                group_id=group_id,
-                connection_data=connection_data,
-                is_manual=is_manual,
-                no_ack=no_ack,
-                retry=retry,
-                broker_dependencies=broker_dependencies,
-                broker_middlewares=broker_middlewares,
-                title_=title_,
-                description_=description_,
-                include_in_schema=include_in_schema,
-            )
-        else:
-            return AsyncAPIDefaultSubscriber(
-                *topics,
-                group_id=group_id,
-                connection_data=connection_data,
-                is_manual=is_manual,
-                no_ack=no_ack,
-                retry=retry,
-                broker_dependencies=broker_dependencies,
-                broker_middlewares=broker_middlewares,
-                title_=title_,
-                description_=description_,
-                include_in_schema=include_in_schema,
-            )
-
-
-class AsyncAPIDefaultSubscriber(
-    DefaultSubscriber,
-    AsyncAPISubscriber["ConfluentMsg"],
-):
-    pass
-
-
-class AsyncAPIBatchSubscriber(
-    BatchSubscriber,
-    AsyncAPISubscriber[Tuple["ConfluentMsg", ...]],
-):
-    pass
+@overload
+def create_subscriber(
+    *topics: str,
+    batch: Literal[True],
+    batch_timeout_ms: int,
+    max_records: Optional[int],
+    # Kafka information
+    group_id: Optional[str],
+    listener: Optional["ConsumerRebalanceListener"],
+    pattern: Optional[str],
+    connection_args: "AnyDict",
+    partitions: Iterable["TopicPartition"],
+    is_manual: bool,
+    # Subscriber args
+    no_ack: bool,
+    no_reply: bool,
+    retry: bool,
+    broker_dependencies: Iterable["Depends"],
+    broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConsumerRecord, ...]]"],
+    # AsyncAPI args
+    title_: Optional[str],
+    description_: Optional[str],
+    include_in_schema: bool,
+) -> "AsyncAPIBatchSubscriber": ...
+
+
+@overload
+def create_subscriber(
+    *topics: str,
+    batch: Literal[False],
+    batch_timeout_ms: int,
+    max_records: Optional[int],
+    # Kafka information
+    group_id: Optional[str],
+    listener: Optional["ConsumerRebalanceListener"],
+    pattern: Optional[str],
+    connection_args: "AnyDict",
+    partitions: Iterable["TopicPartition"],
+    is_manual: bool,
+    # Subscriber args
+    no_ack: bool,
+    no_reply: bool,
+    retry: bool,
+    broker_dependencies: Iterable["Depends"],
+    broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
+    # AsyncAPI args
+    title_: Optional[str],
+    description_: Optional[str],
+    include_in_schema: bool,
+) -> "AsyncAPIDefaultSubscriber": ...
+
+
+@overload
+def create_subscriber(
+    *topics: str,
+    batch: bool,
+    batch_timeout_ms: int,
+    max_records: Optional[int],
+    # Kafka information
+    group_id: Optional[str],
+    listener: Optional["ConsumerRebalanceListener"],
+    pattern: Optional[str],
+    connection_args: "AnyDict",
+    partitions: Iterable["TopicPartition"],
+    is_manual: bool,
+    # Subscriber args
+    no_ack: bool,
+    no_reply: bool,
+    retry: bool,
+    broker_dependencies: Iterable["Depends"],
+    broker_middlewares: Iterable[
+        "BrokerMiddleware[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]"
+    ],
+    # AsyncAPI args
+    title_: Optional[str],
+    description_: Optional[str],
+    include_in_schema: bool,
+) -> Union[
+    "AsyncAPIDefaultSubscriber",
+    "AsyncAPIBatchSubscriber",
+]: ...
+
+
+def create_subscriber(
+    *topics: str,
+    batch: bool,
+    batch_timeout_ms: int,
+    max_records: Optional[int],
+    # Kafka information
+    group_id: Optional[str],
+    listener: Optional["ConsumerRebalanceListener"],
+    pattern: Optional[str],
+    connection_args: "AnyDict",
+    partitions: Iterable["TopicPartition"],
+    is_manual: bool,
+    # Subscriber args
+    no_ack: bool,
+    no_reply: bool,
+    retry: bool,
+    broker_dependencies: Iterable["Depends"],
+    broker_middlewares: Iterable[
+        "BrokerMiddleware[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]"
+    ],
+    # AsyncAPI args
+    title_: Optional[str],
+    description_: Optional[str],
+    include_in_schema: bool,
+) -> Union[
+    "AsyncAPIDefaultSubscriber",
+    "AsyncAPIBatchSubscriber",
+]:
+    if is_manual and not group_id:
+        raise SetupError("You must use `group_id` with manual commit mode.")
+
+    if not topics and not partitions and not pattern:
+        raise SetupError(
+            "You should provide either `topics` or `partitions` or `pattern`."
+        )
+    elif topics and partitions:
+        raise SetupError("You can't provide both `topics` and `partitions`.")
+    elif topics and pattern:
+        raise SetupError("You can't provide both `topics` and `pattern`.")
+    elif partitions and pattern:
+        raise SetupError("You can't provide both `partitions` and `pattern`.")
+
+    if batch:
+        return AsyncAPIBatchSubscriber(
+            *topics,
+            batch_timeout_ms=batch_timeout_ms,
+            max_records=max_records,
+            group_id=group_id,
+            listener=listener,
+            pattern=pattern,
+            connection_args=connection_args,
+            partitions=partitions,
+            is_manual=is_manual,
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_dependencies=broker_dependencies,
+            broker_middlewares=broker_middlewares,
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
+
+    else:
+        return AsyncAPIDefaultSubscriber(
+            *topics,
+            group_id=group_id,
+            listener=listener,
+            pattern=pattern,
+            connection_args=connection_args,
+            partitions=partitions,
+            is_manual=is_manual,
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_dependencies=broker_dependencies,
+            broker_middlewares=broker_middlewares,
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
```

### Comparing `faststream-0.5.7/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.8/faststream/confluent/subscriber/usecase.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,27 +53,29 @@
         group_id: Optional[str],
         connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
         no_ack: bool,
+        no_reply: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
             default_decoder=default_decoder,
             # Propagated args
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
@@ -152,17 +154,18 @@
 
         if self.task is not None and not self.task.done():
             self.task.cancel()
 
         self.task = None
 
     def _make_response_publisher(
-        self, message: "StreamMessage[Any]"
+        self,
+        message: "StreamMessage[Any]",
     ) -> Sequence[FakePublisher]:
-        if not message.reply_to or self._producer is None:
+        if self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
                     "topic": message.reply_to,
@@ -222,14 +225,15 @@
         *topics: str,
         # Kafka information
         group_id: Optional[str],
         connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
+        no_reply: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[Message]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
@@ -240,14 +244,15 @@
             connection_data=connection_data,
             is_manual=is_manual,
             # subscriber args
             default_parser=AsyncConfluentParser.parse_message,
             default_decoder=AsyncConfluentParser.decode_message,
             # Propagated args
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
@@ -281,14 +286,15 @@
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
         connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
+        no_reply: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[Tuple[Message, ...]]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
@@ -302,14 +308,15 @@
             connection_data=connection_data,
             is_manual=is_manual,
             # subscriber args
             default_parser=AsyncConfluentParser.parse_message_batch,
             default_decoder=AsyncConfluentParser.decode_message_batch,
             # Propagated args
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
```

### Comparing `faststream-0.5.7/faststream/kafka/annotations.py` & `faststream-0.5.8/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/message.py` & `faststream-0.5.8/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/parser.py` & `faststream-0.5.8/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/router.py` & `faststream-0.5.8/faststream/confluent/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,32 @@
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
-from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
-from faststream.kafka.broker.registrator import KafkaRegistrator
+from faststream.confluent.broker.registrator import KafkaRegistrator
 
 if TYPE_CHECKING:
-    from aiokafka import ConsumerRecord, TopicPartition
-    from aiokafka.abc import ConsumerRebalanceListener
-    from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
+    from confluent_kafka import Message
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
-    from faststream.kafka.message import KafkaMessage
+    from faststream.confluent.message import KafkaMessage
     from faststream.types import SendableMessage
 
 
 class KafkaPublisher(ArgsContainer):
     """Delayed KafkaPublisher registration object.
 
     Just a copy of `KafkaRegistrator.publisher(...)` arguments.
@@ -47,30 +44,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -124,48 +125,43 @@
             description=description,
             schema=schema,
             include_in_schema=include_in_schema,
         )
 
 
 class KafkaRoute(SubscriberRoute):
-    """Class to store delayed KafkaBroker subscriber registration."""
+    """Class to store delaied KafkaBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
             Union[
                 Callable[..., "SendableMessage"],
                 Callable[..., Awaitable["SendableMessage"]],
             ],
-            Doc(
-                "Message handler function "
-                "to wrap the same with `@broker.subscriber(...)` way."
-            ),
+            Doc("Message handler function."),
         ],
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         publishers: Annotated[
             Iterable[KafkaPublisher],
             Doc("Kafka publishers to broadcast the handler result."),
         ] = (),
-        batch: Annotated[
-            bool,
-            Doc("Whether to consume messages in batches or not."),
-        ] = False,
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -173,180 +169,213 @@
         value_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
+        fetch_max_wait_ms: Annotated[
+            int,
+            Doc(
+                """
+            The maximum amount of time in milliseconds
+            the server will block before answering the fetch request if
+            there isn't sufficient data to immediately satisfy the
+            requirement given by `fetch_min_bytes`.
+            """
+            ),
+        ] = 500,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
-        fetch_max_wait_ms: Annotated[
-            int,
-            Doc("""
-            The maximum amount of time in milliseconds
-            the server will block before answering the fetch request if
-            there isn't sufficient data to immediately satisfy the
-            requirement given by `fetch_min_bytes`.
-            """),
-        ] = 500,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence["AbstractPartitionAssignor"],
-            Doc("""
+            Sequence[str],
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
-        ] = (RoundRobinPartitionAssignor,),
+            """
+            ),
+        ] = ("roundrobin",),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -362,75 +391,44 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
+        batch: Annotated[
+            bool,
+            Doc("Whether to consume messages in batches or not."),
+        ] = False,
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
-        listener: Annotated[
-            Optional["ConsumerRebalanceListener"],
-            Doc("""
-            Optionally include listener
-               callback, which will be called before and after each rebalance
-               operation.
-               As part of group management, the consumer will keep track of
-               the list of consumers that belong to a particular group and
-               will trigger a rebalance operation if one of the following
-               events trigger:
-
-               * Number of partitions change for any of the subscribed topics
-               * Topic is created or deleted
-               * An existing member of the consumer group dies
-               * A new member is added to the consumer group
-
-               When any of these events are triggered, the provided listener
-               will be invoked first to indicate that the consumer's
-               assignment has been revoked, and then again when the new
-               assignment has been received. Note that this listener will
-               immediately override any listener set in a previous call
-               to subscribe. It is guaranteed, however, that the partitions
-               revoked/assigned
-               through this interface are from topics subscribed in this call.
-            """),
-        ] = None,
-        pattern: Annotated[
-            Optional[str],
-            Doc("""
-            Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
-        ] = None,
-        partitions: Annotated[
-            Optional[Iterable["TopicPartition"]],
-            Doc("""
-            A topic and partition tuple. You can't use 'topics' and 'partitions' in the same time.
-            """),
-        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
-            Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
+            Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware[KafkaMessage]"],
@@ -451,14 +449,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -495,39 +499,37 @@
             consumer_timeout_ms=consumer_timeout_ms,
             max_poll_records=max_poll_records,
             exclude_internal_topics=exclude_internal_topics,
             isolation_level=isolation_level,
             max_records=max_records,
             batch_timeout_ms=batch_timeout_ms,
             batch=batch,
-            listener=listener,
-            pattern=pattern,
-            partitions=partitions,
             # basic args
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
+            no_reply=no_reply,
             # AsyncAPI args
             title=title,
             description=description,
             include_in_schema=include_in_schema,
             # FastDepends args
             retry=retry,
             no_ack=no_ack,
         )
 
 
 class KafkaRouter(
     KafkaRegistrator,
     BrokerRouter[
         Union[
-            "ConsumerRecord",
-            Tuple["ConsumerRecord", ...],
+            "Message",
+            Tuple["Message", ...],
         ]
     ],
 ):
     """Includable to KafkaBroker router."""
 
     def __init__(
         self,
@@ -545,23 +547,23 @@
             Doc(
                 "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
         ] = (),
         middlewares: Annotated[
             Iterable[
                 Union[
-                    "BrokerMiddleware[ConsumerRecord]",
-                    "BrokerMiddleware[Tuple[ConsumerRecord, ...]]",
+                    "BrokerMiddleware[Message]",
+                    "BrokerMiddleware[Tuple[Message, ...]]",
                 ]
             ],
             Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
-            Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
+            Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
             Optional[bool],
```

### Comparing `faststream-0.5.7/faststream/kafka/security.py` & `faststream-0.5.8/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/testing.py` & `faststream-0.5.8/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/broker/broker.py` & `faststream-0.5.8/faststream/kafka/broker/broker.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,50 +63,57 @@
         ]
         retry_backoff_ms: Annotated[
             int,
             Doc(" Milliseconds to backoff when retrying on errors."),
         ]
         metadata_max_age_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The period of time in milliseconds after
             which we force a refresh of metadata even if we haven't seen any
             partition leadership changes to proactively discover any new
             brokers or partitions.
-            """),
+            """
+            ),
         ]
         connections_max_idle_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
              Close idle connections after the number
             of milliseconds specified by this config. Specifying `None` will
             disable idle checks.
-            """),
+            """
+            ),
         ]
         sasl_kerberos_service_name: str
         sasl_kerberos_domain_name: Optional[str]
         sasl_oauth_token_provider: Annotated[
             Optional[AbstractTokenProvider],
             Doc("OAuthBearer token provider instance."),
         ]
         loop: Optional[AbstractEventLoop]
         client_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             A name for this client. This string is passed in
             each request to servers and can be used to identify specific
             server-side log entries that correspond to this client. Also
             submitted to :class:`~.consumer.group_coordinator.GroupCoordinator`
             for logging with respect to consumer group administration.
-            """),
+            """
+            ),
         ]
         # publisher args
         acks: Annotated[
             Union[Literal[0, 1, -1, "all"], object],
-            Doc("""
+            Doc(
+                """
             One of ``0``, ``1``, ``all``. The number of acknowledgments
             the producer requires the leader to have received before considering a
             request complete. This controls the durability of records that are
             sent. The following settings are common:
 
             * ``0``: Producer will not wait for any acknowledgment from the server
               at all. The message will immediately be added to the socket
@@ -123,90 +130,103 @@
             * ``all``: The broker leader will wait for the full set of in-sync
               replicas to acknowledge the record. This guarantees that the
               record will not be lost as long as at least one in-sync replica
               remains alive. This is the strongest available guarantee.
 
             If unset, defaults to ``acks=1``. If `enable_idempotence` is
             :data:`True` defaults to ``acks=all``.
-            """),
+            """
+            ),
         ]
         key_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
             Doc("Used to convert user-supplied keys to bytes."),
         ]
         value_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
             Doc("used to convert user-supplied message values to bytes."),
         ]
         compression_type: Annotated[
             Optional[Literal["gzip", "snappy", "lz4", "zstd"]],
-            Doc("""
+            Doc(
+                """
             The compression type for all data generated bythe producer.
             Compression is of full batches of data, so the efficacy of batching
             will also impact the compression ratio (more batching means better
             compression).
-            """),
+            """
+            ),
         ]
         max_batch_size: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum size of buffered data per partition.
             After this amount `send` coroutine will block until batch is drained.
-            """),
+            """
+            ),
         ]
         partitioner: Annotated[
             Callable[
                 [bytes, List[Partition], List[Partition]],
                 Partition,
             ],
-            Doc("""
+            Doc(
+                """
             Callable used to determine which partition
             each message is assigned to. Called (after key serialization):
             ``partitioner(key_bytes, all_partitions, available_partitions)``.
             The default partitioner implementation hashes each non-None key
             using the same murmur2 algorithm as the Java client so that
             messages with the same key are assigned to the same partition.
             When a key is :data:`None`, the message is delivered to a random partition
             (filtered to partitions with available leaders only, if possible).
-            """),
+            """
+            ),
         ]
         max_request_size: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum size of a request. This is also
             effectively a cap on the maximum record size. Note that the server
             has its own cap on record size which may be different from this.
             This setting will limit the number of record batches the producer
             will send in a single request to avoid sending huge requests.
-            """),
+            """
+            ),
         ]
         linger_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The producer groups together any records that arrive
             in between request transmissions into a single batched request.
             Normally this occurs only under load when records arrive faster
             than they can be sent out. However in some circumstances the client
             may want to reduce the number of requests even under moderate load.
             This setting accomplishes this by adding a small amount of
             artificial delay; that is, if first request is processed faster,
             than `linger_ms`, producer will wait ``linger_ms - process_time``.
-            """),
+            """
+            ),
         ]
         send_backoff_ms: int
         enable_idempotence: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             When set to `True`, the producer will
             ensure that exactly one copy of each message is written in the
             stream. If `False`, producer retries due to broker failures,
             etc., may write duplicates of the retried message in the stream.
             Note that enabling idempotence acks to set to ``all``. If it is not
             explicitly set by the user it will be chosen.
-            """),
+            """
+            ),
         ]
         transactional_id: Optional[str]
         transaction_timeout_ms: int
 
 
 class KafkaBroker(
     KafkaRegistrator,
@@ -215,71 +235,80 @@
     url: List[str]
     _producer: Optional["AioKafkaFastProducer"]
 
     def __init__(
         self,
         bootstrap_servers: Annotated[
             Union[str, Iterable[str]],
-            Doc("""
+            Doc(
+                """
             A `host[:port]` string (or list of `host[:port]` strings) that the consumer should contact to bootstrap
             initial cluster metadata.
 
             This does not have to be the full node list.
             It just needs to have at least one broker that will respond to a
             Metadata API Request. Default port is 9092.
-            """),
+            """
+            ),
         ] = "localhost",
         *,
         # both
         request_timeout_ms: Annotated[
             int,
             Doc("Client request timeout in milliseconds."),
         ] = 40 * 1000,
         retry_backoff_ms: Annotated[
             int,
             Doc(" Milliseconds to backoff when retrying on errors."),
         ] = 100,
         metadata_max_age_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The period of time in milliseconds after
             which we force a refresh of metadata even if we haven't seen any
             partition leadership changes to proactively discover any new
             brokers or partitions.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         connections_max_idle_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
              Close idle connections after the number
             of milliseconds specified by this config. Specifying `None` will
             disable idle checks.
-            """),
+            """
+            ),
         ] = 9 * 60 * 1000,
         sasl_kerberos_service_name: str = "kafka",
         sasl_kerberos_domain_name: Optional[str] = None,
         sasl_oauth_token_provider: Annotated[
             Optional["AbstractTokenProvider"],
             Doc("OAuthBearer token provider instance."),
         ] = None,
         loop: Optional["AbstractEventLoop"] = None,
         client_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             A name for this client. This string is passed in
             each request to servers and can be used to identify specific
             server-side log entries that correspond to this client. Also
             submitted to :class:`~.consumer.group_coordinator.GroupCoordinator`
             for logging with respect to consumer group administration.
-            """),
+            """
+            ),
         ] = SERVICE_NAME,
         # publisher args
         acks: Annotated[
             Union[Literal[0, 1, -1, "all"], object],
-            Doc("""
+            Doc(
+                """
             One of ``0``, ``1``, ``all``. The number of acknowledgments
             the producer requires the leader to have received before considering a
             request complete. This controls the durability of records that are
             sent. The following settings are common:
 
             * ``0``: Producer will not wait for any acknowledgment from the server
               at all. The message will immediately be added to the socket
@@ -296,90 +325,103 @@
             * ``all``: The broker leader will wait for the full set of in-sync
               replicas to acknowledge the record. This guarantees that the
               record will not be lost as long as at least one in-sync replica
               remains alive. This is the strongest available guarantee.
 
             If unset, defaults to ``acks=1``. If `enable_idempotence` is
             :data:`True` defaults to ``acks=all``.
-            """),
+            """
+            ),
         ] = _missing,
         key_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
             Doc("Used to convert user-supplied keys to bytes."),
         ] = None,
         value_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
             Doc("used to convert user-supplied message values to bytes."),
         ] = None,
         compression_type: Annotated[
             Optional[Literal["gzip", "snappy", "lz4", "zstd"]],
-            Doc("""
+            Doc(
+                """
             The compression type for all data generated bythe producer.
             Compression is of full batches of data, so the efficacy of batching
             will also impact the compression ratio (more batching means better
             compression).
-            """),
+            """
+            ),
         ] = None,
         max_batch_size: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum size of buffered data per partition.
             After this amount `send` coroutine will block until batch is drained.
-            """),
+            """
+            ),
         ] = 16 * 1024,
         partitioner: Annotated[
             Callable[
                 [bytes, List[Partition], List[Partition]],
                 Partition,
             ],
-            Doc("""
+            Doc(
+                """
             Callable used to determine which partition
             each message is assigned to. Called (after key serialization):
             ``partitioner(key_bytes, all_partitions, available_partitions)``.
             The default partitioner implementation hashes each non-None key
             using the same murmur2 algorithm as the Java client so that
             messages with the same key are assigned to the same partition.
             When a key is :data:`None`, the message is delivered to a random partition
             (filtered to partitions with available leaders only, if possible).
-            """),
+            """
+            ),
         ] = DefaultPartitioner(),
         max_request_size: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum size of a request. This is also
             effectively a cap on the maximum record size. Note that the server
             has its own cap on record size which may be different from this.
             This setting will limit the number of record batches the producer
             will send in a single request to avoid sending huge requests.
-            """),
+            """
+            ),
         ] = 1024 * 1024,
         linger_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The producer groups together any records that arrive
             in between request transmissions into a single batched request.
             Normally this occurs only under load when records arrive faster
             than they can be sent out. However in some circumstances the client
             may want to reduce the number of requests even under moderate load.
             This setting accomplishes this by adding a small amount of
             artificial delay; that is, if first request is processed faster,
             than `linger_ms`, producer will wait ``linger_ms - process_time``.
-            """),
+            """
+            ),
         ] = 0,
         send_backoff_ms: int = 100,
         enable_idempotence: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             When set to `True`, the producer will
             ensure that exactly one copy of each message is written in the
             stream. If `False`, producer retries due to broker failures,
             etc., may write duplicates of the retried message in the stream.
             Note that enabling idempotence acks to set to ``all``. If it is not
             explicitly set by the user it will be chosen.
-            """),
+            """
+            ),
         ] = False,
         transactional_id: Optional[str] = None,
         transaction_timeout_ms: int = 60 * 1000,
         # broker base args
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
@@ -628,37 +670,43 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Message headers to store metainformation."),
         ] = None,
         correlation_id: Annotated[
             Optional[str],
@@ -704,25 +752,29 @@
         ],
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Messages headers to store metainformation."),
         ] = None,
         reply_to: Annotated[
             str,
```

### Comparing `faststream-0.5.7/faststream/kafka/broker/logging.py` & `faststream-0.5.8/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/broker/registrator.py` & `faststream-0.5.8/faststream/kafka/broker/registrator.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from aiokafka import ConsumerRecord
 from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
 from faststream.kafka.publisher.asyncapi import AsyncAPIPublisher
-from faststream.kafka.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.kafka.subscriber.factory import create_subscriber
 
 if TYPE_CHECKING:
-    from aiokafka import ConsumerRecord, TopicPartition
+    from aiokafka import TopicPartition
     from aiokafka.abc import ConsumerRebalanceListener
     from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         CustomCallable,
         Filter,
@@ -44,16 +44,16 @@
         AsyncAPIDefaultSubscriber,
     )
 
 
 class KafkaRegistrator(
     ABCBroker[
         Union[
-            "ConsumerRecord",
-            Tuple["ConsumerRecord", ...],
+            ConsumerRecord,
+            Tuple[ConsumerRecord, ...],
         ]
     ]
 ):
     """Includable to KafkaBroker router."""
 
     _subscribers: Dict[
         int,
@@ -73,20 +73,22 @@
         ],
         batch: Annotated[
             Literal[False],
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -96,178 +98,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence["AbstractPartitionAssignor"],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = (RoundRobinPartitionAssignor,),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -283,32 +318,36 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -322,28 +361,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -373,14 +417,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -404,20 +454,22 @@
         ],
         batch: Annotated[
             Literal[True],
             Doc("Whether to consume messages in batches or not."),
         ],
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -427,178 +479,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence["AbstractPartitionAssignor"],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = (RoundRobinPartitionAssignor,),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -614,32 +699,36 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -653,28 +742,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -704,14 +798,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -735,20 +835,22 @@
         ],
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -758,178 +860,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence["AbstractPartitionAssignor"],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = (RoundRobinPartitionAssignor,),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -945,32 +1080,36 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -984,28 +1123,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -1035,14 +1179,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -1069,20 +1219,22 @@
         ],
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         group_id: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Name of the consumer group to join for dynamic
             partition assignment (if enabled), and to use for fetching and
             committing offsets. If `None`, auto-partition assignment (via
             group coordinator) and offset commits are disabled.
-            """),
+            """
+            ),
         ] = None,
         key_deserializer: Annotated[
             Optional[Callable[[bytes], Any]],
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "key and returns a deserialized one."
             ),
@@ -1092,178 +1244,211 @@
             Doc(
                 "Any callable that takes a raw message `bytes` "
                 "value and returns a deserialized value."
             ),
         ] = None,
         fetch_max_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data the server should
             return for a fetch request. This is not an absolute maximum, if
             the first message in the first non-empty partition of the fetch
             is larger than this value, the message will still be returned
             to ensure that the consumer can make progress. NOTE: consumer
             performs fetches to multiple brokers in parallel so memory
             usage will depend on the number of brokers containing
             partitions for the topic.
-            """),
+            """
+            ),
         ] = 50 * 1024 * 1024,
         fetch_min_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Minimum amount of data the server should
             return for a fetch request, otherwise wait up to
             `fetch_max_wait_ms` for more data to accumulate.
-            """),
+            """
+            ),
         ] = 1,
         fetch_max_wait_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of time in milliseconds
             the server will block before answering the fetch request if
             there isn't sufficient data to immediately satisfy the
             requirement given by `fetch_min_bytes`.
-            """),
+            """
+            ),
         ] = 500,
         max_partition_fetch_bytes: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The maximum amount of data
             per-partition the server will return. The maximum total memory
             used for a request ``= #partitions * max_partition_fetch_bytes``.
             This size must be at least as large as the maximum message size
             the server allows or else it is possible for the producer to
             send messages larger than the consumer can fetch. If that
             happens, the consumer can get stuck trying to fetch a large
             message on a certain partition.
-            """),
+            """
+            ),
         ] = 1 * 1024 * 1024,
         auto_offset_reset: Annotated[
             Literal["latest", "earliest", "none"],
-            Doc("""
+            Doc(
+                """
             A policy for resetting offsets on `OffsetOutOfRangeError` errors:
 
             * `earliest` will move to the oldest available message
             * `latest` will move to the most recent
             * `none` will raise an exception so you can handle this case
-            """),
+            """
+            ),
         ] = "latest",
         auto_commit: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             If `True` the consumer's offset will be
             periodically committed in the background.
-            """),
+            """
+            ),
         ] = True,
         auto_commit_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds between automatic
-            offset commits, if `auto_commit` is `True`."""),
+            offset commits, if `auto_commit` is `True`."""
+            ),
         ] = 5 * 1000,
         check_crcs: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
-            """),
+            """
+            ),
         ] = True,
         partition_assignment_strategy: Annotated[
             Sequence["AbstractPartitionAssignor"],
-            Doc("""
+            Doc(
+                """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
             one. The coordinator will choose the old assignment strategy until
             all members have been updated. Then it will choose the new
             strategy.
-            """),
+            """
+            ),
         ] = (RoundRobinPartitionAssignor,),
         max_poll_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum allowed time between calls to
             consume messages in batches. If this interval
             is exceeded the consumer is considered failed and the group will
             rebalance in order to reassign the partitions to another consumer
             group member. If API methods block waiting for messages, that time
             does not count against this timeout.
-            """),
+            """
+            ),
         ] = 5 * 60 * 1000,
         rebalance_timeout_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum time server will wait for this
             consumer to rejoin the group in a case of rebalance. In Java client
             this behaviour is bound to `max.poll.interval.ms` configuration,
             but as ``aiokafka`` will rejoin the group in the background, we
             decouple this setting to allow finer tuning by users that use
             `ConsumerRebalanceListener` to delay rebalacing. Defaults
             to ``session_timeout_ms``
-            """),
+            """
+            ),
         ] = None,
         session_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Client group session and failure detection
             timeout. The consumer sends periodic heartbeats
             (`heartbeat.interval.ms`) to indicate its liveness to the broker.
             If no hearts are received by the broker for a group member within
             the session timeout, the broker will remove the consumer from the
             group and trigger a rebalance. The allowed range is configured with
             the **broker** configuration properties
             `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
-            """),
+            """
+            ),
         ] = 10 * 1000,
         heartbeat_interval_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             The expected time in milliseconds
             between heartbeats to the consumer coordinator when using
             Kafka's group management feature. Heartbeats are used to ensure
             that the consumer's session stays active and to facilitate
             rebalancing when new consumers join or leave the group. The
             value must be set lower than `session_timeout_ms`, but typically
             should be set no higher than 1/3 of that value. It can be
             adjusted even lower to control the expected time for normal
             rebalances.
-            """),
+            """
+            ),
         ] = 3 * 1000,
         consumer_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Maximum wait timeout for background fetching
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions.
-            """),
+            """
+            ),
         ] = 200,
         max_poll_records: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             The maximum number of records returned in a
             single call by batch consumer. Has no limit by default.
-            """),
+            """
+            ),
         ] = None,
         exclude_internal_topics: Annotated[
             bool,
-            Doc("""
+            Doc(
+                """
             Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
             subscribing to it.
-            """),
+            """
+            ),
         ] = True,
         isolation_level: Annotated[
             Literal["read_uncommitted", "read_committed"],
-            Doc("""
+            Doc(
+                """
             Controls how to read messages written
             transactionally.
 
             * `read_committed`, batch consumer will only return
             transactional messages which have been committed.
 
             * `read_uncommitted` (the default), batch consumer will
@@ -1279,32 +1464,36 @@
             than the offset of the first open transaction. In particular any
             messages appearing after messages belonging to ongoing transactions
             will be withheld until the relevant transaction has been completed.
             As a result, `read_committed` consumers will not be able to read up
             to the high watermark when there are in flight transactions.
             Further, when in `read_committed` the seek_to_end method will
             return the LSO. See method docs below.
-            """),
+            """
+            ),
         ] = "read_uncommitted",
         batch_timeout_ms: Annotated[
             int,
-            Doc("""
+            Doc(
+                """
             Milliseconds spent waiting if
             data is not available in the buffer. If 0, returns immediately
             with any records that are available currently in the buffer,
             else returns empty.
-            """),
+            """
+            ),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -1318,28 +1507,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -1369,14 +1563,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -1390,15 +1590,15 @@
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
     ]:
         subscriber = super().subscriber(
-            AsyncAPISubscriber.create(
+            create_subscriber(
                 *topics,
                 batch=batch,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
                 listener=listener,
                 pattern=pattern,
@@ -1423,14 +1623,15 @@
                     "exclude_internal_topics": exclude_internal_topics,
                     "isolation_level": isolation_level,
                 },
                 partitions=partitions,
                 is_manual=not auto_commit,
                 # subscriber args
                 no_ack=no_ack,
+                no_reply=no_reply,
                 retry=retry,
                 broker_middlewares=self._middlewares,
                 broker_dependencies=self._dependencies,
                 # AsyncAPI
                 title_=title,
                 description_=description,
                 include_in_schema=self._solve_include_in_schema(include_in_schema),
@@ -1461,30 +1662,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -1531,30 +1736,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -1601,30 +1810,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
@@ -1674,30 +1887,34 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
```

### Comparing `faststream-0.5.7/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.8/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.8/faststream/kafka/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -886,15 +886,16 @@
         ] = None,
         batch: Annotated[
             Literal[False],
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -908,28 +909,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -959,14 +965,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -1375,15 +1387,16 @@
         ] = None,
         batch: Annotated[
             Literal[True],
             Doc("Whether to consume messages in batches or not."),
         ],
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -1397,28 +1410,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -1448,14 +1466,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -1864,15 +1888,16 @@
         ] = None,
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -1886,28 +1911,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -1937,14 +1967,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -2356,15 +2392,16 @@
         ] = None,
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         listener: Annotated[
             Optional["ConsumerRebalanceListener"],
-            Doc("""
+            Doc(
+                """
             Optionally include listener
                callback, which will be called before and after each rebalance
                operation.
                As part of group management, the consumer will keep track of
                the list of consumers that belong to a particular group and
                will trigger a rebalance operation if one of the following
                events trigger:
@@ -2378,28 +2415,33 @@
                will be invoked first to indicate that the consumer's
                assignment has been revoked, and then again when the new
                assignment has been received. Note that this listener will
                immediately override any listener set in a previous call
                to subscribe. It is guaranteed, however, that the partitions
                revoked/assigned
                through this interface are from topics subscribed in this call.
-            """),
+            """
+            ),
         ] = None,
         pattern: Annotated[
             Optional[str],
-            Doc("""
+            Doc(
+                """
             Pattern to match available topics. You must provide either topics or pattern, but not both.
-            """),
+            """
+            ),
         ] = None,
         partitions: Annotated[
             Iterable["TopicPartition"],
-            Doc("""
+            Doc(
+                """
             An explicit partitions list to assign.
             You can't use 'topics' and 'partitions' in the same time.
-            """),
+            """
+            ),
         ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
@@ -2429,14 +2471,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -2609,14 +2657,15 @@
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
             no_ack=no_ack,
+            no_reply=no_reply,
             title=title,
             description=description,
             include_in_schema=include_in_schema,
             # FastAPI args
             response_model=response_model,
             response_model_include=response_model_include,
             response_model_exclude=response_model_exclude,
```

### Comparing `faststream-0.5.7/faststream/kafka/opentelemetry/middleware.py` & `faststream-0.5.8/faststream/kafka/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/opentelemetry/provider.py` & `faststream-0.5.8/faststream/kafka/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.8/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/publisher/producer.py` & `faststream-0.5.8/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/publisher/usecase.py` & `faststream-0.5.8/faststream/kafka/publisher/usecase.py`

 * *Files 11% similar despite different names*

```diff
@@ -106,37 +106,43 @@
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ] = "",
         *,
         key: Annotated[
             Union[bytes, Any, None],
-            Doc("""
+            Doc(
+                """
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """),
+            """
+            ),
         ] = None,
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Message headers to store metainformation."),
         ] = None,
         correlation_id: Annotated[
             Optional[str],
@@ -201,25 +207,29 @@
         ],
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ] = "",
         partition: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
-            """),
+            """
+            ),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
-            Doc("""
+            Doc(
+                """
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """),
+            """
+            ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Messages headers to store metainformation."),
         ] = None,
         reply_to: Annotated[
             str,
```

### Comparing `faststream-0.5.7/faststream/kafka/schemas/params.py` & `faststream-0.5.8/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.8/faststream/kafka/subscriber/usecase.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,27 +61,29 @@
         pattern: Optional[str],
         partitions: Iterable["TopicPartition"],
         is_manual: bool,
         # Subscriber args
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
         no_ack: bool,
+        no_reply: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
             default_decoder=default_decoder,
             # Propagated args
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
@@ -175,15 +177,15 @@
 
         self.task = None
 
     def _make_response_publisher(
         self,
         message: "StreamMessage[Any]",
     ) -> Sequence[FakePublisher]:
-        if not message.reply_to or self._producer is None:
+        if self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
                     "topic": message.reply_to,
@@ -291,14 +293,15 @@
         listener: Optional["ConsumerRebalanceListener"],
         pattern: Optional[str],
         connection_args: "AnyDict",
         partitions: Iterable["TopicPartition"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
+        no_reply: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
@@ -312,14 +315,15 @@
             partitions=partitions,
             is_manual=is_manual,
             # subscriber args
             default_parser=AioKafkaParser.parse_message,
             default_decoder=AioKafkaParser.decode_message,
             # Propagated args
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
@@ -341,14 +345,15 @@
         listener: Optional["ConsumerRebalanceListener"],
         pattern: Optional[str],
         connection_args: "AnyDict",
         partitions: Iterable["TopicPartition"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
+        no_reply: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable[
             "BrokerMiddleware[Sequence[Tuple[ConsumerRecord, ...]]]"
         ],
         # AsyncAPI args
         title_: Optional[str],
@@ -367,14 +372,15 @@
             partitions=partitions,
             is_manual=is_manual,
             # subscriber args
             default_parser=AioKafkaParser.parse_message_batch,
             default_decoder=AioKafkaParser.decode_message_batch,
             # Propagated args
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
```

### Comparing `faststream-0.5.7/faststream/log/formatter.py` & `faststream-0.5.8/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/log/logging.py` & `faststream-0.5.8/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/annotations.py` & `faststream-0.5.8/faststream/nats/fastapi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from nats.aio.client import Client as NatsClient
 from nats.js.client import JetStreamContext
 from typing_extensions import Annotated
 
-from faststream.annotations import ContextRepo, Logger, NoCast
+from faststream.broker.fastapi.context import Context, ContextRepo, Logger
 from faststream.nats.broker import NatsBroker as NB
+from faststream.nats.fastapi.fastapi import NatsRouter
 from faststream.nats.message import NatsMessage as NM
 from faststream.nats.publisher.producer import NatsFastProducer, NatsJSFastProducer
-from faststream.utils.context import Context
+
+NatsMessage = Annotated[NM, Context("message")]
+NatsBroker = Annotated[NB, Context("broker")]
+Client = Annotated[NatsClient, Context("broker._connection")]
+JsClient = Annotated[JetStreamContext, Context("broker._stream")]
+NatsProducer = Annotated[NatsFastProducer, Context("broker._producer")]
+NatsJsProducer = Annotated[NatsJSFastProducer, Context("broker._js_producer")]
 
 __all__ = (
+    "Context",
     "Logger",
     "ContextRepo",
-    "NoCast",
-    "NatsMessage",
+    "NatsRouter",
     "NatsBroker",
+    "NatsMessage",
     "Client",
     "JsClient",
+    "NatsProducer",
+    "NatsJsProducer",
 )
-
-NatsMessage = Annotated[NM, Context("message")]
-NatsBroker = Annotated[NB, Context("broker")]
-Client = Annotated[NatsClient, Context("broker._connection")]
-JsClient = Annotated[JetStreamContext, Context("broker._stream")]
-NatsProducer = Annotated[NatsFastProducer, Context("broker._producer")]
-NatsJsProducer = Annotated[NatsJSFastProducer, Context("broker._js_producer")]
```

### Comparing `faststream-0.5.7/faststream/nats/message.py` & `faststream-0.5.8/faststream/nats/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import TYPE_CHECKING, List, Union
+from typing import List, Union
 
-from faststream.broker.message import StreamMessage
+from nats.aio.msg import Msg
+from nats.js.api import ObjectInfo
+from nats.js.kv import KeyValue
 
-if TYPE_CHECKING:
-    from nats.aio.msg import Msg
+from faststream.broker.message import StreamMessage
 
 
-class NatsMessage(StreamMessage["Msg"]):
+class NatsMessage(StreamMessage[Msg]):
     """A class to represent a NATS message."""
 
     async def ack(self) -> None:
         # Check `self.raw_message._ackd` instead of `self.committed`
         # to be compatible with `self.raw_message.ack()`
         if not self.raw_message._ackd:
             await self.raw_message.ack()
@@ -30,15 +31,15 @@
             await super().reject()
 
     async def in_progress(self) -> None:
         if not self.raw_message._ackd:
             await self.raw_message.in_progress()
 
 
-class NatsBatchMessage(StreamMessage[List["Msg"]]):
+class NatsBatchMessage(StreamMessage[List[Msg]]):
     """A class to represent a NATS batch message."""
 
     async def ack(self) -> None:
         for m in filter(
             lambda m: not m._ackd,
             self.raw_message,
         ):
@@ -69,7 +70,15 @@
 
     async def in_progress(self) -> None:
         for m in filter(
             lambda m: not m._ackd,
             self.raw_message,
         ):
             await m.in_progress()
+
+
+class NatsKvMessage(StreamMessage[KeyValue.Entry]):
+    pass
+
+
+class NatsObjMessage(StreamMessage[ObjectInfo]):
+    pass
```

### Comparing `faststream-0.5.7/faststream/nats/parser.py` & `faststream-0.5.8/faststream/nats/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-from typing import TYPE_CHECKING, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
-from faststream.nats.message import NatsBatchMessage, NatsMessage
+from faststream.nats.message import (
+    NatsBatchMessage,
+    NatsKvMessage,
+    NatsMessage,
+    NatsObjMessage,
+)
 from faststream.nats.schemas.js_stream import compile_nats_wildcard
 
 if TYPE_CHECKING:
     from nats.aio.msg import Msg
+    from nats.js.api import ObjectInfo
+    from nats.js.kv import KeyValue
 
     from faststream.types import AnyDict, DecodedMessage
 
 
 class NatsBaseParser:
     """A class to parse NATS messages."""
 
@@ -32,15 +39,15 @@
         ) is not None:
             path = match.groupdict()
 
         return path
 
     @staticmethod
     async def decode_message(
-        msg: "StreamMessage[Msg]",
+        msg: "StreamMessage[Any]",
     ) -> "DecodedMessage":
         return decode_message(msg)
 
 
 class NatsParser(NatsBaseParser):
     """A class to parse NATS core messages."""
 
@@ -135,7 +142,26 @@
         for m in msg.raw_message:
             one_msg = await self.parse_message(m, path=path)
             path = one_msg.path
 
             data.append(decode_message(one_msg))
 
         return data
+
+
+class KvParser(NatsBaseParser):
+    async def parse_message(
+        self, msg: "KeyValue.Entry"
+    ) -> StreamMessage["KeyValue.Entry"]:
+        return NatsKvMessage(
+            raw_message=msg,
+            body=msg.value,
+            path=self.get_path(msg.key) or {},
+        )
+
+
+class ObjParser(NatsBaseParser):
+    async def parse_message(self, msg: "ObjectInfo") -> StreamMessage["ObjectInfo"]:
+        return NatsObjMessage(
+            raw_message=msg,
+            body=msg.name,
+        )
```

### Comparing `faststream-0.5.7/faststream/nats/router.py` & `faststream-0.5.8/faststream/nats/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         BrokerMiddleware,
         CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
     from faststream.nats.message import NatsBatchMessage, NatsMessage
-    from faststream.nats.schemas import JStream, PullSub
+    from faststream.nats.schemas import JStream, KvWatch, ObjWatch, PullSub
     from faststream.types import SendableMessage
 
 
 class NatsPublisher(ArgsContainer):
     """Delayed NatsPublisher registration object.
 
     Just a copy of `KafkaRegistrator.publisher(...)` arguments.
@@ -201,14 +201,22 @@
         pull_sub: Annotated[
             Optional["PullSub"],
             Doc(
                 "NATS Pull consumer parameters container. "
                 "Should be used with `stream` only."
             ),
         ] = None,
+        kv_watch: Annotated[
+            Union[str, "KvWatch", None],
+            Doc("KeyValue watch parameters container."),
+        ] = None,
+        obj_watch: Annotated[
+            Union[bool, "ObjWatch"],
+            Doc("ObjecStore watch parameters container."),
+        ] = False,
         inbox_prefix: Annotated[
             bytes,
             Doc(
                 "Prefix for generating unique inboxes, subjects with that prefix and NUID."
             ),
         ] = api.INBOX_PREFIX,
         # custom
@@ -259,14 +267,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -291,26 +305,29 @@
             config=config,
             ordered_consumer=ordered_consumer,
             idle_heartbeat=idle_heartbeat,
             flow_control=flow_control,
             deliver_policy=deliver_policy,
             headers_only=headers_only,
             pull_sub=pull_sub,
+            kv_watch=kv_watch,
+            obj_watch=obj_watch,
             inbox_prefix=inbox_prefix,
             ack_first=ack_first,
             stream=stream,
             max_workers=max_workers,
             queue=queue,
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
             no_ack=no_ack,
+            no_reply=no_reply,
             title=title,
             description=description,
             include_in_schema=include_in_schema,
         )
 
 
 class NatsRouter(
```

### Comparing `faststream-0.5.7/faststream/nats/security.py` & `faststream-0.5.8/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/testing.py` & `faststream-0.5.8/faststream/nats/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
 from faststream.exceptions import WRONG_PUBLISH_ARGS
 from faststream.nats.broker import NatsBroker
 from faststream.nats.publisher.producer import NatsFastProducer
 from faststream.nats.schemas.js_stream import is_subject_match_wildcard
-from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.nats.subscriber.usecase import LogicSubscriber
 from faststream.testing.broker import TestBroker, call_handler
 
 if TYPE_CHECKING:
     from faststream.broker.wrapper.call import HandlerCallWrapper
     from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
     from faststream.types import AnyDict, SendableMessage
 
@@ -51,15 +51,15 @@
         return AsyncMock()
 
     @staticmethod
     def remove_publisher_fake_subscriber(
         broker: NatsBroker, publisher: "AsyncAPIPublisher"
     ) -> None:
         broker._subscribers.pop(
-            AsyncAPISubscriber.get_routing_hash(publisher.subject), None
+            LogicSubscriber.get_routing_hash(publisher.subject), None
         )
 
 
 class FakeProducer(NatsFastProducer):
     def __init__(self, broker: NatsBroker) -> None:
         self.broker = broker
 
@@ -87,20 +87,23 @@
             subject=subject,
             headers=headers,
             correlation_id=correlation_id,
             reply_to=reply_to,
         )
 
         for handler in self.broker._subscribers.values():  # pragma: no branch
-            if stream and getattr(handler.stream, "name", None) != stream:
+            if stream and (
+                not (handler_stream := getattr(handler, "stream", None))
+                or stream != handler_stream.name
+            ):
                 continue
 
-            if is_subject_match_wildcard(subject, handler.subject):
+            if is_subject_match_wildcard(subject, handler.clear_subject):
                 msg: Union[List[PatchedMessage], PatchedMessage]
-                if getattr(handler.pull_sub, "batch", False):
+                if (pull := getattr(handler, "pull_sub", None)) and pull.batch:
                     msg = [incoming]
                 else:
                     msg = incoming
 
                 r = await call_handler(
                     handler=handler,
                     message=msg,
@@ -138,15 +141,16 @@
 
 
 class PatchedMessage(Msg):
     async def ack(self) -> None:
         pass
 
     async def ack_sync(
-        self, timeout: float = 1
+        self,
+        timeout: float = 1,
     ) -> "PatchedMessage":  # pragma: no cover
         return self
 
     async def nak(self, delay: Union[int, float, None] = None) -> None:
         pass
 
     async def term(self) -> None:
```

### Comparing `faststream-0.5.7/faststream/nats/broker/broker.py` & `faststream-0.5.8/faststream/nats/broker/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from nats.js.errors import BadRequestError
 from typing_extensions import Annotated, Doc, override
 
 from faststream.__about__ import SERVICE_NAME
 from faststream.broker.message import gen_cor_id
 from faststream.nats.broker.logging import NatsLoggingBroker
 from faststream.nats.broker.registrator import NatsRegistrator
+from faststream.nats.helpers import KVBucketDeclarer, OSBucketDeclarer
 from faststream.nats.publisher.producer import NatsFastProducer, NatsJSFastProducer
 from faststream.nats.security import parse_security
 from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
 
 if TYPE_CHECKING:
     import ssl
     from types import TracebackType
@@ -47,15 +48,18 @@
         Client,
         Credentials,
         ErrorCallback,
         JWTCallback,
         SignatureCallback,
     )
     from nats.aio.msg import Msg
+    from nats.js.api import Placement, RePublish, StorageType
     from nats.js.client import JetStreamContext
+    from nats.js.kv import KeyValue
+    from nats.js.object_store import ObjectStore
     from typing_extensions import TypedDict, Unpack
 
     from faststream.asyncapi import schema as asyncapi
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
@@ -214,14 +218,16 @@
     """A class to represent a NATS broker."""
 
     url: List[str]
     stream: Optional["JetStreamContext"]
 
     _producer: Optional["NatsFastProducer"]
     _js_producer: Optional["NatsJSFastProducer"]
+    _kv_declarer: Optional["KVBucketDeclarer"]
+    _os_declarer: Optional["OSBucketDeclarer"]
 
     def __init__(
         self,
         servers: Annotated[
             Union[str, Iterable[str]],
             Doc("NATS cluster addresses to connect."),
         ] = ("nats://localhost:4222",),
@@ -537,14 +543,16 @@
 
         self.__is_connected = False
         self._producer = None
 
         # JS options
         self.stream = None
         self._js_producer = None
+        self._kv_declarer = None
+        self._os_declarer = None
 
     @override
     async def connect(  # type: ignore[override]
         self,
         servers: Annotated[
             Union[str, Iterable[str], object],
             Doc("NATS cluster addresses to connect."),
@@ -579,14 +587,17 @@
 
         self._js_producer = NatsJSFastProducer(
             connection=stream,
             decoder=self._decoder,
             parser=self._parser,
         )
 
+        self._kv_declarer = KVBucketDeclarer(stream)
+        self._os_declarer = OSBucketDeclarer(stream)
+
         return connection
 
     async def _close(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional["TracebackType"] = None,
@@ -605,52 +616,58 @@
         """Connect broker to NATS cluster and startup all subscribers."""
         await super().start()
 
         assert self._connection  # nosec B101
         assert self.stream, "Broker should be started already"  # nosec B101
         assert self._producer, "Broker should be started already"  # nosec B101
 
-        # TODO: filter by already running handlers after TestClient refactor
-        for handler in self._subscribers.values():
-            stream = handler.stream
-
-            log_context = handler.get_log_context(None)
+        for stream in filter(
+            lambda x: x.declare,
+            self._stream_builder.objects.values(),
+        ):
+            try:
+                await self.stream.add_stream(
+                    config=stream.config,
+                    subjects=stream.subjects,
+                )
+
+            except BadRequestError as e:  # noqa: PERF203
+                log_context = AsyncAPISubscriber.build_log_context(
+                    message=None,
+                    subject="",
+                    queue="",
+                    stream=stream.name,
+                )
+
+                if (
+                    e.description
+                    == "stream name already in use with a different configuration"
+                ):
+                    old_config = (await self.stream.stream_info(stream.name)).config
 
-            if stream is not None and stream.declare:
-                try:  # pragma: no branch
-                    await self.stream.add_stream(
+                    self._log(str(e), logging.WARNING, log_context)
+                    await self.stream.update_stream(
                         config=stream.config,
-                        subjects=stream.subjects,
+                        subjects=tuple(
+                            set(old_config.subjects or ()).union(stream.subjects)
+                        ),
                     )
 
-                except BadRequestError as e:
-                    if (
-                        e.description
-                        == "stream name already in use with a different configuration"
-                    ):
-                        old_config = (await self.stream.stream_info(stream.name)).config
-
-                        self._log(str(e), logging.WARNING, log_context)
-                        await self.stream.update_stream(
-                            config=stream.config,
-                            subjects=tuple(
-                                set(old_config.subjects or ()).union(stream.subjects)
-                            ),
-                        )
-
-                    else:  # pragma: no cover
-                        self._log(str(e), logging.ERROR, log_context, exc_info=e)
-
-                finally:
-                    # prevent from double declaration
-                    stream.declare = False
+                else:  # pragma: no cover
+                    self._log(str(e), logging.ERROR, log_context, exc_info=e)
 
+            finally:
+                # prevent from double declaration
+                stream.declare = False
+
+        # TODO: filter by already running handlers after TestClient refactor
+        for handler in self._subscribers.values():
             self._log(
                 f"`{handler.call_name}` waiting for messages",
-                extra=log_context,
+                extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
@@ -746,19 +763,38 @@
         )
 
     @override
     def setup_subscriber(  # type: ignore[override]
         self,
         subscriber: "AsyncAPISubscriber",
     ) -> None:
-        connection: Union["Client", "JetStreamContext", None] = None
+        connection: Union[
+            "Client",
+            "JetStreamContext",
+            KVBucketDeclarer,
+            OSBucketDeclarer,
+            None,
+        ] = None
 
-        connection = self._connection if subscriber.stream is None else self.stream
+        if getattr(subscriber, "kv_watch", None):
+            connection = self._kv_declarer
 
-        return super().setup_subscriber(subscriber, connection=connection)
+        elif getattr(subscriber, "obj_watch", None):
+            connection = self._os_declarer
+
+        elif getattr(subscriber, "stream", None):
+            connection = self.stream
+
+        else:
+            connection = self._connection
+
+        return super().setup_subscriber(
+            subscriber,
+            connection=connection,
+        )
 
     @override
     def setup_publisher(  # type: ignore[override]
         self,
         publisher: "AsyncAPIPublisher",
     ) -> None:
         producer: Optional[ProducerProto] = None
@@ -768,14 +804,74 @@
                 producer = self._js_producer
 
         elif self._producer is not None:
             producer = self._producer
 
         super().setup_publisher(publisher, producer=producer)
 
+    async def key_value(
+        self,
+        bucket: str,
+        *,
+        description: Optional[str] = None,
+        max_value_size: Optional[int] = None,
+        history: int = 1,
+        ttl: Optional[float] = None,  # in seconds
+        max_bytes: Optional[int] = None,
+        storage: Optional["StorageType"] = None,
+        replicas: int = 1,
+        placement: Optional["Placement"] = None,
+        republish: Optional["RePublish"] = None,
+        direct: Optional[bool] = None,
+        # custom
+        declare: bool = True,
+    ) -> "KeyValue":
+        assert self._kv_declarer, "Broker should be connected already."  # nosec B101
+
+        return await self._kv_declarer.create_key_value(
+            bucket=bucket,
+            description=description,
+            max_value_size=max_value_size,
+            history=history,
+            ttl=ttl,
+            max_bytes=max_bytes,
+            storage=storage,
+            replicas=replicas,
+            placement=placement,
+            republish=republish,
+            direct=direct,
+            declare=declare,
+        )
+
+    async def object_storage(
+        self,
+        bucket: str,
+        *,
+        description: Optional[str] = None,
+        ttl: Optional[float] = None,
+        max_bytes: Optional[int] = None,
+        storage: Optional["StorageType"] = None,
+        replicas: int = 1,
+        placement: Optional["Placement"] = None,
+        # custom
+        declare: bool = True,
+    ) -> "ObjectStore":
+        assert self._os_declarer, "Broker should be connected already."  # nosec B101
+
+        return await self._os_declarer.create_object_store(
+            bucket=bucket,
+            description=description,
+            ttl=ttl,
+            max_bytes=max_bytes,
+            storage=storage,
+            replicas=replicas,
+            placement=placement,
+            declare=declare,
+        )
+
     def _log_connection_broken(
         self,
         error_cb: Optional["ErrorCallback"] = None,
     ) -> "ErrorCallback":
         c = AsyncAPISubscriber.build_log_context(None, "")
 
         async def wrapper(err: Exception) -> None:
```

### Comparing `faststream-0.5.7/faststream/nats/broker/logging.py` & `faststream-0.5.8/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/broker/registrator.py` & `faststream-0.5.8/faststream/nats/broker/registrator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union, cast
 
 from nats.js import api
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
+from faststream.nats.helpers import StreamBuilder
 from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
+from faststream.nats.schemas import JStream, KvWatch, ObjWatch, PullSub
 from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.nats.subscriber.factory import create_subscriber
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
     from nats.aio.msg import Msg  # noqa: F401
 
     from faststream.broker.types import (
         CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
     from faststream.nats.message import NatsBatchMessage, NatsMessage
-    from faststream.nats.schemas import JStream, PullSub
 
 
 class NatsRegistrator(ABCBroker["Msg"]):
     """Includable to RabbitBroker router."""
 
     _subscribers: Dict[int, "AsyncAPISubscriber"]
     _publishers: Dict[int, "AsyncAPIPublisher"]
 
+    def __init__(self, **kwargs: Any) -> None:
+        self._stream_builder = StreamBuilder()
+
+        super().__init__(**kwargs)
+
     @override
     def subscriber(  # type: ignore[override]
         self,
         subject: Annotated[
             str,
             Doc("NATS subject to subscribe."),
         ],
@@ -98,20 +105,28 @@
             Optional[bool],
             Doc(
                 "Should be message delivered without payload, only headers and metadata."
             ),
         ] = None,
         # pull arguments
         pull_sub: Annotated[
-            Optional["PullSub"],
+            Union[bool, "PullSub"],
             Doc(
                 "NATS Pull consumer parameters container. "
                 "Should be used with `stream` only."
             ),
-        ] = None,
+        ] = False,
+        kv_watch: Annotated[
+            Union[str, "KvWatch", None],
+            Doc("KeyValue watch parameters container."),
+        ] = None,
+        obj_watch: Annotated[
+            Union[bool, "ObjWatch"],
+            Doc("ObjecStore watch parameters container."),
+        ] = False,
         inbox_prefix: Annotated[
             bytes,
             Doc(
                 "Prefix for generating unique inboxes, subjects with that prefix and NUID."
             ),
         ] = api.INBOX_PREFIX,
         # custom
@@ -162,14 +177,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -183,22 +204,27 @@
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> AsyncAPISubscriber:
         """Creates NATS subscriber object.
 
         You can use it as a handler decorator `@broker.subscriber(...)`.
         """
+        if stream := self._stream_builder.create(stream):
+            stream.add_subject(subject)
+
         subscriber = cast(
             AsyncAPISubscriber,
             super().subscriber(
-                AsyncAPISubscriber.create(  # type: ignore[arg-type]
+                create_subscriber(
                     subject=subject,
                     queue=queue,
                     stream=stream,
-                    pull_sub=pull_sub,
+                    pull_sub=PullSub.validate(pull_sub),
+                    kv_watch=KvWatch.validate(kv_watch),
+                    obj_watch=ObjWatch.validate(obj_watch),
                     max_workers=max_workers,
                     # extra args
                     pending_msgs_limit=pending_msgs_limit,
                     pending_bytes_limit=pending_bytes_limit,
                     max_msgs=max_msgs,
                     durable=durable,
                     config=config,
@@ -207,14 +233,15 @@
                     flow_control=flow_control,
                     deliver_policy=deliver_policy,
                     headers_only=headers_only,
                     inbox_prefix=inbox_prefix,
                     ack_first=ack_first,
                     # subscriber args
                     no_ack=no_ack,
+                    no_reply=no_reply,
                     retry=retry,
                     broker_middlewares=self._middlewares,
                     broker_dependencies=self._dependencies,
                     # AsyncAPI
                     title_=title,
                     description_=description,
                     include_in_schema=self._solve_include_in_schema(include_in_schema),
@@ -291,14 +318,17 @@
         """Creates long-living and AsyncAPI-documented publisher object.
 
         You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
         In such case publisher will publish your handler return value.
 
         Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
         """
+        if stream := self._stream_builder.create(stream):
+            stream.add_subject(subject)
+
         publisher = cast(
             AsyncAPIPublisher,
             super().publisher(
                 publisher=AsyncAPIPublisher.create(
                     subject=subject,
                     headers=headers,
                     # Core
```

### Comparing `faststream-0.5.7/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.8/faststream/nats/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         BrokerMiddleware,
         CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
     from faststream.nats.message import NatsBatchMessage, NatsMessage
-    from faststream.nats.schemas import JStream, PullSub
+    from faststream.nats.schemas import JStream, KvWatch, ObjWatch, PullSub
     from faststream.security import BaseSecurity
     from faststream.types import AnyDict, LoggerProto
 
 
 class NatsRouter(StreamRouter["Msg"]):
     """A class to represent a NATS router."""
 
@@ -647,14 +647,22 @@
         pull_sub: Annotated[
             Optional["PullSub"],
             Doc(
                 "NATS Pull consumer parameters container. "
                 "Should be used with `stream` only."
             ),
         ] = None,
+        kv_watch: Annotated[
+            Union[str, "KvWatch", None],
+            Doc("KeyValue watch parameters container."),
+        ] = None,
+        obj_watch: Annotated[
+            Union[bool, "ObjWatch"],
+            Doc("ObjecStore watch parameters container."),
+        ] = False,
         inbox_prefix: Annotated[
             bytes,
             Doc(
                 "Prefix for generating unique inboxes, subjects with that prefix and NUID."
             ),
         ] = api.INBOX_PREFIX,
         # custom
@@ -705,14 +713,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -862,24 +876,27 @@
                 config=config,
                 ordered_consumer=ordered_consumer,
                 idle_heartbeat=idle_heartbeat,
                 flow_control=flow_control,
                 deliver_policy=deliver_policy,
                 headers_only=headers_only,
                 pull_sub=pull_sub,
+                kv_watch=kv_watch,
+                obj_watch=obj_watch,
                 inbox_prefix=inbox_prefix,
                 ack_first=ack_first,
                 stream=stream,
                 parser=parser,
                 decoder=decoder,
                 middlewares=middlewares,
                 filter=filter,
                 max_workers=max_workers,
                 retry=retry,
                 no_ack=no_ack,
+                no_reply=no_reply,
                 title=title,
                 description=description,
                 include_in_schema=include_in_schema,
                 dependencies=dependencies,
                 # FastAPI args
                 response_model=response_model,
                 response_model_include=response_model_include,
```

### Comparing `faststream-0.5.7/faststream/nats/opentelemetry/middleware.py` & `faststream-0.5.8/faststream/nats/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/opentelemetry/provider.py` & `faststream-0.5.8/faststream/nats/opentelemetry/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import TYPE_CHECKING, List, Optional, Sequence, Union, overload
 
+from nats.aio.msg import Msg
 from opentelemetry.semconv.trace import SpanAttributes
 
 from faststream.__about__ import SERVICE_NAME
 from faststream.broker.types import MsgType
 from faststream.opentelemetry import TelemetrySettingsProvider
 from faststream.opentelemetry.consts import MESSAGING_DESTINATION_PUBLISH_NAME
 
 if TYPE_CHECKING:
-    from nats.aio.msg import Msg
-
     from faststream.broker.message import StreamMessage
     from faststream.types import AnyDict
 
 
 class BaseNatsTelemetrySettingsProvider(TelemetrySettingsProvider[MsgType]):
     __slots__ = ("messaging_system",)
 
@@ -103,12 +102,16 @@
 
 
 def telemetry_attributes_provider_factory(
     msg: Union["Msg", Sequence["Msg"], None],
 ) -> Union[
     NatsTelemetrySettingsProvider,
     NatsBatchTelemetrySettingsProvider,
+    None,
 ]:
     if isinstance(msg, Sequence):
         return NatsBatchTelemetrySettingsProvider()
-    else:
+    elif isinstance(msg, Msg) or msg is None:
         return NatsTelemetrySettingsProvider()
+    else:
+        # KeyValue and Object Storage watch cases
+        return None
```

### Comparing `faststream-0.5.7/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.8/faststream/nats/publisher/asyncapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional
 
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import nats
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.nats.helpers import stream_builder
 from faststream.nats.publisher.usecase import LogicPublisher
 
 if TYPE_CHECKING:
     from nats.aio.msg import Msg
 
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.nats.schemas.js_stream import JStream
@@ -54,28 +53,25 @@
     @classmethod
     def create(  # type: ignore[override]
         cls,
         *,
         subject: str,
         reply_to: str,
         headers: Optional[Dict[str, str]],
-        stream: Union[str, "JStream", None],
+        stream: Optional["JStream"],
         timeout: Optional[float],
         # Publisher args
         broker_middlewares: Iterable["BrokerMiddleware[Msg]"],
         middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> "AsyncAPIPublisher":
-        if stream := stream_builder.stream(stream):
-            stream.add_subject(subject)
-
         return cls(
             subject=subject,
             reply_to=reply_to,
             headers=headers,
             stream=stream,
             timeout=timeout,
             # Publisher args
```

### Comparing `faststream-0.5.7/faststream/nats/publisher/producer.py` & `faststream-0.5.8/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/publisher/usecase.py` & `faststream-0.5.8/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/schemas/js_stream.py` & `faststream-0.5.8/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.8/faststream/redis/testing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,196 +1,227 @@
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
+import re
+from typing import TYPE_CHECKING, Any, Optional, Sequence, Union
+from unittest.mock import AsyncMock, MagicMock
 
-from nats.aio.subscription import (
-    DEFAULT_SUB_PENDING_BYTES_LIMIT,
-    DEFAULT_SUB_PENDING_MSGS_LIMIT,
-)
-from nats.js.client import (
-    DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-    DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-)
 from typing_extensions import override
 
-from faststream.asyncapi.schema import (
-    Channel,
-    ChannelBinding,
-    CorrelationId,
-    Message,
-    Operation,
-)
-from faststream.asyncapi.schema.bindings import nats
-from faststream.asyncapi.utils import resolve_payloads
-from faststream.exceptions import SetupError
-from faststream.nats.helpers import stream_builder
-from faststream.nats.subscriber.usecase import (
-    BatchHandler,
-    DefaultHandler,
-    LogicSubscriber,
+from faststream.broker.message import gen_cor_id
+from faststream.exceptions import WRONG_PUBLISH_ARGS, SetupError
+from faststream.redis.broker.broker import RedisBroker
+from faststream.redis.message import (
+    BatchListMessage,
+    BatchStreamMessage,
+    DefaultListMessage,
+    DefaultStreamMessage,
+    PubSubMessage,
+    bDATA_KEY,
 )
+from faststream.redis.parser import RawMessage
+from faststream.redis.publisher.producer import RedisFastProducer
+from faststream.redis.schemas import INCORRECT_SETUP_MSG
+from faststream.redis.subscriber.factory import create_subscriber
+from faststream.testing.broker import TestBroker, call_handler
 
 if TYPE_CHECKING:
-    from fast_depends.dependencies import Depends
-    from nats.js import api
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
+    from faststream.types import AnyDict, SendableMessage
 
-    from faststream.broker.types import BrokerMiddleware
-    from faststream.nats.schemas import JStream, PullSub
-    from faststream.types import AnyDict
-
-
-class AsyncAPISubscriber(LogicSubscriber[Any]):
-    """A class to represent a NATS handler."""
-
-    def get_name(self) -> str:
-        return f"{self.subject}:{self.call_name}"
-
-    def get_schema(self) -> Dict[str, Channel]:
-        payloads = self.get_payloads()
-
-        return {
-            self.name: Channel(
-                description=self.description,
-                subscribe=Operation(
-                    message=Message(
-                        title=f"{self.name}:Message",
-                        payload=resolve_payloads(payloads),
-                        correlationId=CorrelationId(
-                            location="$message.header#/correlation_id"
-                        ),
-                    ),
-                ),
-                bindings=ChannelBinding(
-                    nats=nats.ChannelBinding(
-                        subject=self.subject,
-                        queue=self.queue or None,
-                    )
-                ),
-            )
-        }
+__all__ = ("TestRedisBroker",)
+
+
+class TestRedisBroker(TestBroker[RedisBroker]):
+    """A class to test Redis brokers."""
 
-    @override
     @staticmethod
-    def create(  # type: ignore[override]
+    def create_publisher_fake_subscriber(
+        broker: RedisBroker,
+        publisher: "AsyncAPIPublisher",
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
+        sub = broker.subscriber(**publisher.subscriber_property)
+
+        if not sub.calls:
+
+            @sub
+            def f(msg: Any) -> None:
+                pass
+
+            broker.setup_subscriber(sub)
+
+        return sub.calls[0].handler
+
+    @staticmethod
+    async def _fake_connect(  # type: ignore[override]
+        broker: RedisBroker,
+        *args: Any,
+        **kwargs: Any,
+    ) -> AsyncMock:
+        broker._producer = FakeProducer(broker)  # type: ignore[assignment]
+        connection = MagicMock()
+        connection.pubsub.side_effect = AsyncMock
+        return connection
+
+    @staticmethod
+    def remove_publisher_fake_subscriber(
+        broker: RedisBroker,
+        publisher: "AsyncAPIPublisher",
+    ) -> None:
+        broker._subscribers.pop(
+            hash(create_subscriber(**publisher.subscriber_property)),
+            None,
+        )
+
+
+class FakeProducer(RedisFastProducer):
+    def __init__(self, broker: RedisBroker) -> None:
+        self.broker = broker
+
+    @override
+    async def publish(  # type: ignore[override]
+        self,
+        message: "SendableMessage",
         *,
-        subject: str,
-        queue: str,
-        pending_msgs_limit: Optional[int],
-        pending_bytes_limit: Optional[int],
-        # Core args
-        max_msgs: int,
-        # JS args
-        durable: Optional[str],
-        config: Optional["api.ConsumerConfig"],
-        ordered_consumer: bool,
-        idle_heartbeat: Optional[float],
-        flow_control: bool,
-        deliver_policy: Optional["api.DeliverPolicy"],
-        headers_only: Optional[bool],
-        # pull args
-        pull_sub: Optional["PullSub"],
-        inbox_prefix: bytes,
-        # custom args
-        ack_first: bool,
-        max_workers: int,
-        stream: Union[str, "JStream", None],
-        # Subscriber args
-        no_ack: bool,
-        retry: Union[bool, int],
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[Any]"],
-        # AsyncAPI information
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> Union[
-        "AsyncAPIDefaultSubscriber",
-        "AsyncAPIBatchSubscriber",
-    ]:
-        if stream := stream_builder.stream(stream):
-            stream.add_subject(subject)
-
-        if pull_sub is not None and stream is None:
-            raise SetupError("Pull subscriber can be used only with a stream")
-
-        if stream:
-            # TODO: pull & queue warning
-            # TODO: push & durable warning
-
-            extra_options: AnyDict = {
-                "pending_msgs_limit": pending_msgs_limit
-                or DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-                "pending_bytes_limit": pending_bytes_limit
-                or DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-                "durable": durable,
-                "stream": stream.name,
-                "config": config,
-            }
-
-            if pull_sub is not None:
-                extra_options.update({"inbox_prefix": inbox_prefix})
-
-            else:
-                extra_options.update(
-                    {
-                        "ordered_consumer": ordered_consumer,
-                        "idle_heartbeat": idle_heartbeat,
-                        "flow_control": flow_control,
-                        "deliver_policy": deliver_policy,
-                        "headers_only": headers_only,
-                        "manual_ack": not ack_first,
-                    }
+        channel: Optional[str] = None,
+        list: Optional[str] = None,
+        stream: Optional[str] = None,
+        maxlen: Optional[int] = None,
+        headers: Optional["AnyDict"] = None,
+        reply_to: str = "",
+        correlation_id: Optional[str] = None,
+        rpc: bool = False,
+        rpc_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
+    ) -> Optional[Any]:
+        if rpc and reply_to:
+            raise WRONG_PUBLISH_ARGS
+
+        correlation_id = correlation_id or gen_cor_id()
+
+        body = build_message(
+            message=message,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+            headers=headers,
+        )
+
+        any_of = channel or list or stream
+        if any_of is None:
+            raise SetupError(INCORRECT_SETUP_MSG)
+
+        msg: Any = None
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            call = False
+
+            if channel and (ch := getattr(handler, "channel", None)) is not None:
+                call = bool(
+                    (not ch.pattern and ch.name == channel)
+                    or (
+                        ch.pattern
+                        and re.match(
+                            ch.name.replace(".", "\\.").replace("*", ".*"),
+                            channel,
+                        )
+                    )
+                )
+
+                msg = PubSubMessage(
+                    type="message",
+                    data=body,
+                    channel=channel,
+                    pattern=ch.pattern,
+                )
+
+            elif list and (ls := getattr(handler, "list_sub", None)) is not None:
+                if ls.batch:
+                    msg = BatchListMessage(
+                        type="blist",
+                        channel=list,
+                        data=[body],
+                    )
+
+                else:
+                    msg = DefaultListMessage(
+                        type="list",
+                        channel=list,
+                        data=body,
+                    )
+
+                call = list == ls.name
+
+            elif stream and (st := getattr(handler, "stream_sub", None)) is not None:
+                if st.batch:
+                    msg = BatchStreamMessage(
+                        type="bstream",
+                        channel=stream,
+                        data=[{bDATA_KEY: body}],
+                        message_ids=[],
+                    )
+                else:
+                    msg = DefaultStreamMessage(
+                        type="stream",
+                        channel=stream,
+                        data={bDATA_KEY: body},
+                        message_ids=[],
+                    )
+
+                call = stream == st.name
+
+            if call:
+                r = await call_handler(
+                    handler=handler,
+                    message=msg,
+                    rpc=rpc,
+                    rpc_timeout=rpc_timeout,
+                    raise_timeout=raise_timeout,
                 )
 
-        else:
-            extra_options = {
-                "pending_msgs_limit": pending_msgs_limit
-                or DEFAULT_SUB_PENDING_MSGS_LIMIT,
-                "pending_bytes_limit": pending_bytes_limit
-                or DEFAULT_SUB_PENDING_BYTES_LIMIT,
-                "max_msgs": max_msgs,
-            }
-
-        if getattr(pull_sub, "batch", False):
-            return AsyncAPIBatchSubscriber(
-                extra_options=extra_options,
-                # basic args
-                pull_sub=pull_sub,
-                subject=subject,
-                queue=queue,
-                stream=stream,
-                # Subscriber args
-                no_ack=no_ack,
-                retry=retry,
-                broker_dependencies=broker_dependencies,
-                broker_middlewares=broker_middlewares,
-                # AsyncAPI information
-                title_=title_,
-                description_=description_,
-                include_in_schema=include_in_schema,
-            )
-
-        else:
-            return AsyncAPIDefaultSubscriber(
-                max_workers=max_workers,
-                extra_options=extra_options,
-                # basic args
-                pull_sub=pull_sub,
-                subject=subject,
-                queue=queue,
-                stream=stream,
-                # Subscriber args
-                no_ack=no_ack,
-                retry=retry,
-                broker_dependencies=broker_dependencies,
-                broker_middlewares=broker_middlewares,
-                # AsyncAPI information
-                title_=title_,
-                description_=description_,
-                include_in_schema=include_in_schema,
-            )
+                if rpc:  # pragma: no branch
+                    return r
+
+        return None
 
+    async def publish_batch(
+        self,
+        *msgs: "SendableMessage",
+        list: str,
+        headers: Optional["AnyDict"] = None,
+        correlation_id: Optional[str] = None,
+    ) -> None:
+        correlation_id = correlation_id or gen_cor_id()
+
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            if (
+                list_sub := getattr(handler, "list_sub", None)
+            ) and list_sub.name == list:
+                await call_handler(
+                    handler=handler,
+                    message=BatchListMessage(
+                        type="blist",
+                        channel=list,
+                        data=[
+                            build_message(
+                                m,
+                                correlation_id=correlation_id,
+                                headers=headers,
+                            )
+                            for m in msgs
+                        ],
+                    ),
+                )
 
-class AsyncAPIDefaultSubscriber(DefaultHandler, AsyncAPISubscriber):
-    """One-message consumer with AsyncAPI methods."""
+        return None
 
 
-class AsyncAPIBatchSubscriber(BatchHandler, AsyncAPISubscriber):
-    """Batch-message consumer with AsyncAPI methods."""
+def build_message(
+    message: Union[Sequence["SendableMessage"], "SendableMessage"],
+    *,
+    correlation_id: str,
+    reply_to: str = "",
+    headers: Optional["AnyDict"] = None,
+) -> bytes:
+    data = RawMessage.encode(
+        message=message,
+        reply_to=reply_to,
+        headers=headers,
+        correlation_id=correlation_id,
+    )
+    return data
```

### Comparing `faststream-0.5.7/faststream/nats/subscriber/usecase.py` & `faststream-0.5.8/faststream/redis/subscriber/usecase.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,466 +1,742 @@
 import asyncio
 from abc import abstractmethod
 from contextlib import suppress
+from copy import deepcopy
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Sequence,
-    Union,
-    cast,
+    Tuple,
 )
 
 import anyio
-from fast_depends.dependencies import Depends
-from nats.errors import ConnectionClosedError, TimeoutError
-from typing_extensions import Annotated, Doc, override
+from redis.asyncio.client import PubSub as RPubSub
+from redis.asyncio.client import Redis
+from redis.exceptions import ResponseError
+from typing_extensions import TypeAlias, override
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.fake import FakePublisher
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import CustomCallable, MsgType
-from faststream.exceptions import NOT_CONNECTED_YET, SetupError
-from faststream.nats.parser import BatchParser, JsParser, NatsParser
-from faststream.nats.schemas.js_stream import compile_nats_wildcard
-from faststream.types import AnyDict, LoggerProto, SendableMessage
+from faststream.redis.message import (
+    BatchListMessage,
+    BatchStreamMessage,
+    DefaultListMessage,
+    DefaultStreamMessage,
+    PubSubMessage,
+    UnifyRedisDict,
+)
+from faststream.redis.parser import (
+    RedisBatchListParser,
+    RedisBatchStreamParser,
+    RedisListParser,
+    RedisPubSubParser,
+    RedisStreamParser,
+)
+from faststream.redis.schemas import ListSub, PubSub, StreamSub
 
 if TYPE_CHECKING:
-    from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
-    from nats.aio.client import Client
-    from nats.aio.msg import Msg
-    from nats.aio.subscription import Subscription
-    from nats.js import JetStreamContext
+    from fast_depends.dependencies import Depends
 
-    from faststream.broker.message import StreamMessage
+    from faststream.broker.message import StreamMessage as BrokerStreamMessage
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         AsyncCallable,
         BrokerMiddleware,
+        CustomCallable,
     )
-    from faststream.nats.schemas import JStream, PullSub
-    from faststream.types import Decorator
+    from faststream.types import AnyDict, Decorator, LoggerProto
+
+
+TopicName: TypeAlias = bytes
+Offset: TypeAlias = bytes
 
 
-class LogicSubscriber(SubscriberUsecase[MsgType]):
-    """A class to represent a NATS handler."""
+class LogicSubscriber(SubscriberUsecase[UnifyRedisDict]):
+    """A class to represent a Redis handler."""
 
-    subscription: Union[
-        None,
-        "Subscription",
-        "JetStreamContext.PushSubscription",
-        "JetStreamContext.PullSubscription",
-    ]
-    producer: Optional["ProducerProto"]
-    _connection: Union["Client", "JetStreamContext", None]
+    _client: Optional["Redis[bytes]"]
 
     def __init__(
         self,
         *,
-        subject: str,
-        extra_options: Optional[AnyDict],
-        queue: str,
-        stream: Optional["JStream"],
-        pull_sub: Optional["PullSub"],
-        # Subscriber args
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
+        # Subscriber args
         no_ack: bool,
-        retry: Union[bool, int],
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
-        _, path = compile_nats_wildcard(subject)
-
-        self.subject = path
-        self.queue = queue
-
-        self.stream = stream
-        self.pull_sub = pull_sub
-        self.extra_options = extra_options or {}
-
         super().__init__(
             default_parser=default_parser,
             default_decoder=default_decoder,
-            # Propagated args
+            # Propagated options
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
-            # AsyncAPI args
+            # AsyncAPI
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-        self._connection = None
-        self.subscription = None
-        self.producer = None
-        self.tasks: List["asyncio.Task[Any]"] = []
+        self._client = None
+        self.task: Optional["asyncio.Task[None]"] = None
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
-        connection: Union["Client", "JetStreamContext"],
+        connection: Optional["Redis[bytes]"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
         extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
         _call_decorators: Iterable["Decorator"],
     ) -> None:
-        self._connection = connection
+        self._client = connection
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
             _call_decorators=_call_decorators,
         )
 
-    async def start(self) -> None:
-        """Create NATS subscription and start consume tasks."""
-        assert self._connection, NOT_CONNECTED_YET  # nosec B101
-        await super().start()
-        await self._create_subscription(connection=self._connection)
-
-    async def close(self) -> None:
-        """Clean up handler subscription, cancel consume task in graceful mode."""
-        await super().close()
-
-        if self.subscription is not None:
-            await self.subscription.unsubscribe()
-            self.subscription = None
-
-        for task in self.tasks:
-            if not task.done():
-                task.cancel()
-        self.tasks = []
-
-    @abstractmethod
-    async def _create_subscription(
-        self,
-        *,
-        connection: Union["Client", "JetStreamContext"],
-    ) -> None:
-        """Create NATS subscription object to consume messages."""
-        raise NotImplementedError()
-
     def _make_response_publisher(
         self,
-        message: Annotated[
-            "StreamMessage[Any]",
-            Doc("Message requiring reply"),
-        ],
+        message: "BrokerStreamMessage[UnifyRedisDict]",
     ) -> Sequence[FakePublisher]:
-        """Create FakePublisher object to use it as one of `publishers` in `self.consume` scope."""
-        if not message.reply_to or self._producer is None:
+        if self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
-                    "subject": message.reply_to,
+                    "channel": message.reply_to,
                 },
             ),
         )
 
-    def __hash__(self) -> int:
-        return self.get_routing_hash(self.subject)
+    @override
+    async def start(  # type: ignore[override]
+        self,
+        *args: Any,
+    ) -> None:
+        await super().start()
 
-    @staticmethod
-    def get_routing_hash(
-        subject: Annotated[
-            str,
-            Doc("NATS subject to consume messages"),
-        ],
-    ) -> int:
-        """Get handler hash by outer data.
+        start_signal = anyio.Event()
+        self.task = asyncio.create_task(self._consume(*args, start_signal=start_signal))
+
+        await start_signal.wait()
 
-        Using to find handler in `broker.handlers` dictionary.
-        """
-        return hash(subject)
+    async def _consume(self, *args: Any, start_signal: anyio.Event) -> None:
+        connected = True
+
+        while self.running:
+            with suppress(Exception):
+                try:
+                    await self._get_msgs(*args)
+
+                except Exception:
+                    if connected:
+                        connected = False
+                    await anyio.sleep(5)
+
+                else:
+                    if not connected:
+                        connected = True
+
+                finally:
+                    if not start_signal.is_set():
+                        start_signal.set()
+
+    @abstractmethod
+    async def _get_msgs(self, *args: Any) -> None:
+        raise NotImplementedError()
+
+    async def close(self) -> None:
+        await super().close()
+
+        if self.task is not None and not self.task.done():
+            self.task.cancel()
+        self.task = None
 
     @staticmethod
     def build_log_context(
-        message: Annotated[
-            Optional["StreamMessage[Any]"],
-            Doc("Message which we are building context for"),
-        ],
-        subject: Annotated[
-            str,
-            Doc("NATS subject we are listening"),
-        ],
-        *,
-        queue: Annotated[
-            str,
-            Doc("Using queue group name"),
-        ] = "",
-        stream: Annotated[
-            Optional["JStream"],
-            Doc("Stream object we are listening"),
-        ] = None,
+        message: Optional["BrokerStreamMessage[Any]"],
+        channel: str = "",
     ) -> Dict[str, str]:
-        """Static method to build log context out of `self.consume` scope."""
         return {
-            "subject": subject,
-            "queue": queue,
-            "stream": getattr(stream, "name", ""),
+            "channel": channel,
             "message_id": getattr(message, "message_id", ""),
         }
 
+
+class ChannelSubscriber(LogicSubscriber):
+    subscription: Optional[RPubSub]
+
+    def __init__(
+        self,
+        *,
+        channel: "PubSub",
+        # Subscriber args
+        no_ack: bool,
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        parser = RedisPubSubParser(pattern=channel.path_regex)
+        super().__init__(
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
+            # Propagated options
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
+
+        self.channel = channel
+        self.subscription = None
+
+    def __hash__(self) -> int:
+        return hash(self.channel)
+
     def get_log_context(
         self,
-        message: Annotated[
-            Optional["StreamMessage[Any]"],
-            Doc("Message which we are building context for"),
-        ],
+        message: Optional["BrokerStreamMessage[Any]"],
     ) -> Dict[str, str]:
-        """Log context factory using in `self.consume` scope."""
         return self.build_log_context(
             message=message,
-            subject=self.subject,
-            queue=self.queue,
-            stream=self.stream,
+            channel=self.channel.name,
         )
 
-    def add_prefix(self, prefix: str) -> None:
-        """Include Subscriber in router."""
-        self.subject = "".join((prefix, self.subject))
+    @override
+    async def start(self) -> None:
+        assert self._client, "You should setup subscriber at first."  # nosec B101
+
+        self.subscription = psub = self._client.pubsub()
+
+        if self.channel.pattern:
+            await psub.psubscribe(self.channel.name)
+        else:
+            await psub.subscribe(self.channel.name)
+
+        await super().start(psub)
+
+    async def close(self) -> None:
+        if self.subscription is not None:
+            await self.subscription.unsubscribe()
+            await self.subscription.aclose()  # type: ignore[attr-defined]
+            self.subscription = None
+
+        await super().close()
 
+    async def _get_msgs(self, psub: RPubSub) -> None:
+        raw_msg = await psub.get_message(
+            ignore_subscribe_messages=True,
+            timeout=self.channel.polling_interval,
+        )
+
+        if raw_msg:
+            msg = PubSubMessage(
+                type=raw_msg["type"],
+                data=raw_msg["data"],
+                channel=raw_msg["channel"].decode(),
+                pattern=raw_msg["pattern"],
+            )
+            await self.consume(msg)  # type: ignore[arg-type]
 
-class DefaultHandler(LogicSubscriber["Msg"]):
-    """One-message consumer class."""
+    def add_prefix(self, prefix: str) -> None:
+        new_ch = deepcopy(self.channel)
+        new_ch.name = "".join((prefix, new_ch.name))
+        self.channel = new_ch
 
-    send_stream: "MemoryObjectSendStream[Msg]"
-    receive_stream: "MemoryObjectReceiveStream[Msg]"
 
+class _ListHandlerMixin(LogicSubscriber):
     def __init__(
         self,
         *,
-        max_workers: int,
-        # default args
-        subject: str,
-        queue: str,
-        stream: Optional["JStream"],
-        pull_sub: Optional["PullSub"],
-        extra_options: Optional[AnyDict],
+        list: ListSub,
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         # Subscriber args
         no_ack: bool,
-        retry: Union[bool, int],
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable["BrokerMiddleware[Msg]"],
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
-        parser_: Union[NatsParser, JsParser] = (
-            NatsParser(pattern=subject) if stream is None else JsParser(pattern=subject)
-        )
-
         super().__init__(
-            subject=subject,
-            queue=queue,
-            stream=stream,
-            pull_sub=pull_sub,
-            extra_options=extra_options,
-            # subscriber args
-            default_parser=parser_.parse_message,
-            default_decoder=parser_.decode_message,
-            # Propagated args
+            default_parser=default_parser,
+            default_decoder=default_decoder,
+            # Propagated options
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
-            # AsyncAPI args
-            description_=description_,
+            # AsyncAPI
             title_=title_,
+            description_=description_,
             include_in_schema=include_in_schema,
         )
 
-        self.max_workers = max_workers
+        self.list_sub = list
+
+    def __hash__(self) -> int:
+        return hash(self.list_sub)
 
-        self.send_stream, self.receive_stream = anyio.create_memory_object_stream(
-            max_buffer_size=max_workers
+    def get_log_context(
+        self,
+        message: Optional["BrokerStreamMessage[Any]"],
+    ) -> Dict[str, str]:
+        return self.build_log_context(
+            message=message,
+            channel=self.list_sub.name,
         )
-        self.limiter = anyio.Semaphore(max_workers)
 
-    async def _create_subscription(
+    @override
+    async def _consume(  # type: ignore[override]
         self,
+        client: "Redis[bytes]",
         *,
-        connection: Union["Client", "JetStreamContext"],
+        start_signal: "anyio.Event",
     ) -> None:
-        """Create NATS subscription and start consume task."""
-        cb: Callable[["Msg"], Awaitable[Any]]
-        if self.max_workers > 1:
-            self.tasks.append(asyncio.create_task(self._serve_consume_queue()))
-            cb = self.__put_msg
-        else:
-            cb = self.consume
+        start_signal.set()
+        await super()._consume(client, start_signal=start_signal)
 
-        if self.pull_sub is not None:
-            connection = cast("JetStreamContext", connection)
+    @override
+    async def start(self) -> None:
+        assert self._client, "You should setup subscriber at first."  # nosec B101
+        await super().start(self._client)
+
+    def add_prefix(self, prefix: str) -> None:
+        new_list = deepcopy(self.list_sub)
+        new_list.name = "".join((prefix, new_list.name))
+        self.list_sub = new_list
+
+
+class ListSubscriber(_ListHandlerMixin):
+    def __init__(
+        self,
+        *,
+        list: ListSub,
+        # Subscriber args
+        no_ack: bool,
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        parser = RedisListParser()
+        super().__init__(
+            list=list,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
+            # Propagated options
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
 
-            if self.stream is None:
-                raise SetupError("Pull subscriber can be used only with a stream")
+    async def _get_msgs(self, client: "Redis[bytes]") -> None:
+        raw_msg = await client.lpop(name=self.list_sub.name)
 
-            self.subscription = await connection.pull_subscribe(
-                subject=self.subject,
-                **self.extra_options,
+        if raw_msg:
+            message = DefaultListMessage(
+                type="list",
+                data=raw_msg,
+                channel=self.list_sub.name,
             )
-            self.tasks.append(asyncio.create_task(self._consume_pull(cb=cb)))
+
+            await self.consume(message)  # type: ignore[arg-type]
 
         else:
-            self.subscription = await connection.subscribe(
-                subject=self.subject,
-                queue=self.queue,
-                cb=cb,  # type: ignore[arg-type]
-                **self.extra_options,
-            )
+            await anyio.sleep(self.list_sub.polling_interval)
+
 
-    async def _serve_consume_queue(
+class BatchListSubscriber(_ListHandlerMixin):
+    def __init__(
         self,
+        *,
+        list: ListSub,
+        # Subscriber args
+        no_ack: bool,
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Endless task consuming messages from in-memory queue.
+        parser = RedisBatchListParser()
+        super().__init__(
+            list=list,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
+            # Propagated options
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
+
+    async def _get_msgs(self, client: "Redis[bytes]") -> None:
+        raw_msgs = await client.lpop(
+            name=self.list_sub.name,
+            count=self.list_sub.max_records,
+        )
+
+        if raw_msgs:
+            msg = BatchListMessage(
+                type="blist",
+                channel=self.list_sub.name,
+                data=raw_msgs,
+            )
+
+            await self.consume(msg)  # type: ignore[arg-type]
+
+        else:
+            await anyio.sleep(self.list_sub.polling_interval)
 
-        Suitable to batch messages by amount, timestamps, etc and call `consume` for this batches.
-        """
-        async with anyio.create_task_group() as tg:
-            async for msg in self.receive_stream:
-                tg.start_soon(self.__consume_msg, msg)
 
-    async def _consume_pull(
+class _StreamHandlerMixin(LogicSubscriber):
+    def __init__(
         self,
-        cb: Callable[["Msg"], Awaitable[SendableMessage]],
+        *,
+        stream: StreamSub,
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
+        # Subscriber args
+        no_ack: bool,
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Endless task consuming messages using NATS Pull subscriber."""
-        assert self.pull_sub  # nosec B101
+        super().__init__(
+            default_parser=default_parser,
+            default_decoder=default_decoder,
+            # Propagated options
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
 
-        sub = cast("JetStreamContext.PullSubscription", self.subscription)
+        self.stream_sub = stream
+        self.last_id = stream.last_id
 
-        while self.running:  # pragma: no branch
-            messages = []
-            with suppress(TimeoutError, ConnectionClosedError):
-                messages = await sub.fetch(
-                    batch=self.pull_sub.batch_size,
-                    timeout=self.pull_sub.timeout,
+    def __hash__(self) -> int:
+        return hash(self.stream_sub)
+
+    def get_log_context(
+        self,
+        message: Optional["BrokerStreamMessage[Any]"],
+    ) -> Dict[str, str]:
+        return self.build_log_context(
+            message=message,
+            channel=self.stream_sub.name,
+        )
+
+    @override
+    async def start(self) -> None:
+        assert self._client, "You should setup subscriber at first."  # nosec B101
+        client = self._client
+
+        self.extra_watcher_options.update(
+            redis=client,
+            group=self.stream_sub.group,
+        )
+
+        stream = self.stream_sub
+
+        read: Callable[
+            [str],
+            Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ],
+        ]
+
+        if stream.group and stream.consumer:
+            try:
+                await client.xgroup_create(
+                    name=stream.name,
+                    id=self.last_id,
+                    groupname=stream.group,
+                    mkstream=True,
                 )
+            except ResponseError as e:
+                if "already exists" not in str(e):
+                    raise e
+
+            def read(
+                _: str,
+            ) -> Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ]:
+                return client.xreadgroup(
+                    groupname=stream.group,
+                    consumername=stream.consumer,
+                    streams={stream.name: ">"},
+                    count=stream.max_records,
+                    block=stream.polling_interval,
+                    noack=stream.no_ack,
+                )
+
+        else:
+
+            def read(
+                last_id: str,
+            ) -> Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ]:
+                return client.xread(
+                    {stream.name: last_id},
+                    block=stream.polling_interval,
+                    count=stream.max_records,
+                )
+
+        await super().start(read)
+
+    def add_prefix(self, prefix: str) -> None:
+        new_stream = deepcopy(self.stream_sub)
+        new_stream.name = "".join((prefix, new_stream.name))
+        self.stream_sub = new_stream
 
-            if messages:
-                async with anyio.create_task_group() as tg:
-                    for msg in messages:
-                        tg.start_soon(cb, msg)
 
-    async def __consume_msg(
+class StreamSubscriber(_StreamHandlerMixin):
+    def __init__(
         self,
-        msg: "Msg",
+        *,
+        stream: StreamSub,
+        # Subscriber args
+        no_ack: bool,
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Proxy method to call `self.consume` with semaphore block."""
-        async with self.limiter:
-            await self.consume(msg)
-
-    async def __put_msg(self, msg: "Msg") -> None:
-        """Proxy method to put msg into in-memory queue with semaphore block."""
-        async with self.limiter:
-            await self.send_stream.send(msg)
+        parser = RedisStreamParser()
+        super().__init__(
+            stream=stream,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
+            # Propagated options
+            no_ack=no_ack,
+            no_reply=no_reply,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
 
+    async def _get_msgs(
+        self,
+        read: Callable[
+            [str],
+            Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ],
+        ],
+    ) -> None:
+        for stream_name, msgs in await read(self.last_id):
+            if msgs:
+                self.last_id = msgs[-1][0].decode()
+
+                for message_id, raw_msg in msgs:
+                    msg = DefaultStreamMessage(
+                        type="stream",
+                        channel=stream_name.decode(),
+                        message_ids=[message_id],
+                        data=raw_msg,
+                    )
 
-class BatchHandler(LogicSubscriber[List["Msg"]]):
-    """Batch-message consumer class."""
+                    await self.consume(msg)  # type: ignore[arg-type]
 
-    pull_sub: "PullSub"
-    stream: "JStream"
 
+class BatchStreamSubscriber(_StreamHandlerMixin):
     def __init__(
         self,
         *,
-        # default args
-        subject: str,
-        queue: str,
-        stream: Optional["JStream"],
-        pull_sub: Optional["PullSub"],
-        extra_options: Optional[AnyDict],
+        stream: StreamSub,
         # Subscriber args
         no_ack: bool,
-        retry: Union[bool, int],
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable["BrokerMiddleware[List[Msg]]"],
+        no_reply: bool,
+        retry: bool,
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
-        parser = BatchParser(pattern=subject)
-
+        parser = RedisBatchStreamParser()
         super().__init__(
-            subject=subject,
-            queue=queue,
             stream=stream,
-            pull_sub=pull_sub,
-            extra_options=extra_options,
-            # subscriber args
-            default_parser=parser.parse_batch,
-            default_decoder=parser.decode_batch,
-            # Propagated args
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
+            # Propagated options
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
-            # AsyncAPI args
-            description_=description_,
+            # AsyncAPI
             title_=title_,
+            description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    @override
-    async def _create_subscription(  # type: ignore[override]
+    async def _get_msgs(
         self,
-        *,
-        connection: "JetStreamContext",
+        read: Callable[
+            [str],
+            Awaitable[
+                Tuple[Tuple[bytes, Tuple[Tuple[bytes, Dict[bytes, bytes]], ...]], ...],
+            ],
+        ],
     ) -> None:
-        """Create NATS subscription and start consume task."""
-        self.subscription = await connection.pull_subscribe(
-            subject=self.subject,
-            **self.extra_options,
-        )
-        self.tasks.append(asyncio.create_task(self._consume_pull()))
-
-    async def _consume_pull(self) -> None:
-        """Endless task consuming messages using NATS Pull subscriber."""
-        assert self.subscription, "You should call `create_subscription` at first."  # nosec B101
-
-        sub = cast("JetStreamContext.PullSubscription", self.subscription)
-
-        while self.running:  # pragma: no branch
-            with suppress(TimeoutError, ConnectionClosedError):
-                messages = await sub.fetch(
-                    batch=self.pull_sub.batch_size,
-                    timeout=self.pull_sub.timeout,
+        for stream_name, msgs in await read(self.last_id):
+            if msgs:
+                self.last_id = msgs[-1][0].decode()
+
+                data: List[Dict[bytes, bytes]] = []
+                ids: List[bytes] = []
+                for message_id, i in msgs:
+                    data.append(i)
+                    ids.append(message_id)
+
+                msg = BatchStreamMessage(
+                    type="bstream",
+                    channel=stream_name.decode(),
+                    data=data,
+                    message_ids=ids,
                 )
 
-                if messages:
-                    await self.consume(messages)
+                await self.consume(msg)  # type: ignore[arg-type]
```

### Comparing `faststream-0.5.7/faststream/opentelemetry/middleware.py` & `faststream-0.5.8/faststream/opentelemetry/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,17 @@
 
 
 class BaseTelemetryMiddleware(BaseMiddleware):
     def __init__(
         self,
         *,
         tracer: "Tracer",
-        settings_provider_factory: Callable[[Any], TelemetrySettingsProvider[Any]],
+        settings_provider_factory: Callable[
+            [Any], Optional[TelemetrySettingsProvider[Any]]
+        ],
         metrics_container: _MetricsContainer,
         msg: Optional[Any] = None,
     ) -> None:
         self.msg = msg
 
         self._tracer = tracer
         self._metrics = metrics_container
@@ -117,15 +119,16 @@
     async def publish_scope(
         self,
         call_next: "AsyncFunc",
         msg: Any,
         *args: Any,
         **kwargs: Any,
     ) -> Any:
-        provider = self.__settings_provider
+        if (provider := self.__settings_provider) is None:
+            return await call_next(msg, *args, **kwargs)
 
         headers = kwargs.pop("headers", {}) or {}
         current_context = context.get_current()
         destination_name = provider.get_publish_destination_name(kwargs)
 
         trace_attributes = provider.get_publish_attrs_from_kwargs(kwargs)
         metrics_attributes = {
@@ -178,15 +181,16 @@
         return result
 
     async def consume_scope(
         self,
         call_next: "AsyncFuncAny",
         msg: "StreamMessage[Any]",
     ) -> Any:
-        provider = self.__settings_provider
+        if (provider := self.__settings_provider) is None:
+            return await call_next(msg)
 
         current_context = propagate.extract(msg.headers)
         destination_name = provider.get_consume_destination_name(msg)
 
         trace_attributes = provider.get_consume_attrs_from_message(msg)
         metrics_attributes = {
             SpanAttributes.MESSAGING_SYSTEM: provider.messaging_system,
@@ -254,15 +258,17 @@
         "_metrics",
         "_settings_provider_factory",
     )
 
     def __init__(
         self,
         *,
-        settings_provider_factory: Callable[[Any], TelemetrySettingsProvider[Any]],
+        settings_provider_factory: Callable[
+            [Any], Optional[TelemetrySettingsProvider[Any]]
+        ],
         tracer_provider: Optional["TracerProvider"] = None,
         meter_provider: Optional["MeterProvider"] = None,
         meter: Optional["Meter"] = None,
         include_messages_counters: bool = False,
     ) -> None:
         self._tracer = _get_tracer(tracer_provider)
         self._meter = _get_meter(meter_provider, meter)
```

### Comparing `faststream-0.5.7/faststream/opentelemetry/provider.py` & `faststream-0.5.8/faststream/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/__init__.py` & `faststream-0.5.8/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/annotations.py` & `faststream-0.5.8/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/message.py` & `faststream-0.5.8/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/parser.py` & `faststream-0.5.8/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/router.py` & `faststream-0.5.8/faststream/rabbit/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,20 @@
             Union[bool, int],
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -277,14 +283,15 @@
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
             no_ack=no_ack,
+            no_reply=no_reply,
             title=title,
             description=description,
             include_in_schema=include_in_schema,
         )
 
 
 class RabbitRouter(
```

### Comparing `faststream-0.5.7/faststream/rabbit/security.py` & `faststream-0.5.8/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/testing.py` & `faststream-0.5.8/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/utils.py` & `faststream-0.5.8/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/broker/broker.py` & `faststream-0.5.8/faststream/rabbit/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/broker/logging.py` & `faststream-0.5.8/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/broker/registrator.py` & `faststream-0.5.8/faststream/rabbit/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from faststream.rabbit.publisher.asyncapi import AsyncAPIPublisher
 from faststream.rabbit.publisher.usecase import PublishKwargs
 from faststream.rabbit.schemas import (
     RabbitExchange,
     RabbitQueue,
 )
 from faststream.rabbit.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.rabbit.subscriber.factory import create_subscriber
 
 if TYPE_CHECKING:
     from aio_pika import IncomingMessage  # noqa: F401
     from aio_pika.abc import DateType, HeadersType, TimeoutType
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
@@ -93,14 +94,20 @@
             Union[bool, int],
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -113,21 +120,22 @@
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> AsyncAPISubscriber:
         subscriber = cast(
             AsyncAPISubscriber,
             super().subscriber(
-                AsyncAPISubscriber.create(
+                create_subscriber(
                     queue=RabbitQueue.validate(queue),
                     exchange=RabbitExchange.validate(exchange),
                     consume_args=consume_args,
                     reply_config=reply_config,
                     # subscriber args
                     no_ack=no_ack,
+                    no_reply=no_reply,
                     retry=retry,
                     broker_middlewares=self._middlewares,
                     broker_dependencies=self._dependencies,
                     # AsyncAPI
                     title_=title,
                     description_=description,
                     include_in_schema=self._solve_include_in_schema(include_in_schema),
```

### Comparing `faststream-0.5.7/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.8/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/fastapi/router.py` & `faststream-0.5.8/faststream/rabbit/fastapi/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,14 +524,20 @@
             Union[bool, int],
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -680,14 +686,15 @@
                 dependencies=dependencies,
                 parser=parser,
                 decoder=decoder,
                 middlewares=middlewares,
                 filter=filter,
                 retry=retry,
                 no_ack=no_ack,
+                no_reply=no_reply,
                 title=title,
                 description=description,
                 include_in_schema=include_in_schema,
                 # FastAPI args
                 response_model=response_model,
                 response_model_include=response_model_include,
                 response_model_exclude=response_model_exclude,
```

### Comparing `faststream-0.5.7/faststream/rabbit/opentelemetry/middleware.py` & `faststream-0.5.8/faststream/rabbit/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/opentelemetry/provider.py` & `faststream-0.5.8/faststream/rabbit/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.8/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/publisher/producer.py` & `faststream-0.5.8/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.8/faststream/rabbit/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/schemas/constants.py` & `faststream-0.5.8/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.8/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/schemas/queue.py` & `faststream-0.5.8/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/schemas/reply.py` & `faststream-0.5.8/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.8/faststream/rabbit/subscriber/usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         *,
         queue: "RabbitQueue",
         exchange: Optional["RabbitExchange"],
         consume_args: Optional["AnyDict"],
         reply_config: Optional["ReplyConfig"],
         # Subscriber args
         no_ack: bool,
+        no_reply: bool,
         retry: Union[bool, int],
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[IncomingMessage]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
@@ -66,14 +67,15 @@
         parser = AioPikaParser(pattern=queue.path_regex)
 
         super().__init__(
             default_parser=parser.parse_message,
             default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
+            no_reply=no_reply,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
@@ -169,15 +171,15 @@
 
             self._queue_obj = None
 
     def _make_response_publisher(
         self,
         message: "StreamMessage[Any]",
     ) -> Sequence["FakePublisher"]:
-        if not message.reply_to or self._producer is None:
+        if self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
                     **self.reply_config,
```

### Comparing `faststream-0.5.7/faststream/redis/__init__.py` & `faststream-0.5.8/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/annotations.py` & `faststream-0.5.8/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/message.py` & `faststream-0.5.8/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/parser.py` & `faststream-0.5.8/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/router.py` & `faststream-0.5.8/faststream/redis/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,14 +159,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -189,14 +195,15 @@
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
             no_ack=no_ack,
+            no_reply=no_reply,
             title=title,
             description=description,
             include_in_schema=include_in_schema,
         )
 
 
 class RedisRouter(
```

### Comparing `faststream-0.5.7/faststream/redis/security.py` & `faststream-0.5.8/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/broker/broker.py` & `faststream-0.5.8/faststream/redis/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Mapping,
     Optional,
     Type,
     Union,
 )
 from urllib.parse import urlparse
 
-from fast_depends.dependencies import Depends
 from redis.asyncio.client import Redis
 from redis.asyncio.connection import (
     Connection,
     ConnectionPool,
     DefaultParser,
     Encoder,
     parse_url,
```

### Comparing `faststream-0.5.7/faststream/redis/broker/logging.py` & `faststream-0.5.8/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/broker/registrator.py` & `faststream-0.5.8/faststream/redis/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
 from faststream.redis.message import UnifyRedisDict
 from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
 from faststream.redis.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.redis.subscriber.factory import SubsciberType, create_subscriber
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
     from faststream.redis.message import UnifyRedisMessage
     from faststream.redis.publisher.asyncapi import PublisherType
     from faststream.redis.schemas import ListSub, PubSub, StreamSub
-    from faststream.redis.subscriber.asyncapi import SubsciberType
     from faststream.types import AnyDict
 
 
 class RedisRegistrator(ABCBroker[UnifyRedisDict]):
     """Includable to RabbitBroker router."""
 
     _subscribers: Dict[int, "SubsciberType"]
@@ -80,14 +80,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -100,20 +106,21 @@
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> AsyncAPISubscriber:
         subscriber = cast(
             AsyncAPISubscriber,
             super().subscriber(
-                AsyncAPISubscriber.create(
+                create_subscriber(
                     channel=channel,
                     list=list,
                     stream=stream,
                     # subscriber args
                     no_ack=no_ack,
+                    no_reply=no_reply,
                     retry=retry,
                     broker_middlewares=self._middlewares,
                     broker_dependencies=self._dependencies,
                     # AsyncAPI
                     title_=title,
                     description_=description,
                     include_in_schema=self._solve_include_in_schema(include_in_schema),
```

### Comparing `faststream-0.5.7/faststream/redis/fastapi/__init__.py` & `faststream-0.5.8/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.8/faststream/redis/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,14 +484,20 @@
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
+        no_reply: Annotated[
+            bool,
+            Doc(
+                "Whether to disable **FastStream** RPC and Reply To auto responses or not."
+            ),
+        ] = False,
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
@@ -644,14 +650,15 @@
                 dependencies=dependencies,
                 parser=parser,
                 decoder=decoder,
                 middlewares=middlewares,
                 filter=filter,
                 retry=retry,
                 no_ack=no_ack,
+                no_reply=no_reply,
                 title=title,
                 description=description,
                 include_in_schema=include_in_schema,
                 # FastAPI args
                 response_model=response_model,
                 response_model_include=response_model_include,
                 response_model_exclude=response_model_exclude,
```

### Comparing `faststream-0.5.7/faststream/redis/opentelemetry/middleware.py` & `faststream-0.5.8/faststream/redis/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/opentelemetry/provider.py` & `faststream-0.5.8/faststream/redis/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.8/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/publisher/producer.py` & `faststream-0.5.8/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/publisher/usecase.py` & `faststream-0.5.8/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/schemas/list_sub.py` & `faststream-0.5.8/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/schemas/proto.py` & `faststream-0.5.8/faststream/redis/schemas/proto.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,18 +13,14 @@
     @property
     @abstractmethod
     def channel_binding(self) -> "redis.ChannelBinding": ...
 
     @abstractmethod
     def get_payloads(self) -> Any: ...
 
-    @staticmethod
-    @abstractmethod
-    def create() -> Any: ...
-
 
 def validate_options(
     *,
     channel: Union["PubSub", str, None],
     list: Union["ListSub", str, None],
     stream: Union["StreamSub", str, None],
 ) -> None:
```

### Comparing `faststream-0.5.7/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.8/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.8/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/testing/app.py` & `faststream-0.5.8/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/testing/broker.py` & `faststream-0.5.8/faststream/testing/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,16 @@
                 )
 
                 connect_only = False
 
         self.connect_only = connect_only
 
     async def __aenter__(self) -> Broker:
+        # TODO: remove useless middlewares filter
+
         middlewares = tuple(
             filter(
                 lambda x: not isinstance(x, CriticalLogMiddleware),
                 self.broker._middlewares,
             )
         )
 
@@ -86,14 +88,15 @@
 
         self._ctx = self._create_ctx()
         return await self._ctx.__aenter__()
 
     async def __aexit__(self, *args: Any) -> None:
         await self._ctx.__aexit__(*args)
 
+        # TODO: remove useless middlewares filter
         middlewares: Tuple["BrokerMiddleware[Any]", ...] = (
             CriticalLogMiddleware(  # type: ignore[arg-type]
                 logger=self.broker.logger,
                 log_level=self.broker._msg_log_level,
             ),
             *self.broker._middlewares,
         )
```

### Comparing `faststream-0.5.7/faststream/utils/ast.py` & `faststream-0.5.8/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/classes.py` & `faststream-0.5.8/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/data.py` & `faststream-0.5.8/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/functions.py` & `faststream-0.5.8/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/no_cast.py` & `faststream-0.5.8/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/path.py` & `faststream-0.5.8/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/context/builders.py` & `faststream-0.5.8/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/context/repository.py` & `faststream-0.5.8/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/faststream/utils/context/types.py` & `faststream-0.5.8/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/scripts/build-docs-pre-commit.sh` & `faststream-0.5.8/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/scripts/lint-pre-commit.sh` & `faststream-0.5.8/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/scripts/set_variables.sh` & `faststream-0.5.8/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/scripts/static-pre-commit.sh` & `faststream-0.5.8/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/LICENSE` & `faststream-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/README.md` & `faststream-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.7/pyproject.toml` & `faststream-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -75,55 +75,56 @@
 
 otel = ["opentelemetry-sdk>=1.24.0,<2.0.0"]
 
 # dev dependencies
 optionals = ["faststream[rabbit,kafka,confluent,nats,redis,otel]"]
 
 devdocs = [
-    "mkdocs-material==9.5.21",
+    "mkdocs-material==9.5.24",
     "mkdocs-static-i18n==1.2.3",
     "mdx-include==1.4.2",
     "mkdocstrings[python]==0.25.1",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.5",
     "mike==2.1.1",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",                      # includes with variables
-    "mkdocs-glightbox==0.3.7",                          # img zoom
+    "mkdocs-glightbox==0.4.0",                          # img zoom
     "pillow",                                           # required for mkdocs-glightbo
     "cairosvg",                                         # required for mkdocs-glightbo
     "requests",                                         # using in CI, do not pin it
     "griffe-typingdoc==0.2.5",                          # Annotated[..., Doc("")] support
 ]
 
 types = [
     "faststream[optionals]",
     "mypy==1.10.0",
     # mypy extensions
+    "types-Deprecated",
     "types-PyYAML",
     "types-setuptools",
     "types-ujson",
     "types-redis",
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
 ]
 
 lint = [
     "faststream[types]",
     "ruff==0.4.4",
     "bandit==1.7.8",
-    "semgrep==1.70.0",
+    "semgrep==1.73.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
     "coverage[toml]==7.5.1",
-    "pytest==8.2.0",
-    "pytest-asyncio==0.23.6",
+    "pytest==8.2.1",
+    "pytest-asyncio==0.23.7",
     "dirty-equals==0.7.1.post0",
 ]
 
 testing = [
     "faststream[test-core]",
     "fastapi==0.111.0",
     "pydantic-settings>=2.0.0,<3.0.0",
```

### Comparing `faststream-0.5.7/PKG-INFO` & `faststream-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.7
+Version: 0.5.8
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -58,52 +58,53 @@
 Requires-Dist: email-validator==2.1.1; extra == 'dev'
 Requires-Dist: fastapi==0.111.0; extra == 'dev'
 Requires-Dist: griffe-typingdoc==0.2.5; extra == 'dev'
 Requires-Dist: httpx==0.27.0; extra == 'dev'
 Requires-Dist: mdx-include==1.4.2; extra == 'dev'
 Requires-Dist: mike==2.1.1; extra == 'dev'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.5; extra == 'dev'
-Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'dev'
+Requires-Dist: mkdocs-glightbox==0.4.0; extra == 'dev'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'dev'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
-Requires-Dist: mkdocs-material==9.5.21; extra == 'dev'
+Requires-Dist: mkdocs-material==9.5.24; extra == 'dev'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'dev'
 Requires-Dist: mkdocs-static-i18n==1.2.3; extra == 'dev'
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == 'dev'
 Requires-Dist: mypy==1.10.0; extra == 'dev'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'dev'
 Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'dev'
 Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'dev'
-Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
-Requires-Dist: pytest==8.2.0; extra == 'dev'
+Requires-Dist: pytest-asyncio==0.23.7; extra == 'dev'
+Requires-Dist: pytest==8.2.1; extra == 'dev'
 Requires-Dist: pyyaml==6.0.1; extra == 'dev'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'dev'
 Requires-Dist: requests; extra == 'dev'
 Requires-Dist: ruff==0.4.4; extra == 'dev'
-Requires-Dist: semgrep==1.70.0; extra == 'dev'
+Requires-Dist: semgrep==1.73.0; extra == 'dev'
+Requires-Dist: types-deprecated; extra == 'dev'
 Requires-Dist: types-docutils; extra == 'dev'
 Requires-Dist: types-pygments; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Requires-Dist: types-redis; extra == 'dev'
 Requires-Dist: types-setuptools; extra == 'dev'
 Requires-Dist: types-ujson; extra == 'dev'
 Requires-Dist: watchfiles==0.21.0; extra == 'dev'
 Provides-Extra: devdocs
 Requires-Dist: cairosvg; extra == 'devdocs'
 Requires-Dist: griffe-typingdoc==0.2.5; extra == 'devdocs'
 Requires-Dist: mdx-include==1.4.2; extra == 'devdocs'
 Requires-Dist: mike==2.1.1; extra == 'devdocs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.5; extra == 'devdocs'
-Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
+Requires-Dist: mkdocs-glightbox==0.4.0; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
-Requires-Dist: mkdocs-material==9.5.21; extra == 'devdocs'
+Requires-Dist: mkdocs-material==9.5.24; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
 Requires-Dist: mkdocs-static-i18n==1.2.3; extra == 'devdocs'
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == 'devdocs'
 Requires-Dist: pillow; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
@@ -115,15 +116,16 @@
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'lint'
 Requires-Dist: mypy==1.10.0; extra == 'lint'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'lint'
 Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'lint'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'lint'
 Requires-Dist: ruff==0.4.4; extra == 'lint'
-Requires-Dist: semgrep==1.70.0; extra == 'lint'
+Requires-Dist: semgrep==1.73.0; extra == 'lint'
+Requires-Dist: types-deprecated; extra == 'lint'
 Requires-Dist: types-docutils; extra == 'lint'
 Requires-Dist: types-pygments; extra == 'lint'
 Requires-Dist: types-pyyaml; extra == 'lint'
 Requires-Dist: types-redis; extra == 'lint'
 Requires-Dist: types-setuptools; extra == 'lint'
 Requires-Dist: types-ujson; extra == 'lint'
 Provides-Extra: nats
@@ -140,36 +142,37 @@
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
 Requires-Dist: coverage[toml]==7.5.1; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
-Requires-Dist: pytest-asyncio==0.23.6; extra == 'test-core'
-Requires-Dist: pytest==8.2.0; extra == 'test-core'
+Requires-Dist: pytest-asyncio==0.23.7; extra == 'test-core'
+Requires-Dist: pytest==8.2.1; extra == 'test-core'
 Provides-Extra: testing
 Requires-Dist: coverage[toml]==7.5.1; extra == 'testing'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'testing'
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
 Requires-Dist: fastapi==0.111.0; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
-Requires-Dist: pytest-asyncio==0.23.6; extra == 'testing'
-Requires-Dist: pytest==8.2.0; extra == 'testing'
+Requires-Dist: pytest-asyncio==0.23.7; extra == 'testing'
+Requires-Dist: pytest==8.2.1; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
 Requires-Dist: watchfiles==0.21.0; extra == 'testing'
 Provides-Extra: types
 Requires-Dist: aio-pika<10,>=9; extra == 'types'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'types'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'types'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'types'
 Requires-Dist: mypy==1.10.0; extra == 'types'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'types'
 Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'types'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'types'
+Requires-Dist: types-deprecated; extra == 'types'
 Requires-Dist: types-docutils; extra == 'types'
 Requires-Dist: types-pygments; extra == 'types'
 Requires-Dist: types-pyyaml; extra == 'types'
 Requires-Dist: types-redis; extra == 'types'
 Requires-Dist: types-setuptools; extra == 'types'
 Requires-Dist: types-ujson; extra == 'types'
 Description-Content-Type: text/markdown
```

