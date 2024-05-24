# Comparing `tmp/agentuniverse-0.0.6.tar.gz` & `tmp/agentuniverse-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentuniverse-0.0.6.tar", max compression
+gzip compressed data, was "agentuniverse-0.0.6.dev1.tar", max compression
```

## Comparing `agentuniverse-0.0.6.tar` & `agentuniverse-0.0.6.dev1.tar`

### file list

```diff
@@ -1,184 +1,185 @@
--rw-r--r--   0        0        0    11335 2024-04-02 12:08:01.834225 agentuniverse-0.0.6/LICENSE
--rw-r--r--   0        0        0     1527 2024-04-19 04:40:08.243214 agentuniverse-0.0.6/README_PYPI.md
--rw-r--r--   0        0        0      164 2024-04-02 03:12:13.474920 agentuniverse-0.0.6/agentuniverse/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.835519 agentuniverse-0.0.6/agentuniverse/agent/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835723 agentuniverse-0.0.6/agentuniverse/agent/action/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835932 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.836127 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0        0        0      972 2024-04-26 07:36:14.016798 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0        0        0     4270 2024-05-07 11:44:48.809512 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0        0        0     3097 2024-04-26 03:46:54.112257 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0        0        0      655 2024-04-26 03:46:54.140111 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge_manager.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837041 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837386 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0        0        0     1160 2024-04-26 03:46:54.147189 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0        0        0     1651 2024-04-26 07:36:14.018108 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0        0        0     1568 2024-04-26 03:46:54.126577 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0        0        0     1460 2024-04-26 03:46:54.173810 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0        0        0     1478 2024-04-26 07:36:14.018626 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0        0        0      552 2024-04-26 03:46:54.132260 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/reader.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.838782 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0        0        0     5872 2024-05-07 11:44:48.809653 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0        0        0     2206 2024-05-07 11:44:48.809765 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0        0        0      662 2024-04-02 12:08:01.839355 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0        0        0     3842 2024-05-07 11:44:48.809881 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/store.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.839707 agentuniverse-0.0.6/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0        0        0      276 2024-04-02 12:08:01.839872 agentuniverse-0.0.6/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0        0        0     3868 2024-04-26 07:36:14.019652 agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0        0        0      626 2024-04-26 03:46:54.149120 agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0        0        0     5469 2024-05-09 06:23:55.005965 agentuniverse-0.0.6/agentuniverse/agent/agent.py
--rw-r--r--   0        0        0      639 2024-04-26 03:44:12.686183 agentuniverse-0.0.6/agentuniverse/agent/agent_manager.py
--rw-r--r--   0        0        0      526 2024-04-02 12:08:01.840672 agentuniverse-0.0.6/agentuniverse/agent/agent_model.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.840834 agentuniverse-0.0.6/agentuniverse/agent/default/__init__.py
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.006641 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/__init__.py
--rw-r--r--   0        0        0     1257 2024-05-09 06:23:55.006784 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1446 2024-05-09 06:23:55.006896 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     3126 2024-05-09 06:23:55.006988 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/executing_agent.py
--rw-r--r--   0        0        0      367 2024-05-09 06:23:55.007062 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/executing_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.007720 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/__init__.py
--rw-r--r--   0        0        0     1499 2024-05-09 06:23:55.007805 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1866 2024-05-09 06:23:55.007888 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     2030 2024-05-09 06:23:55.007964 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/expressing_agent.py
--rw-r--r--   0        0        0      365 2024-05-09 06:23:55.008036 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008209 agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/__init__.py
--rw-r--r--   0        0        0     1289 2024-05-09 06:23:55.008282 agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/peer_agent.py
--rw-r--r--   0        0        0      374 2024-05-09 06:23:55.008415 agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/peer_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008732 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-09 06:23:55.008817 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1613 2024-05-09 06:23:55.008890 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     1623 2024-05-09 06:23:55.008965 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/planning_agent.py
--rw-r--r--   0        0        0      353 2024-05-09 06:23:55.009031 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/planning_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009190 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/__init__.py
--rw-r--r--   0        0        0      769 2024-05-09 06:23:55.009270 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0      884 2024-05-09 06:23:55.009355 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     1333 2024-05-09 06:23:55.009442 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/rag_agent.py
--rw-r--r--   0        0        0      276 2024-05-09 06:23:55.009511 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/rag_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009871 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/__init__.py
--rw-r--r--   0        0        0     1222 2024-05-09 06:23:55.009950 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1412 2024-05-09 06:23:55.010031 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     1954 2024-05-09 06:23:55.010184 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
--rw-r--r--   0        0        0      359 2024-05-09 06:23:55.010255 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
--rw-r--r--   0        0        0      657 2024-04-02 12:08:01.841347 agentuniverse-0.0.6/agentuniverse/agent/input_object.py
--rw-r--r--   0        0        0      173 2024-04-09 07:08:39.103227 agentuniverse-0.0.6/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-26 09:03:49.031293 agentuniverse-0.0.6/agentuniverse/agent/memory/chat_memory.py
--rw-r--r--   0        0        0      174 2024-04-26 09:03:49.031587 agentuniverse-0.0.6/agentuniverse/agent/memory/default/__init__.py
--rw-r--r--   0        0        0      845 2024-04-26 09:03:49.032072 agentuniverse-0.0.6/agentuniverse/agent/memory/default/default_memory.py
--rw-r--r--   0        0        0      321 2024-04-26 09:03:49.032468 agentuniverse-0.0.6/agentuniverse/agent/memory/default/default_memory.yaml
--rw-r--r--   0        0        0      402 2024-04-01 06:19:56.174000 agentuniverse-0.0.6/agentuniverse/agent/memory/enum.py
--rw-r--r--   0        0        0     7689 2024-04-26 09:03:49.032798 agentuniverse-0.0.6/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0        0        0     3054 2024-04-26 07:36:14.022682 agentuniverse-0.0.6/agentuniverse/agent/memory/memory.py
--rw-r--r--   0        0        0      635 2024-04-26 03:46:54.130633 agentuniverse-0.0.6/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0        0        0      508 2024-04-09 16:15:17.142565 agentuniverse-0.0.6/agentuniverse/agent/memory/message.py
--rw-r--r--   0        0        0      754 2024-04-26 09:03:49.033037 agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
--rw-r--r--   0        0        0      896 2024-04-26 09:03:49.033338 agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_en_prompt.yaml
--rw-r--r--   0        0        0      572 2024-04-02 12:08:01.842690 agentuniverse-0.0.6/agentuniverse/agent/output_object.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842823 agentuniverse-0.0.6/agentuniverse/agent/plan/__init__.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842962 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/__init__.py
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.142958 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0        0        0     3670 2024-05-09 06:23:55.010687 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0        0        0      195 2024-04-26 03:46:54.158656 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.144134 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0        0        0     3599 2024-05-09 06:23:55.010948 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0        0        0      200 2024-04-26 03:46:54.188023 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
--rw-r--r--   0        0        0      158 2024-04-09 16:15:17.145177 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0        0        0     8919 2024-05-09 06:23:55.011260 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0        0        0      170 2024-04-26 03:46:54.113707 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0        0        0     6438 2024-05-09 06:23:55.011722 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0        0        0      659 2024-04-26 03:46:54.185023 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner_manager.py
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.145969 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0        0        0     3599 2024-05-09 06:23:55.012182 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0        0        0      190 2024-04-26 03:46:54.166967 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
--rw-r--r--   0        0        0      157 2024-04-02 12:08:01.843408 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0        0        0     3397 2024-05-09 06:23:55.012606 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0        0        0      165 2024-04-26 03:46:54.135943 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.147020 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0        0        0     3603 2024-05-09 06:23:55.012846 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0        0        0      195 2024-04-26 03:46:54.178755 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
--rw-r--r--   0        0        0        0 2024-04-02 12:08:01.843939 agentuniverse-0.0.6/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0        0        0     1944 2024-04-02 12:08:01.844114 agentuniverse-0.0.6/agentuniverse/agent_serve/service.py
--rw-r--r--   0        0        0     3152 2024-04-26 03:46:54.144088 agentuniverse-0.0.6/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0        0        0     1161 2024-04-02 12:08:01.844424 agentuniverse-0.0.6/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0        0        0      402 2024-04-02 12:08:01.844558 agentuniverse-0.0.6/agentuniverse/agent_serve/service_manager.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844690 agentuniverse-0.0.6/agentuniverse/agent_serve/web/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844823 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.845006 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0        0        0     1075 2024-04-02 12:08:01.845143 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0        0        0     5473 2024-04-26 15:29:30.264684 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0        0        0     5019 2024-05-15 03:58:25.722266 agentuniverse-0.0.6/agentuniverse/agent_serve/web/flask_server.py
--rw-r--r--   0        0        0     2351 2024-04-26 15:29:30.265783 agentuniverse-0.0.6/agentuniverse/agent_serve/web/gunicorn_server.py
--rw-r--r--   0        0        0     9311 2024-04-26 09:03:49.038432 agentuniverse-0.0.6/agentuniverse/agent_serve/web/request_task.py
--rw-r--r--   0        0        0      164 2024-04-26 09:03:49.038779 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-05-15 03:58:25.722567 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/__init__.py
--rw-r--r--   0        0        0      617 2024-05-15 03:58:25.722726 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto
--rw-r--r--   0        0        0     2092 2024-05-15 03:58:25.722866 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py
--rw-r--r--   0        0        0     5979 2024-05-15 03:58:25.723032 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py
--rw-r--r--   0        0        0     5033 2024-05-15 03:58:25.723168 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py
--rw-r--r--   0        0        0     3307 2024-05-15 03:58:25.723368 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/rpc_server.py
--rw-r--r--   0        0        0     1146 2024-04-02 12:08:01.845635 agentuniverse-0.0.6/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0        0        0      822 2024-04-26 15:29:30.266263 agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0        0        0     2679 2024-04-26 15:29:30.266639 agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_util.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846346 agentuniverse-0.0.6/agentuniverse/base/__init__.py
--rw-r--r--   0        0        0    11557 2024-05-15 03:58:25.723582 agentuniverse-0.0.6/agentuniverse/base/agentuniverse.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846609 agentuniverse-0.0.6/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0        0        0      515 2024-04-02 12:08:01.846840 agentuniverse-0.0.6/agentuniverse/base/annotation/singleton.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.847286 agentuniverse-0.0.6/agentuniverse/base/component/__init__.py
--rw-r--r--   0        0        0     1081 2024-04-26 03:46:54.108902 agentuniverse-0.0.6/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0        0        0     1264 2024-04-26 03:46:54.107724 agentuniverse-0.0.6/agentuniverse/base/component/component_base.py
--rw-r--r--   0        0        0     4380 2024-04-26 09:03:49.040235 agentuniverse-0.0.6/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0        0        0      626 2024-04-26 09:03:49.040545 agentuniverse-0.0.6/agentuniverse/base/component/component_enum.py
--rw-r--r--   0        0        0     2576 2024-04-26 03:46:54.137220 agentuniverse-0.0.6/agentuniverse/base/component/component_manager_base.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.848825 agentuniverse-0.0.6/agentuniverse/base/config/__init__.py
--rw-r--r--   0        0        0      165 2024-04-02 12:08:01.849235 agentuniverse-0.0.6/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0        0        0     4173 2024-04-26 09:03:49.040952 agentuniverse-0.0.6/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0        0        0     1006 2024-04-26 03:46:54.105041 agentuniverse-0.0.6/agentuniverse/base/config/application_configer/application_config_manager.py
--rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850062 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0        0        0     2811 2024-04-26 09:03:49.041321 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/component_configer.py
--rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850500 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0        0        0     2599 2024-04-26 03:46:54.162861 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0        0        0     2053 2024-04-26 03:46:54.189422 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0        0        0     3272 2024-04-26 03:46:54.100009 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0        0        0     2540 2024-04-26 03:46:54.198928 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0        0        0     2392 2024-04-26 03:46:54.181023 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0        0        0     1889 2024-04-26 09:03:49.041670 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/prompt_configer.py
--rw-r--r--   0        0        0     2192 2024-04-26 03:46:54.165777 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0        0        0      423 2024-04-02 12:08:01.852070 agentuniverse-0.0.6/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0        0        0     4846 2024-04-26 15:29:30.267459 agentuniverse-0.0.6/agentuniverse/base/config/configer.py
--rw-r--r--   0        0        0      163 2024-04-02 12:08:01.852534 agentuniverse-0.0.6/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0        0        0      707 2024-04-26 03:55:12.618569 agentuniverse-0.0.6/agentuniverse/base/config/custom_configer/custom_key_configer.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.852949 agentuniverse-0.0.6/agentuniverse/base/context/__init__.py
--rw-r--r--   0        0        0     1447 2024-04-26 03:46:54.182246 agentuniverse-0.0.6/agentuniverse/base/context/framework_context.py
--rw-r--r--   0        0        0     2768 2024-04-26 03:46:54.110018 agentuniverse-0.0.6/agentuniverse/base/context/framework_context_manager.py
--rw-r--r--   0        0        0      174 2024-04-26 09:03:49.042097 agentuniverse-0.0.6/agentuniverse/base/prompt/__init__.py
--rw-r--r--   0        0        0      286 2024-04-26 09:03:49.042363 agentuniverse-0.0.6/agentuniverse/base/prompt/combine_cn_prompt.yaml
--rw-r--r--   0        0        0      318 2024-04-26 09:03:49.042631 agentuniverse-0.0.6/agentuniverse/base/prompt/combine_en_prompt.yaml
--rw-r--r--   0        0        0      253 2024-04-26 09:03:49.042893 agentuniverse-0.0.6/agentuniverse/base/prompt/summary_cn_prompt.yaml
--rw-r--r--   0        0        0      272 2024-04-26 09:03:49.043156 agentuniverse-0.0.6/agentuniverse/base/prompt/summary_en_prompt.yaml
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.853924 agentuniverse-0.0.6/agentuniverse/base/util/__init__.py
--rw-r--r--   0        0        0      307 2024-04-02 12:08:01.854131 agentuniverse-0.0.6/agentuniverse/base/util/env_util.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.854373 agentuniverse-0.0.6/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0        0        0     6600 2024-04-26 03:42:29.579851 agentuniverse-0.0.6/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0        0        0     5132 2024-04-02 12:08:01.854819 agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0        0        0     6395 2024-04-26 03:42:21.826133 agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0        0        0      502 2024-04-26 03:42:41.042298 agentuniverse-0.0.6/agentuniverse/base/util/memory_util.py
--rw-r--r--   0        0        0     6776 2024-05-09 06:23:55.013451 agentuniverse-0.0.6/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0        0        0      715 2024-04-02 12:08:01.855496 agentuniverse-0.0.6/agentuniverse/base/util/system_util.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.855704 agentuniverse-0.0.6/agentuniverse/llm/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.855856 agentuniverse-0.0.6/agentuniverse/llm/default/__init__.py
--rw-r--r--   0        0        0     1352 2024-04-26 09:03:49.043837 agentuniverse-0.0.6/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0        0        0      223 2024-04-26 09:03:49.044133 agentuniverse-0.0.6/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0        0        0     5625 2024-05-09 06:23:55.013593 agentuniverse-0.0.6/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0        0        0     5601 2024-05-15 03:58:25.723788 agentuniverse-0.0.6/agentuniverse/llm/llm.py
--rw-r--r--   0        0        0      619 2024-04-26 03:46:54.138842 agentuniverse-0.0.6/agentuniverse/llm/llm_manager.py
--rw-r--r--   0        0        0      408 2024-04-26 09:03:49.045322 agentuniverse-0.0.6/agentuniverse/llm/llm_output.py
--rw-r--r--   0        0        0     8294 2024-05-15 03:58:25.723994 agentuniverse-0.0.6/agentuniverse/llm/openai_llm.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.856945 agentuniverse-0.0.6/agentuniverse/prompt/__init__.py
--rw-r--r--   0        0        0      548 2024-04-26 07:36:14.033265 agentuniverse-0.0.6/agentuniverse/prompt/enum.py
--rw-r--r--   0        0        0     2891 2024-05-09 06:23:55.015272 agentuniverse-0.0.6/agentuniverse/prompt/prompt.py
--rw-r--r--   0        0        0      741 2024-04-26 09:03:49.046141 agentuniverse-0.0.6/agentuniverse/prompt/prompt_manager.py
--rw-r--r--   0        0        0     1120 2024-05-15 03:58:25.724188 agentuniverse-0.0.6/agentuniverse/prompt/prompt_model.py
--rw-r--r--   0        0        0      164 2024-04-02 03:12:13.477398 agentuniverse-0.0.6/agentuniverse_connector/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 03:13:12.638584 agentuniverse-0.0.6/agentuniverse_extension/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.857428 agentuniverse-0.0.6/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0        0        0     7321 2024-04-02 12:08:01.857588 agentuniverse-0.0.6/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0        0        0     2581 2024-05-15 05:26:47.421174 agentuniverse-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 agentuniverse-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-04-02 12:08:01.834225 agentuniverse-0.0.6.dev1/LICENSE
+-rw-r--r--   0        0        0     1527 2024-04-19 04:40:08.243214 agentuniverse-0.0.6.dev1/README_PYPI.md
+-rw-r--r--   0        0        0      164 2024-04-02 03:12:13.474920 agentuniverse-0.0.6.dev1/agentuniverse/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.835519 agentuniverse-0.0.6.dev1/agentuniverse/agent/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835723 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835932 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.836127 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0        0        0      972 2024-05-24 05:33:08.351840 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0        0        0     4270 2024-05-24 05:33:08.352083 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0        0        0     3097 2024-04-26 03:46:54.112257 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0        0        0      655 2024-04-26 03:46:54.140111 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge_manager.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837041 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837386 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0        0        0     1160 2024-04-26 03:46:54.147189 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0        0        0     1651 2024-05-24 05:33:08.352329 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0        0        0     1568 2024-04-26 03:46:54.126577 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0        0        0     1460 2024-04-26 03:46:54.173810 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0        0        0     1478 2024-05-24 05:33:08.352566 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0        0        0      552 2024-04-26 03:46:54.132260 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/reader.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.838782 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0        0        0     5872 2024-05-24 05:33:08.352856 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0        0        0     2206 2024-05-24 05:33:08.353136 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0        0        0      662 2024-04-02 12:08:01.839355 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0        0        0     3842 2024-05-07 11:44:48.809881 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/store.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.839707 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-02 12:08:01.839872 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0        0        0     3868 2024-05-24 05:33:08.353396 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0        0        0      626 2024-04-26 03:46:54.149120 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0        0        0     5806 2024-05-21 09:31:45.014048 agentuniverse-0.0.6.dev1/agentuniverse/agent/agent.py
+-rw-r--r--   0        0        0      639 2024-04-26 03:44:12.686183 agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0        0        0      526 2024-04-02 12:08:01.840672 agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_model.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.840834 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.006641 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-09 06:23:55.006784 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1446 2024-05-09 06:23:55.006896 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     3123 2024-05-21 09:31:45.014435 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/executing_agent.py
+-rw-r--r--   0        0        0      367 2024-05-09 06:23:55.007062 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/executing_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.007720 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/__init__.py
+-rw-r--r--   0        0        0     1499 2024-05-09 06:23:55.007805 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1866 2024-05-09 06:23:55.007888 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     2094 2024-05-21 09:31:45.014618 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/expressing_agent.py
+-rw-r--r--   0        0        0      365 2024-05-09 06:23:55.008036 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008209 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-21 09:31:45.014795 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/peer_agent.py
+-rw-r--r--   0        0        0      374 2024-05-09 06:23:55.008415 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/peer_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008732 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-09 06:23:55.008817 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1613 2024-05-09 06:23:55.008890 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1687 2024-05-21 09:31:45.014972 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/planning_agent.py
+-rw-r--r--   0        0        0      353 2024-05-09 06:23:55.009031 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/planning_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009190 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-09 06:23:55.009270 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0      884 2024-05-09 06:23:55.009355 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1377 2024-05-21 09:31:45.015159 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/rag_agent.py
+-rw-r--r--   0        0        0      276 2024-05-09 06:23:55.009511 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/rag_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009871 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/__init__.py
+-rw-r--r--   0        0        0     1222 2024-05-09 06:23:55.009950 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1412 2024-05-09 06:23:55.010031 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     2011 2024-05-21 09:31:45.015355 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
+-rw-r--r--   0        0        0      359 2024-05-09 06:23:55.010255 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
+-rw-r--r--   0        0        0      657 2024-04-02 12:08:01.841347 agentuniverse-0.0.6.dev1/agentuniverse/agent/input_object.py
+-rw-r--r--   0        0        0      173 2024-04-09 07:08:39.103227 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0        0        0     3907 2024-05-24 05:33:08.353668 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/chat_memory.py
+-rw-r--r--   0        0        0      174 2024-04-26 09:03:49.031587 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-26 09:03:49.032072 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/default_memory.py
+-rw-r--r--   0        0        0      321 2024-04-26 09:03:49.032468 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/default_memory.yaml
+-rw-r--r--   0        0        0      402 2024-04-01 06:19:56.174000 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0        0        0     7689 2024-04-26 09:03:49.032798 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0        0        0     3054 2024-05-24 05:33:08.353951 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0        0        0      635 2024-04-26 03:46:54.130633 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0        0        0     2005 2024-05-24 05:33:08.354185 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/message.py
+-rw-r--r--   0        0        0      754 2024-04-26 09:03:49.033037 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
+-rw-r--r--   0        0        0      896 2024-04-26 09:03:49.033338 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_en_prompt.yaml
+-rw-r--r--   0        0        0      572 2024-04-02 12:08:01.842690 agentuniverse-0.0.6.dev1/agentuniverse/agent/output_object.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842823 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842962 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.142958 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0        0        0     3691 2024-05-21 09:31:45.017893 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0        0        0      195 2024-04-26 03:46:54.158656 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.144134 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0        0        0     3620 2024-05-21 09:31:45.018077 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0        0        0      200 2024-04-26 03:46:54.188023 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+-rw-r--r--   0        0        0      158 2024-04-09 16:15:17.145177 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0        0        0     8940 2024-05-21 09:31:45.018315 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0        0        0      170 2024-04-26 03:46:54.113707 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0        0        0     6449 2024-05-21 09:31:45.018505 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0        0        0      659 2024-04-26 03:46:54.185023 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner_manager.py
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.145969 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0        0        0     3620 2024-05-21 09:31:45.018670 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0        0        0      190 2024-04-26 03:46:54.166967 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-02 12:08:01.843408 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0        0        0     3680 2024-05-21 09:31:45.018865 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0        0        0      165 2024-04-26 03:46:54.135943 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.147020 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0        0        0     3626 2024-05-21 09:31:45.019044 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0        0        0      195 2024-04-26 03:46:54.178755 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+-rw-r--r--   0        0        0        0 2024-04-02 12:08:01.843939 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0        0        0     1944 2024-04-02 12:08:01.844114 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service.py
+-rw-r--r--   0        0        0     3152 2024-04-26 03:46:54.144088 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0        0        0     1161 2024-04-02 12:08:01.844424 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0        0        0      402 2024-04-02 12:08:01.844558 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_manager.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844690 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844823 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.845006 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-02 12:08:01.845143 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0        0        0     5602 2024-05-24 05:33:08.366607 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0        0        0     5019 2024-05-15 03:58:25.722266 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/flask_server.py
+-rw-r--r--   0        0        0     2351 2024-04-26 15:29:30.265783 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/gunicorn_server.py
+-rw-r--r--   0        0        0     9311 2024-04-26 09:03:49.038432 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/request_task.py
+-rw-r--r--   0        0        0      164 2024-04-26 09:03:49.038779 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-15 03:58:25.722567 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-15 03:58:25.722726 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto
+-rw-r--r--   0        0        0     2092 2024-05-15 03:58:25.722866 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py
+-rw-r--r--   0        0        0     5979 2024-05-15 03:58:25.723032 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5033 2024-05-15 03:58:25.723168 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py
+-rw-r--r--   0        0        0     3307 2024-05-15 03:58:25.723368 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/rpc_server.py
+-rw-r--r--   0        0        0     1146 2024-04-02 12:08:01.845635 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0        0        0      822 2024-04-26 15:29:30.266263 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0        0        0     2679 2024-04-26 15:29:30.266639 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846346 agentuniverse-0.0.6.dev1/agentuniverse/base/__init__.py
+-rw-r--r--   0        0        0    11557 2024-05-15 03:58:25.723582 agentuniverse-0.0.6.dev1/agentuniverse/base/agentuniverse.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846609 agentuniverse-0.0.6.dev1/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-02 12:08:01.846840 agentuniverse-0.0.6.dev1/agentuniverse/base/annotation/singleton.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.847286 agentuniverse-0.0.6.dev1/agentuniverse/base/component/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-26 03:46:54.108902 agentuniverse-0.0.6.dev1/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0        0        0     1264 2024-04-26 03:46:54.107724 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_base.py
+-rw-r--r--   0        0        0     4380 2024-04-26 09:03:49.040235 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0        0        0      626 2024-04-26 09:03:49.040545 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0        0        0     2576 2024-04-26 03:46:54.137220 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_manager_base.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.848825 agentuniverse-0.0.6.dev1/agentuniverse/base/config/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.849235 agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-26 09:03:49.040952 agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0        0        0     1006 2024-04-26 03:46:54.105041 agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/application_config_manager.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850062 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-26 09:03:49.041321 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/component_configer.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850500 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0        0        0     2599 2024-04-26 03:46:54.162861 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0        0        0     2053 2024-04-26 03:46:54.189422 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0        0        0     3272 2024-04-26 03:46:54.100009 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0        0        0     2540 2024-04-26 03:46:54.198928 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0        0        0     2392 2024-04-26 03:46:54.181023 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0        0        0     1889 2024-04-26 09:03:49.041670 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/prompt_configer.py
+-rw-r--r--   0        0        0     2192 2024-04-26 03:46:54.165777 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0        0        0      423 2024-04-02 12:08:01.852070 agentuniverse-0.0.6.dev1/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0        0        0     4846 2024-04-26 15:29:30.267459 agentuniverse-0.0.6.dev1/agentuniverse/base/config/configer.py
+-rw-r--r--   0        0        0      163 2024-04-02 12:08:01.852534 agentuniverse-0.0.6.dev1/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-26 03:55:12.618569 agentuniverse-0.0.6.dev1/agentuniverse/base/config/custom_configer/custom_key_configer.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.852949 agentuniverse-0.0.6.dev1/agentuniverse/base/context/__init__.py
+-rw-r--r--   0        0        0     1447 2024-04-26 03:46:54.182246 agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0        0        0     2768 2024-04-26 03:46:54.110018 agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context_manager.py
+-rw-r--r--   0        0        0      174 2024-04-26 09:03:49.042097 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-26 09:03:49.042363 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/combine_cn_prompt.yaml
+-rw-r--r--   0        0        0      318 2024-04-26 09:03:49.042631 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/combine_en_prompt.yaml
+-rw-r--r--   0        0        0      253 2024-04-26 09:03:49.042893 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/summary_cn_prompt.yaml
+-rw-r--r--   0        0        0      272 2024-04-26 09:03:49.043156 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/summary_en_prompt.yaml
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.853924 agentuniverse-0.0.6.dev1/agentuniverse/base/util/__init__.py
+-rw-r--r--   0        0        0      307 2024-04-02 12:08:01.854131 agentuniverse-0.0.6.dev1/agentuniverse/base/util/env_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.854373 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-26 03:42:29.579851 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0        0        0     5132 2024-04-02 12:08:01.854819 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0        0        0     6395 2024-04-26 03:42:21.826133 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0        0        0      502 2024-04-26 03:42:41.042298 agentuniverse-0.0.6.dev1/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0        0        0     7465 2024-05-21 09:31:45.019227 agentuniverse-0.0.6.dev1/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0        0        0      715 2024-04-02 12:08:01.855496 agentuniverse-0.0.6.dev1/agentuniverse/base/util/system_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.855704 agentuniverse-0.0.6.dev1/agentuniverse/llm/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.855856 agentuniverse-0.0.6.dev1/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-26 09:03:49.043837 agentuniverse-0.0.6.dev1/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0        0        0      223 2024-04-26 09:03:49.044133 agentuniverse-0.0.6.dev1/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0        0        0     5625 2024-05-24 05:33:08.354446 agentuniverse-0.0.6.dev1/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0        0        0     5601 2024-05-16 08:48:01.873337 agentuniverse-0.0.6.dev1/agentuniverse/llm/llm.py
+-rw-r--r--   0        0        0      619 2024-04-26 03:46:54.138842 agentuniverse-0.0.6.dev1/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0        0        0      408 2024-04-26 09:03:49.045322 agentuniverse-0.0.6.dev1/agentuniverse/llm/llm_output.py
+-rw-r--r--   0        0        0     8294 2024-05-24 05:33:08.354632 agentuniverse-0.0.6.dev1/agentuniverse/llm/openai_llm.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.856945 agentuniverse-0.0.6.dev1/agentuniverse/prompt/__init__.py
+-rw-r--r--   0        0        0     3351 2024-05-21 09:31:45.020660 agentuniverse-0.0.6.dev1/agentuniverse/prompt/chat_prompt.py
+-rw-r--r--   0        0        0      548 2024-04-26 07:36:14.033265 agentuniverse-0.0.6.dev1/agentuniverse/prompt/enum.py
+-rw-r--r--   0        0        0     2863 2024-05-21 09:31:45.020823 agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt.py
+-rw-r--r--   0        0        0      741 2024-04-26 09:03:49.046141 agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_manager.py
+-rw-r--r--   0        0        0     1882 2024-05-21 09:31:45.020988 agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_model.py
+-rw-r--r--   0        0        0      164 2024-04-02 03:12:13.477398 agentuniverse-0.0.6.dev1/agentuniverse_connector/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 03:13:12.638584 agentuniverse-0.0.6.dev1/agentuniverse_extension/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.857428 agentuniverse-0.0.6.dev1/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0        0        0     7321 2024-04-02 12:08:01.857588 agentuniverse-0.0.6.dev1/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0        0        0     2586 2024-05-24 05:33:38.652207 agentuniverse-0.0.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 agentuniverse-0.0.6.dev1/PKG-INFO
```

### Comparing `agentuniverse-0.0.6/LICENSE` & `agentuniverse-0.0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/README_PYPI.md` & `agentuniverse-0.0.6.dev1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         """Get embeddings."""
 
     @abstractmethod
     async def async_get_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Asynchronously get embeddings."""
 
     def as_langchain(self) -> LCEmbeddings:
-        """Convert the AgentUniverse(AU) embedding class to the langchain embedding class."""
+        """Convert the agentUniverse(aU) embedding class to the langchain embedding class."""
         pass
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,10 +87,10 @@
 
             # Return the embeddings as a list of lists of floats
             return [embedding.embedding for embedding in data]
         except BadRequestError as e:
             raise ValueError(e.message)
 
     def as_langchain(self) -> OpenAIEmbeddings:
-        """Convert the AgentUniverse(AU) openai embedding class to the langchain openai embedding class."""
+        """Convert the agentUniverse(aU) openai embedding class to the langchain openai embedding class."""
         return OpenAIEmbeddings(openai_api_key=self.openai_api_key,
                                 client=self.client.embeddings, async_client=self.async_client.embeddings)
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ".pdf": PdfReader,
     ".docx": DocxReader,
     ".pptx": PptxReader,
 }
 
 
 class FileReader(Reader):
-    """The AgentUniverse(AU) file reader class.
+    """The agentUniverse(aU) file reader class.
 
     FileReader is used to load data from files based on the provided file paths.
 
     Attributes:
         file_readers (Dict[str, Type[Reader]], optional): The file reader dictionary,
         the key is the suffix of the file, and the value is the specific file reader class.
     """
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import requests
 
 from agentuniverse.agent.action.knowledge.reader.reader import Reader
 from agentuniverse.agent.action.knowledge.store.document import Document
 
 
 class WebPdfReader(Reader):
-    """The AgentUniverse(AU) web pdf reader.
+    """The agentUniverse(aU) web pdf reader.
 
     The pdf file will be downloaded and then parsed by `pdfminer.six`.
     """
 
     def load_data(self, web_pdf_url: str) -> List[Document]:
         if web_pdf_url is None:
             return []
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 query_embeddings=[embedding]
             )
         else:
             query_result = self.collection.query(
                 n_results=query.similarity_top_k,
                 query_texts=[query.query_str]
             )
-        # convert to the AgentUniverse(AU) document format
+        # convert to the agentUniverse(aU) document format
         return self.to_documents(query_result)
 
     def insert_documents(self, documents: List[Document], **kwargs: Any):
         """Insert documents to the chroma collection.
 
         Args:
             documents (List[Document]): The documents to be inserted.
@@ -123,15 +123,15 @@
                 metadatas=[document.metadata],
                 embeddings=[embedding] if embedding is not None else None,
                 ids=[document.id]
             )
 
     @staticmethod
     def to_documents(query_result: QueryResult) -> List[Document]:
-        """Convert the query results of ChromaDB to the AgentUniverse(AU) document format."""
+        """Convert the query results of ChromaDB to the agentUniverse(aU) document format."""
 
         if query_result is None:
             return []
         documents = []
         for i in range(len(query_result['ids'][0])):
             documents.append(Document(id=query_result['ids'][0][i],
                                       text=query_result['documents'][0][i],
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/document.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     def as_langchain(self) -> LCDocument:
         """Convert to LangChain document format."""
         metadata = self.metadata or {}
         return LCDocument(page_content=self.text, metadata=metadata)
 
     @staticmethod
     def as_langchain_list(document_list) -> List[LCDocument]:
-        """Convert AgentUniverse(AU) document list to langchain document list """
+        """Convert agentUniverse(aU) document list to langchain document list """
         langchain_document_list = []
         if document_list is None:
             return langchain_document_list
         for document in document_list:
             langchain_document_list.append(LCDocument(page_content=document.text, metadata=document.metadata))
         return langchain_document_list
 
     @staticmethod
     def from_langchain_list(lc_document_list: List[LCDocument]):
-        """Convert langchain document list to AgentUniverse(AU) document list """
+        """Convert langchain document list to agentUniverse(aU) document list """
         document_list = []
         if lc_document_list is None:
             return document_list
         for lc_document in lc_document_list:
             document_list.append(Document(text=lc_document.page_content, metadata=lc_document.metadata))
         return document_list
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/query.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/store.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 raise Exception(f'{self.get_instance_code()} - The input must include key: {key}.')
 
     @abstractmethod
     def execute(self, tool_input: ToolInput):
         raise NotImplementedError
 
     def as_langchain(self) -> LangchainTool:
-        """Convert the AgentUniverse(AU) tool class to the langchain tool class."""
+        """Convert the agentUniverse(aU) tool class to the langchain tool class."""
         return LangchainTool(name=self.name,
                              func=self.run,
                              description=self.description)
 
     def get_instance_code(self) -> str:
         """Return the full name of the tool."""
         appname = ApplicationConfigManager().app_configer.base_info_appname
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/agent.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 
     @abstractmethod
     def output_keys(self) -> list[str]:
         """Return the output keys of the Agent."""
         pass
 
     @abstractmethod
-    def parse_input(self, input_object: InputObject, planner_input: dict) -> dict:
-        """Planner parameter parsing.
+    def parse_input(self, input_object: InputObject, agent_input: dict) -> dict:
+        """Agent parameter parsing.
 
         Args:
-            input_object(InputObject): agent parameter object
-            planner_input(dict): Planner input
+            input_object (InputObject): input parameters passed by the user.
+            agent_input (dict): agent input preparsed by the agent.
         Returns:
-            dict: Planner parameter.
+            dict: agent input parsed from `input_object` by the user.
         """
         pass
 
     @abstractmethod
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
@@ -70,49 +70,56 @@
         """Agent instance running entry.
 
         Returns:
             OutputObject: Agent execution result
         """
         self.input_check(kwargs)
         input_object = InputObject(kwargs)
-        execute_result = self.execute(input_object)
-        self.output_check(execute_result)
-        output_object = OutputObject(execute_result)
+
+        agent_input = self.pre_parse_input(input_object)
+
+        planner_result = self.execute(input_object, agent_input)
+
+        agent_result = self.parse_result(planner_result)
+
+        self.output_check(agent_result)
+        output_object = OutputObject(agent_result)
         return output_object
 
-    def execute(self, input_object: InputObject) -> dict:
+    def execute(self, input_object: InputObject, agent_input: dict) -> dict:
         """Execute agent instance.
 
         Args:
-            input_object(InputObject): agent parameter object
+            input_object (InputObject): input parameters passed by the user.
+            agent_input (dict): agent input parsed from `input_object` by the user.
+
         Returns:
-            dict: Agent result object.
+            dict: planner result generated by the planner execution.
         """
-        planner_input = self.pre_parse_input(input_object)
 
         planner_base: Planner = PlannerManager().get_instance_obj(self.agent_model.plan.get('planner').get('name'))
-        planner_result = planner_base.invoke(self.agent_model, planner_input, input_object)
-
-        parser_result = self.parse_result(planner_result)
-        return parser_result
+        planner_result = planner_base.invoke(self.agent_model, agent_input, input_object)
+        return planner_result
 
     def pre_parse_input(self, input_object) -> dict:
         """Agent execution parameter pre-parsing.
 
-        Args: input_object(InputObject): agent parameter object
+        Args:
+            input_object (InputObject): input parameters passed by the user.
         Returns:
-            dict: Planner input
+            dict: agent input preparsed by the agent.
         """
-        planner_input = dict()
-        planner_input['chat_history'] = input_object.get_data('chat_history') or ''
-        planner_input['background'] = input_object.get_data('background') or ''
-        planner_input['date'] = datetime.now().strftime('%Y-%m-%d')
+        agent_input = dict()
+        agent_input['chat_history'] = input_object.get_data('chat_history') or ''
+        agent_input['background'] = input_object.get_data('background') or ''
+        agent_input['image_urls'] = input_object.get_data('image_urls') or []
+        agent_input['date'] = datetime.now().strftime('%Y-%m-%d')
 
-        self.parse_input(input_object, planner_input)
-        return planner_input
+        self.parse_input(input_object, agent_input)
+        return agent_input
 
     def get_instance_code(self) -> str:
         """Return the full name of the agent."""
         appname = ApplicationConfigManager().app_configer.base_info_appname
         name = self.agent_model.info.get('name')
         return (f'{appname}.'
                 f'{self.component_type.value.lower()}.{name}')
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/agent_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/agent_model.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/executing_agent.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/planning_agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,50 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/19 18:18
+# @Time    : 2024/3/15 11:40
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: executing_agent.py
-"""Executing Agent module."""
-import copy
-from concurrent.futures import ThreadPoolExecutor, wait, ALL_COMPLETED
-from typing import Optional, Any
+# @FileName: planning_agent.py
+"""Planning agent module."""
+import json
 from agentuniverse.agent.agent import Agent
 from agentuniverse.agent.input_object import InputObject
-from agentuniverse.agent.plan.planner.planner_manager import PlannerManager
 
 
-class ExecutingAgent(Agent):
-    """Executing Agent class."""
-
-    executor: Optional[Any] = ThreadPoolExecutor(max_workers=10, thread_name_prefix="executing_agent")
+class PlanningAgent(Agent):
+    """Planning Agent class."""
 
     def input_keys(self) -> list[str]:
         """Return the input keys of the Agent."""
-        return ['planning_result']
+        return ['input']
 
     def output_keys(self) -> list[str]:
         """Return the output keys of the Agent."""
-        return ['executing_result']
+        return ['output']
 
-    def parse_input(self, input_object: InputObject, planner_input: dict) -> dict:
-        """Planner parameter parsing.
+    def parse_input(self, input_object: InputObject, agent_input: dict) -> dict:
+        """Agent parameter parsing.
 
         Args:
-            input_object(InputObject): agent parameter object
-            planner_input(dict): Planner input
+            input_object (InputObject): input parameters passed by the user.
+            agent_input (dict): agent input preparsed by the agent.
         Returns:
-            dict: Planner input
+            dict: agent input parsed from `input_object` by the user.
         """
-        planner_input['input'] = input_object.get_data('input')
-        planner_input['framework'] = input_object.get_data('planning_result').get_data('framework')
-        self.agent_model.profile.setdefault('prompt_version', 'default_executing_agent.cn')
-        return planner_input
+        agent_input['input'] = input_object.get_data('input')
+        agent_input['expert_framework'] = input_object.get_data('expert_framework')
+        self.agent_model.profile.setdefault('prompt_version', 'default_planning_agent.cn')
+        return agent_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
         Returns:
             dict: Agent result object.
         """
-        llm_result = []
-        executing_result = []
-        futures = planner_result.get('futures')
-        for future in futures:
-            task_result = future.result()
-            llm_result.append(task_result)
-            executing_result.append({
-                'input': task_result['input'], 'output': task_result['output']
-            })
-
-        return {'executing_result': executing_result, 'llm_result': llm_result}
-
-    def execute(self, input_object: InputObject) -> dict:
-        """Execute agent instance.
-
-        Args:
-            input_object(InputObject): agent parameter object
-        Returns:
-            dict: Agent result object.
-        """
-        planning_result = input_object.get_data('planning_result')
-        framework = planning_result.get_data('framework', [])
-        futures = []
-        for task in framework:
-            input_object_copy: InputObject = copy.deepcopy(input_object)
-            input_object_copy.add_data('input', task)
-            planner_input = super().pre_parse_input(input_object_copy)
-            futures.append(
-                self.executor.submit(
-                    PlannerManager().get_instance_obj(self.agent_model.plan.get('planner').get('name')).invoke,
-                    self.agent_model, planner_input, input_object_copy))
-        wait(futures, return_when=ALL_COMPLETED)
-        return self.parse_result({'futures': futures})
+        output = planner_result.get('output')
+        output = json.loads(output)
+        planner_result['framework'] = output['framework']
+        planner_result['thought'] = output['thought']
+        return planner_result
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/expressing_agent.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/expressing_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
         """Return the input keys of the Agent."""
         return ['input']
 
     def output_keys(self) -> list[str]:
         """Return the output keys of the Agent."""
         return ['output']
 
-    def parse_input(self, input_object: InputObject, planner_input: dict) -> dict:
-        """Planner parameter parsing.
+    def parse_input(self, input_object: InputObject, agent_input: dict) -> dict:
+        """Agent parameter parsing.
 
         Args:
-            input_object(InputObject): agent parameter object
-            planner_input(dict): Planner input
+            input_object (InputObject): input parameters passed by the user.
+            agent_input (dict): agent input preparsed by the agent.
         Returns:
-            dict: Planner input
+            dict: agent input parsed from `input_object` by the user.
         """
-        planner_input['input'] = input_object.get_data('input')
-        planner_input['background'] = self.build_background(input_object)
+        agent_input['input'] = input_object.get_data('input')
+        agent_input['background'] = self.build_background(input_object)
         self.agent_model.profile.setdefault('prompt_version', 'default_expressing_agent.cn')
-        return planner_input
+        return agent_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
         Returns:
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/peer_agent.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/peer_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,25 +16,25 @@
         """Return the input keys of the Agent."""
         return ['input']
 
     def output_keys(self) -> list[str]:
         """Return the output keys of the Agent."""
         return ['output']
 
-    def parse_input(self, input_object: InputObject, planner_input: dict) -> dict:
-        """Planner parameter parsing.
+    def parse_input(self, input_object: InputObject, agent_input: dict) -> dict:
+        """Agent parameter parsing.
 
         Args:
-            input_object(InputObject): agent parameter object
-            planner_input(dict): Planner input
+            input_object(InputObject): input parameters passed by the user.
+            agent_input(dict): agent input preparsed by the agent.
         Returns:
-            dict: Planner input
+            dict: agent input parsed from `input_object` by the user.
         """
-        planner_input['input'] = input_object.get_data('input')
-        return planner_input
+        agent_input['input'] = input_object.get_data('input')
+        return agent_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
         Returns:
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/planning_agent.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/rag_agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/15 11:40
+# @Time    : 2024/3/25 15:03
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: planning_agent.py
+# @FileName: rag_agent.py
 """Planning agent module."""
-import json
 from agentuniverse.agent.agent import Agent
 from agentuniverse.agent.input_object import InputObject
 
 
-class PlanningAgent(Agent):
-    """Planning Agent class."""
+class RagAgent(Agent):
+    """Rag Agent class."""
 
     def input_keys(self) -> list[str]:
         """Return the input keys of the Agent."""
         return ['input']
 
     def output_keys(self) -> list[str]:
         """Return the output keys of the Agent."""
         return ['output']
 
-    def parse_input(self, input_object: InputObject, planner_input: dict) -> dict:
-        """Planner parameter parsing.
+    def parse_input(self, input_object: InputObject, agent_input: dict) -> dict:
+        """Agent parameter parsing.
 
         Args:
-            input_object(InputObject): agent parameter object
-            planner_input(dict): Planner input
+            input_object (InputObject): input parameters passed by the user.
+            agent_input (dict): agent input preparsed by the agent.
         Returns:
-            dict: Planner input
+            dict: agent input parsed from `input_object` by the user.
         """
-        planner_input['input'] = input_object.get_data('input')
-        planner_input['expert_framework'] = input_object.get_data('expert_framework')
-        self.agent_model.profile.setdefault('prompt_version', 'default_planning_agent.cn')
-        return planner_input
+        agent_input['input'] = input_object.get_data('input')
+        self.agent_model.profile.setdefault('prompt_version', 'default_rag_agent.cn')
+        return agent_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
         Returns:
             dict: Agent result object.
         """
-        output = planner_result.get('output')
-        output = json.loads(output)
-        planner_result['framework'] = output['framework']
-        planner_result['thought'] = output['thought']
         return planner_result
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,27 @@
         """Return the input keys of the Agent."""
         return ['input', 'expressing_result']
 
     def output_keys(self) -> list[str]:
         """Return the output keys of the Agent."""
         return ['output']
 
-    def parse_input(self, input_object: InputObject, planner_input: dict) -> dict:
-        """Planner parameter parsing.
+    def parse_input(self, input_object: InputObject, agent_input: dict) -> dict:
+        """Agent parameter parsing.
 
         Args:
-            input_object(InputObject): agent parameter object
-            planner_input(dict): Planner input
+            input_object(InputObject): input parameters passed by the user.
+            agent_input(dict): agent input preparsed by the agent.
         Returns:
-            dict: Planner parameter.
+            dict: agent input parsed from `input_object` by the user.
         """
-        planner_input['input'] = input_object.get_data('input')
-        planner_input['expressing_result'] = input_object.get_data('expressing_result').get_data('output')
+        agent_input['input'] = input_object.get_data('input')
+        agent_input['expressing_result'] = input_object.get_data('expressing_result').get_data('output')
         self.agent_model.profile.setdefault('prompt_version', 'default_reviewing_agent.cn')
-        return planner_input
+        return agent_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
         Returns:
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/input_object.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/chat_memory.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/chat_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     llm: Optional[LLM] = None
     input_key: Optional[str] = None
     output_key: Optional[str] = None
     messages: Optional[List[Message]] = None
     prompt_version: Optional[str] = None
 
     def as_langchain(self) -> BaseChatMemory:
-        """Convert the AgentUniverse(AU) chat memory class to the langchain chat memory class."""
+        """Convert the agentUniverse(aU) chat memory class to the langchain chat memory class."""
         if self.llm is None:
             raise ValueError("Must set `llm` when using langchain memory.")
         if self.type is None or self.type == MemoryTypeEnum.SHORT_TERM:
             return AuConversationTokenBufferMemory(llm=self.llm.as_langchain(), memory_key=self.memory_key,
                                                    input_key=self.input_key, output_key=self.output_key,
                                                    max_token_limit=self.max_tokens, messages=self.messages)
         elif self.type == MemoryTypeEnum.LONG_TERM:
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/default/default_memory.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/default_memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/langchain_instance.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/memory.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     memory_key: Optional[str] = 'chat_history'
     max_tokens: int = 2000
 
     def __init__(self, **kwargs):
         super().__init__(component_type=ComponentEnum.MEMORY, **kwargs)
 
     def as_langchain(self) -> BaseMemory:
-        """Convert the AgentUniverse(AU) memory class to the langchain memory class."""
+        """Convert the agentUniverse(aU) memory class to the langchain memory class."""
         pass
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the Memory model in the agent configuration."""
         if 'memory_key' in kwargs and kwargs['memory_key']:
             self.memory_key = kwargs['memory_key']
         if 'max_tokens' in kwargs and kwargs['max_tokens']:
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/memory_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_cn_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_en_prompt.yaml` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/output_object.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:42
+# @Time    : 2024/3/14 16:02
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: executing_planner.py
-"""Execution planner module."""
+# @FileName: planning_planner.py
+"""Planning planner module."""
 import asyncio
 
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
@@ -16,41 +16,40 @@
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class ExecutingPlanner(Planner):
-    """Executing planner class."""
+class PlanningPlanner(Planner):
+    """Planning planner class."""
 
-    def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
+    def invoke(self, agent_model: AgentModel, planner_input: dict,
+               input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
-
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
-        self.handle_all_actions(agent_model, planner_input, input_object)
-
         llm: LLM = self.handle_llm(agent_model)
 
         prompt: Prompt = self.handle_prompt(agent_model, planner_input)
         process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
                              prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
-        return asyncio.run(llm_chain.acall(inputs=planner_input))
+
+        return asyncio.run(llm_chain.acall(planner_input))
 
     def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
         llm: LLM = self.handle_llm(agent_model)
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
         planner_config = agent_model.plan.get('planner')
         sub_agents = self.generate_sub_agents(planner_config)
         return self.agents_run(sub_agents, planner_config, planner_input, input_object)
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def invoke(self, agent_model: AgentModel, planner_input: dict,
                input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
         pass
 
     def handle_memory(self, agent_model: AgentModel, planner_input: dict) -> BaseMemory | None:
         """Memory module processing.
@@ -120,15 +120,15 @@
             knowledge_res: List[Document] = knowledge.store.query(
                 Query(query_str=input_object.get_data(self.input_key), similarity_top_k=2), **input_object.to_dict())
             for document in knowledge_res:
                 action_result.append(document.text)
 
         planner_input['background'] = planner_input['background'] or '' + "\n".join(action_result)
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
         Returns:
             Prompt: The prompt instance.
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/14 16:02
+# @Time    : 2024/3/18 10:42
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: planning_planner.py
-"""Planning planner module."""
+# @FileName: executing_planner.py
+"""Execution planner module."""
 import asyncio
 
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
@@ -16,40 +16,41 @@
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class PlanningPlanner(Planner):
-    """Planning planner class."""
+class ExecutingPlanner(Planner):
+    """Executing planner class."""
 
-    def invoke(self, agent_model: AgentModel, planner_input: dict,
-               input_object: InputObject) -> dict:
+    def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
+
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
+        self.handle_all_actions(agent_model, planner_input, input_object)
+
         llm: LLM = self.handle_llm(agent_model)
 
         prompt: Prompt = self.handle_prompt(agent_model, planner_input)
         process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
                              prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
-
-        return asyncio.run(llm_chain.acall(planner_input))
+        return asyncio.run(llm_chain.acall(inputs=planner_input))
 
     def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from langchain_core.memory import BaseMemory
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
+from agentuniverse.prompt.chat_prompt import ChatPrompt
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
 class RagPlanner(Planner):
     """Rag planner class."""
@@ -26,40 +27,41 @@
     def invoke(self, agent_model: AgentModel, planner_input: dict,
                input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
         self.handle_all_actions(agent_model, planner_input, input_object)
 
         llm: LLM = self.handle_llm(agent_model)
 
-        prompt: Prompt = self.handle_prompt(agent_model, planner_input)
+        prompt: ChatPrompt = self.handle_prompt(agent_model, planner_input)
         process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
                              prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
+
         return asyncio.run(llm_chain.acall(inputs=planner_input))
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> ChatPrompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
         Returns:
-            Prompt: The prompt instance.
+            ChatPrompt: The chat prompt instance.
         """
         profile: dict = agent_model.profile
 
         profile_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
                                                                   target=profile.get('target'),
                                                                   instruction=profile.get('instruction'))
 
@@ -73,8 +75,12 @@
         if version_prompt:
             version_prompt_model: AgentPromptModel = AgentPromptModel(
                 introduction=getattr(version_prompt, 'introduction', ''),
                 target=getattr(version_prompt, 'target', ''),
                 instruction=getattr(version_prompt, 'instruction', ''))
             profile_prompt_model = profile_prompt_model + version_prompt_model
 
-        return Prompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
+        chat_prompt = ChatPrompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
+        image_urls: list = planner_input.pop('image_urls', []) or []
+        if image_urls:
+            chat_prompt.generate_image_prompt(image_urls)
+        return chat_prompt
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
-            input_object (InputObject): Agent input object.
+            input_object (InputObject): The input parameters passed by the user.
         Returns:
             dict: The planner result.
         """
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
         llm: LLM = self.handle_llm(agent_model)
 
@@ -47,15 +47,15 @@
         return asyncio.run(llm_chain.acall(inputs=planner_input))
 
     def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Generate prompt template for the planner.
 
         Args:
             agent_model (AgentModel): The agent model.
-            planner_input (dict): The agent input.
+            planner_input (dict): The planner input.
         Returns:
             Prompt: The prompt instance.
         """
         expert_framework = planner_input.pop('expert_framework', '') or ''
 
         profile: dict = agent_model.profile
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/service.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/service_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/service_instance.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/request_library.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,21 +41,23 @@
 
 
 @singleton
 class RequestLibrary:
     def __init__(self, configer: Configer = None):
         """Init the database connection. Use uri in config file or use sqlite
         as default database."""
-        mysql_uri = None
+        system_db_uri = None
         if Configer:
-            mysql_uri = configer.get('DB', {}).get('mysql_uri')
-        if mysql_uri and mysql_uri.strip():
-            db_uri = mysql_uri
+            system_db_uri = configer.get('DB', {}).get('system_db_uri')
+            if not system_db_uri:
+                system_db_uri = configer.get('DB', {}).get('mysql_uri')
+        if system_db_uri and system_db_uri.strip():
+            db_uri = system_db_uri
         else:
-            db_path = get_project_root_path() / 'DB' / 'agent_framework.db'
+            db_path = get_project_root_path() / 'DB' / 'agent_universe.db'
             db_path.parent.mkdir(parents=True, exist_ok=True)
             db_uri = f'sqlite:////{db_path}'
 
         self.db_uri = db_uri
         self.Session = None
 
     def query_request_by_request_id(self, request_id: str) -> RequestDO | None:
```

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/flask_server.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/flask_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/gunicorn_server.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/gunicorn_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/request_task.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/request_task.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/rpc_server.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/thread_with_result.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_booster.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_util.py` & `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/agentuniverse.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/agentuniverse.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/annotation/singleton.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/component/application_component_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/component/component_base.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/component/component_configer_util.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_configer_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/component/component_enum.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/component/component_manager_base.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/application_configer/app_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/component_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/component_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/prompt_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/prompt_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/tool_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/context/framework_context.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/context/framework_context_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/util/logging/general_logger.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_config.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_util.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/base/util/prompt_util.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/util/prompt_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 # @Time    : 2024/4/16 14:42
 # @Author  : wangchongshi
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: prompt_util.py
-import asyncio
 from typing import List
 
 from langchain.chains.summarize import load_summarize_chain
 from langchain_core.documents import Document
-from langchain_core.prompts import PromptTemplate
 
+from agentuniverse.agent.memory.message import Message
 from agentuniverse.llm.llm import LLM
 from agentuniverse.llm.llm_manager import LLMManager
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 from agentuniverse.prompt.enum import PromptProcessEnum
 
 
@@ -102,43 +101,61 @@
         value = getattr(agent_prompt_model, attr, None)
         if value is not None:
             values.append(value)
 
     return "\n".join(values)
 
 
-def process_llm_token(agent_llm: LLM, prompt_template: PromptTemplate, profile: dict, planner_input: dict):
+def generate_chat_template(agent_prompt_model: AgentPromptModel, prompt_assemble_order: list[str]) -> list[Message]:
+    """Convert the agent prompt model to the agentUniverse message list.
+
+    Args:
+        agent_prompt_model (AgentPromptModel): The agent prompt model.
+        prompt_assemble_order (list[str]): The prompt assemble ordered list.
+    Returns:
+        list: The agentUniverse message list.
+    """
+    message_list = []
+    for attr in prompt_assemble_order:
+        value = getattr(agent_prompt_model, attr, None)
+        if value is not None:
+            message_list.append(
+                Message(type=agent_prompt_model.get_message_type(attr), content=value))
+    return message_list
+
+
+def process_llm_token(agent_llm: LLM, lc_prompt_template, profile: dict, planner_input: dict):
     """Process the prompt template based on the prompt processor.
 
     Args:
         agent_llm (LLM): The agent llm.
-        prompt_template (PromptTemplate): The prompt template.
+        lc_prompt_template: The langchain prompt template.
         profile (dict): The profile.
         planner_input (dict): The planner input.
     """
     llm_model: dict = profile.get('llm_model')
 
     # get the prompt processor configuration
     prompt_processor: dict = llm_model.get('prompt_processor') or dict()
     prompt_processor_type: str = prompt_processor.get('type') or PromptProcessEnum.TRUNCATE.value
     prompt_processor_llm: str = prompt_processor.get('llm')
 
     # get the summary and combine prompt versions
     summary_prompt_version: str = prompt_processor.get('summary_prompt_version') or 'prompt_processor.summary_cn'
     combine_prompt_version: str = prompt_processor.get('combine_prompt_version') or 'prompt_processor.combine_cn'
 
-    prompt_input_dict = {key: planner_input[key] for key in prompt_template.input_variables if key in planner_input}
+    prompt_input_dict = {key: planner_input[key] for key in lc_prompt_template.input_variables if key in planner_input}
 
     # get the llm instance for prompt compression
     prompt_llm: LLM = LLMManager().get_instance_obj(prompt_processor_llm)
 
     if prompt_llm is None:
         prompt_llm = agent_llm
 
-    prompt = prompt_template.format(**prompt_input_dict)
+    prompt = lc_prompt_template.format(**prompt_input_dict)
     # get the number of tokens in the prompt
     prompt_tokens: int = agent_llm.get_num_tokens(prompt)
 
     input_tokens = agent_llm.max_context_length() - agent_llm.max_tokens
 
     if prompt_tokens <= input_tokens:
         return
```

### Comparing `agentuniverse-0.0.6/agentuniverse/base/util/system_util.py` & `agentuniverse-0.0.6.dev1/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/llm/default/default_openai_llm.py` & `agentuniverse-0.0.6.dev1/agentuniverse/llm/default/default_openai_llm.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/llm/langchain_instance.py` & `agentuniverse-0.0.6.dev1/agentuniverse/llm/langchain_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
     llm: Optional[LLM] = None
 
     def __init__(self, llm: LLM):
         """The __init__ method.
 
         The agentUniverse LLM instance is passed to this class as an argument.
-        Convert the attributes of AgentUniverse(AU) LLM instance to the LangchainOpenAI object for initialization
+        Convert the attributes of agentUniverse(aU) LLM instance to the LangchainOpenAI object for initialization
 
         Args:
-            llm (LLM): the AgentUniverse(AU) LLM instance.
+            llm (LLM): the agentUniverse(aU) LLM instance.
         """
         init_params = dict()
         init_params['model_name'] = llm.model_name if llm.model_name else 'gpt-3.5-turbo'
         init_params['temperature'] = llm.temperature if llm.temperature else 0.7
         init_params['request_timeout'] = llm.request_timeout
         init_params['max_tokens'] = llm.max_tokens
         init_params['max_retries'] = llm.max_retries if llm.max_retries else 2
```

### Comparing `agentuniverse-0.0.6/agentuniverse/llm/llm.py` & `agentuniverse-0.0.6.dev1/agentuniverse/llm/llm.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/llm/llm_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/llm/openai_llm.py` & `agentuniverse-0.0.6.dev1/agentuniverse/llm/openai_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             )
             if not streaming:
                 text = chat_completion.choices[0].message.content
                 return LLMOutput(text=text, raw=chat_completion.model_dump())
             return self.agenerate_stream_result(chat_completion)
 
     def as_langchain(self) -> BaseLanguageModel:
-        """Convert the AgentUniverse(AU) openai llm class to the langchain openai llm class."""
+        """Convert the agentUniverse(aU) openai llm class to the langchain openai llm class."""
         return LangchainOpenAI(self)
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the OpenAILLM model in the agent configuration."""
         super().set_by_agent_model(**kwargs)
         if 'openai_api_key' in kwargs and kwargs['openai_api_key']:
             self.openai_api_key = kwargs['openai_api_key']
```

### Comparing `agentuniverse-0.0.6/agentuniverse/prompt/enum.py` & `agentuniverse-0.0.6.dev1/agentuniverse/prompt/enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse/prompt/prompt.py` & `agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     prompt_version: Optional[str] = None
     prompt_template: Optional[str] = None
     input_variables: Optional[list[str]] = None
 
     def __init__(self, **kwargs):
         super().__init__(component_type=ComponentEnum.PROMPT, **kwargs)
 
-    def as_langchain(self) -> PromptTemplate:
+    def as_langchain(self):
         """Convert the prompt template into a LangChain prompt template.
 
         Returns:
             PromptTemplate: The prompt template.
         """
         return PromptTemplate(template=self.prompt_template,
                               input_variables=self.input_variables)
@@ -40,15 +40,15 @@
         """Build the prompt class.
 
         Args:
             agent_prompt_model (AgentPromptModel): The user agent prompt model.
             prompt_assemble_order (list[str]): The prompt assemble ordered list.
 
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt object.
         """
         self.prompt_template = generate_template(agent_prompt_model, prompt_assemble_order)
         self.input_variables = re.findall(r'\{(.*?)}', self.prompt_template)
         return self
 
     def get_instance_code(self) -> str:
         """Return the prompt version of the current prompt."""
```

### Comparing `agentuniverse-0.0.6/agentuniverse/prompt/prompt_manager.py` & `agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/agentuniverse_extension/logger/sls_sink.py` & `agentuniverse-0.0.6.dev1/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6/pyproject.toml` & `agentuniverse-0.0.6.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentUniverse"
-version = "0.0.6"
+version = "0.0.6.dev1"
 description = "agentUniverse is a framework for developing applications powered by multi-agent base on large language model."
 
 authors = ["AntGroup <jerry.zzw@antgroup.com>"]
 repository = "https://github.com/alipay/agentUniverse"
 readme = "README_PYPI.md"
 
 packages = [
```

### Comparing `agentuniverse-0.0.6/PKG-INFO` & `agentuniverse-0.0.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.6
+Version: 0.0.6.dev1
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
 Home-page: https://github.com/alipay/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

