# Comparing `tmp/swarms-5.0.5.tar.gz` & `tmp/swarms-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-5.0.5.tar", max compression
+gzip compressed data, was "swarms-5.0.7.tar", max compression
```

## Comparing `swarms-5.0.5.tar` & `swarms-5.0.7.tar`

### file list

```diff
@@ -1,207 +1,209 @@
--rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.0.5/LICENSE
--rw-r--r--   0        0        0    33713 2024-05-21 21:17:55.232096 swarms-5.0.5/README.md
--rw-r--r--   0        0        0     1790 2024-05-21 05:06:14.076867 swarms-5.0.5/pyproject.toml
--rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.0.5/swarms/__init__.py
--rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.0.5/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.0.5/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.0.5/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.0.5/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.0.5/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.0.5/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.0.5/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.0.5/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.0.5/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.0.5/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.0.5/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.0.5/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.0.5/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.0.5/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.0.5/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.0.5/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.0.5/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.0.5/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.0.5/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.0.5/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.0.5/swarms/models/__init__.py
--rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.0.5/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.0.5/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.0.5/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.0.5/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.0.5/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.0.5/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.0.5/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.0.5/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.0.5/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.0.5/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.0.5/swarms/models/gemini.py
--rw-r--r--   0        0        0    14236 2024-05-20 23:12:19.586973 swarms-5.0.5/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.0.5/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.0.5/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.0.5/swarms/models/idefics.py
--rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.0.5/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.0.5/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.0.5/swarms/models/llama3_hosted.py
--rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.0.5/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.0.5/swarms/models/llava.py
--rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.0.5/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.0.5/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.0.5/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.0.5/swarms/models/open_router.py
--rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.0.5/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.0.5/swarms/models/openai_tts.py
--rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.0.5/swarms/models/palm.py
--rw-r--r--   0        0        0     2160 2024-05-20 23:12:19.588204 swarms-5.0.5/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.0.5/swarms/models/qwen.py
--rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.0.5/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.0.5/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.0.5/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.0.5/swarms/models/together.py
--rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.0.5/swarms/models/types.py
--rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.0.5/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.0.5/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.0.5/swarms/models/zeroscope.py
--rw-r--r--   0        0        0        0 2024-05-20 23:12:19.588836 swarms-5.0.5/swarms/prebuilt_swarms/__init__.py
--rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.0.5/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.0.5/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.0.5/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.0.5/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.0.5/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.0.5/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.0.5/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.0.5/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.0.5/swarms/prompts/aot_prompt.py
--rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.0.5/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.0.5/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.0.5/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.0.5/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.0.5/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.0.5/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.0.5/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7152 2024-05-20 23:12:19.589946 swarms-5.0.5/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.0.5/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.0.5/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.0.5/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.0.5/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.0.5/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.0.5/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.0.5/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.0.5/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.0.5/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.0.5/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.0.5/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.0.5/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.0.5/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.0.5/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.0.5/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.0.5/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.0.5/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.0.5/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.0.5/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.0.5/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.0.5/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.0.5/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.0.5/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.0.5/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.0.5/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.0.5/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.0.5/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.0.5/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-05-20 23:12:19.591952 swarms-5.0.5/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.0.5/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.0.5/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.0.5/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.0.5/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.0.5/swarms/schemas/__init__.py
--rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.0.5/swarms/schemas/plan.py
--rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.0.5/swarms/schemas/schemas.py
--rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.0.5/swarms/schemas/step.py
--rw-r--r--   0        0        0     4005 2024-05-21 05:06:15.133196 swarms-5.0.5/swarms/structs/__init__.py
--rw-r--r--   0        0        0    60111 2024-05-21 05:06:23.482699 swarms-5.0.5/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.0.5/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.0.5/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.0.5/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     6624 2024-05-20 23:12:19.592755 swarms-5.0.5/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.0.5/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.0.5/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.0.5/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.0.5/swarms/structs/company.py
--rw-r--r--   0        0        0     4738 2024-05-21 03:30:50.037223 swarms-5.0.5/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.0.5/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.0.5/swarms/structs/debate.py
--rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.0.5/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     3684 2024-05-21 05:06:56.355513 swarms-5.0.5/swarms/structs/hiearchical_swarm.py
--rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.0.5/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.0.5/swarms/structs/message.py
--rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.0.5/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.0.5/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     8390 2024-05-20 23:12:19.594122 swarms-5.0.5/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.0.5/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.0.5/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.0.5/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.0.5/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.0.5/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.0.5/swarms/structs/round_robin.py
--rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.0.5/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.0.5/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.0.5/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.0.5/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.0.5/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.0.5/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.595145 swarms-5.0.5/swarms/structs/utils.py
--rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.0.5/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.0.5/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.0.5/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.0.5/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.0.5/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.0.5/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.0.5/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.0.5/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.0.5/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1680 2024-05-20 23:12:19.595775 swarms-5.0.5/swarms/tools/__init__.py
--rw-r--r--   0        0        0    12610 2024-05-21 21:17:55.233502 swarms-5.0.5/swarms/tools/base_tool.py
--rw-r--r--   0        0        0     6653 2024-05-20 23:12:19.595923 swarms-5.0.5/swarms/tools/code_interpreter.py
--rw-r--r--   0        0        0     5367 2024-05-20 23:12:19.595980 swarms-5.0.5/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0      773 2024-05-20 23:12:19.596031 swarms-5.0.5/swarms/tools/function_util.py
--rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.0.5/swarms/tools/json_former.py
--rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.0.5/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.0.5/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.0.5/swarms/tools/math_eval.py
--rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.0.5/swarms/tools/openai_func_calling_schema.py
--rw-r--r--   0        0        0    13875 2024-05-20 23:12:19.596409 swarms-5.0.5/swarms/tools/openai_tool_creator_decorator.py
--rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.0.5/swarms/tools/py_func_to_openai_func_str.py
--rw-r--r--   0        0        0     4275 2024-05-20 23:12:19.596541 swarms-5.0.5/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0      157 2024-05-20 23:12:19.596586 swarms-5.0.5/swarms/tools/tool.py
--rw-r--r--   0        0        0     6170 2024-05-20 23:12:19.596668 swarms-5.0.5/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.0.5/swarms/utils/README.md
--rw-r--r--   0        0        0     1956 2024-05-20 23:12:19.596815 swarms-5.0.5/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.0.5/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.0.5/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.0.5/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.0.5/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.0.5/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.0.5/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.0.5/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.0.5/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.0.5/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.0.5/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.0.5/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.0.5/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.0.5/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.0.5/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.0.5/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.0.5/swarms/utils/get_total_gpus.py
--rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.0.5/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.0.5/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.0.5/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.0.5/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.0.5/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.0.5/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.0.5/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.0.5/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.0.5/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.0.5/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.0.5/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.0.5/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.0.5/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.0.5/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    35219 1970-01-01 00:00:00.000000 swarms-5.0.5/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.0.7/LICENSE
+-rw-r--r--   0        0        0    33713 2024-05-21 21:17:55.232096 swarms-5.0.7/README.md
+-rw-r--r--   0        0        0     1790 2024-05-24 17:37:48.017729 swarms-5.0.7/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.0.7/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.0.7/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.0.7/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.0.7/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.0.7/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.0.7/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.0.7/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.0.7/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.0.7/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.0.7/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.0.7/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.0.7/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.0.7/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.0.7/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.0.7/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.0.7/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.0.7/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.0.7/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.0.7/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.0.7/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.0.7/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.0.7/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.0.7/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.0.7/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.0.7/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.0.7/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.0.7/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.0.7/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.0.7/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.0.7/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.0.7/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.0.7/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.0.7/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14236 2024-05-20 23:12:19.586973 swarms-5.0.7/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.0.7/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.0.7/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.0.7/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.0.7/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.0.7/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.0.7/swarms/models/llama3_hosted.py
+-rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.0.7/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.0.7/swarms/models/llava.py
+-rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.0.7/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.0.7/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.0.7/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.0.7/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.0.7/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.0.7/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.0.7/swarms/models/palm.py
+-rw-r--r--   0        0        0     2160 2024-05-20 23:12:19.588204 swarms-5.0.7/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.0.7/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.0.7/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.0.7/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.0.7/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.0.7/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.0.7/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.0.7/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.0.7/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.0.7/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.588836 swarms-5.0.7/swarms/prebuilt_swarms/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.0.7/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.0.7/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.0.7/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.0.7/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.0.7/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.0.7/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.0.7/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.0.7/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.0.7/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.0.7/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.0.7/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.0.7/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.0.7/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.0.7/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.0.7/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.0.7/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7157 2024-05-23 01:40:32.871666 swarms-5.0.7/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.0.7/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.0.7/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.0.7/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.0.7/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.0.7/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.0.7/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.0.7/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.0.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.0.7/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.0.7/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.0.7/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.0.7/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.0.7/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.0.7/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.0.7/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.0.7/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.0.7/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.0.7/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.0.7/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.0.7/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.0.7/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.0.7/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.0.7/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.0.7/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.0.7/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.0.7/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.0.7/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.0.7/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     6577 2024-05-24 17:25:52.060992 swarms-5.0.7/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.0.7/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.0.7/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.0.7/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.0.7/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.0.7/swarms/schemas/__init__.py
+-rw-r--r--   0        0        0     3168 2024-05-24 00:43:53.750806 swarms-5.0.7/swarms/schemas/hass_agent_schema.py
+-rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.0.7/swarms/schemas/plan.py
+-rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.0.7/swarms/schemas/schemas.py
+-rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.0.7/swarms/schemas/step.py
+-rw-r--r--   0        0        0     4084 2024-05-24 14:40:28.251160 swarms-5.0.7/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    61796 2024-05-24 17:32:12.443311 swarms-5.0.7/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.0.7/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.0.7/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.0.7/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     6624 2024-05-20 23:12:19.592755 swarms-5.0.7/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.0.7/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.0.7/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.0.7/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.0.7/swarms/structs/company.py
+-rw-r--r--   0        0        0     4738 2024-05-21 03:30:50.037223 swarms-5.0.7/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.0.7/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.0.7/swarms/structs/debate.py
+-rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.0.7/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     8747 2024-05-24 15:44:24.762519 swarms-5.0.7/swarms/structs/hiearchical_swarm.py
+-rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.0.7/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.0.7/swarms/structs/message.py
+-rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.0.7/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.0.7/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     8193 2024-05-24 00:28:06.786449 swarms-5.0.7/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.0.7/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.0.7/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.0.7/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.0.7/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.0.7/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.0.7/swarms/structs/round_robin.py
+-rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.0.7/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.0.7/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0     1396 2024-05-23 01:40:40.668233 swarms-5.0.7/swarms/structs/society_of_agents.py
+-rw-r--r--   0        0        0    11249 2024-05-24 16:15:05.490950 swarms-5.0.7/swarms/structs/swarm_load_balancer.py
+-rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.0.7/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.0.7/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.0.7/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.0.7/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3646 2024-05-23 01:40:40.674259 swarms-5.0.7/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.0.7/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.0.7/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.0.7/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.0.7/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.0.7/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.0.7/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.0.7/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.0.7/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.0.7/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1401 2024-05-24 17:17:36.428364 swarms-5.0.7/swarms/tools/__init__.py
+-rw-r--r--   0        0        0    13734 2024-05-24 16:46:49.761815 swarms-5.0.7/swarms/tools/base_tool.py
+-rw-r--r--   0        0        0     6653 2024-05-20 23:12:19.595923 swarms-5.0.7/swarms/tools/code_interpreter.py
+-rw-r--r--   0        0        0      773 2024-05-20 23:12:19.596031 swarms-5.0.7/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.0.7/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.0.7/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.0.7/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.0.7/swarms/tools/math_eval.py
+-rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.0.7/swarms/tools/openai_func_calling_schema_pydantic.py
+-rw-r--r--   0        0        0     8790 2024-05-24 17:01:49.491453 swarms-5.0.7/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.0.7/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     4275 2024-05-20 23:12:19.596541 swarms-5.0.7/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0      171 2024-05-24 17:15:20.974172 swarms-5.0.7/swarms/tools/tool.py
+-rw-r--r--   0        0        0     7152 2024-05-24 17:20:34.711837 swarms-5.0.7/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.0.7/swarms/utils/README.md
+-rw-r--r--   0        0        0     1956 2024-05-20 23:12:19.596815 swarms-5.0.7/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.0.7/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.0.7/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.0.7/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.0.7/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.0.7/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.0.7/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.0.7/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.0.7/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.0.7/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.0.7/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.0.7/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.0.7/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.0.7/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.0.7/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.0.7/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.0.7/swarms/utils/get_total_gpus.py
+-rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.0.7/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.0.7/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.0.7/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.0.7/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.0.7/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.0.7/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.0.7/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.0.7/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.0.7/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.0.7/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.0.7/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.0.7/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.0.7/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.0.7/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    35219 1970-01-01 00:00:00.000000 swarms-5.0.7/PKG-INFO
```

### Comparing `swarms-5.0.5/LICENSE` & `swarms-5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/README.md` & `swarms-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/pyproject.toml` & `swarms-5.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "5.0.5"
+version = "5.0.7"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.world"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
```

### Comparing `swarms-5.0.5/swarms/__init__.py` & `swarms-5.0.7/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/__init__.py` & `swarms-5.0.7/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/agent_wrapper.py` & `swarms-5.0.7/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/base.py` & `swarms-5.0.7/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/developer_agents.py` & `swarms-5.0.7/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/omni_modal_agent.py` & `swarms-5.0.7/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/simple_agent.py` & `swarms-5.0.7/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/tool_agent.py` & `swarms-5.0.7/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/agents/worker_agent.py` & `swarms-5.0.7/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/artifacts/base_artifact.py` & `swarms-5.0.7/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/artifacts/text_artifact.py` & `swarms-5.0.7/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/__init__.py` & `swarms-5.0.7/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/base_db.py` & `swarms-5.0.7/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/base_vectordb.py` & `swarms-5.0.7/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/dict_internal_memory.py` & `swarms-5.0.7/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/dict_shared_memory.py` & `swarms-5.0.7/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/short_term_memory.py` & `swarms-5.0.7/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/memory/visual_memory.py` & `swarms-5.0.7/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/__init__.py` & `swarms-5.0.7/swarms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/base_embedding_model.py` & `swarms-5.0.7/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/base_llm.py` & `swarms-5.0.7/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/base_multimodal_model.py` & `swarms-5.0.7/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/base_tts.py` & `swarms-5.0.7/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/base_ttv.py` & `swarms-5.0.7/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/cog_vlm.py` & `swarms-5.0.7/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/dalle3.py` & `swarms-5.0.7/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/distilled_whisperx.py` & `swarms-5.0.7/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/embeddings_base.py` & `swarms-5.0.7/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/fuyu.py` & `swarms-5.0.7/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/gemini.py` & `swarms-5.0.7/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/gpt4_vision_api.py` & `swarms-5.0.7/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/huggingface.py` & `swarms-5.0.7/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/huggingface_pipeline.py` & `swarms-5.0.7/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/idefics.py` & `swarms-5.0.7/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/kosmos_two.py` & `swarms-5.0.7/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/layoutlm_document_qa.py` & `swarms-5.0.7/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/llama3_hosted.py` & `swarms-5.0.7/swarms/models/llama3_hosted.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/llama_function_caller.py` & `swarms-5.0.7/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/llava.py` & `swarms-5.0.7/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/moondream_mm.py` & `swarms-5.0.7/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/nougat.py` & `swarms-5.0.7/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/open_dalle.py` & `swarms-5.0.7/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/open_router.py` & `swarms-5.0.7/swarms/models/open_router.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/openai_tts.py` & `swarms-5.0.7/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/popular_llms.py` & `swarms-5.0.7/swarms/models/popular_llms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/qwen.py` & `swarms-5.0.7/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/sam.py` & `swarms-5.0.7/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/sampling_params.py` & `swarms-5.0.7/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/ssd_1b.py` & `swarms-5.0.7/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/together.py` & `swarms-5.0.7/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/types.py` & `swarms-5.0.7/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/vilt.py` & `swarms-5.0.7/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/vip_llava.py` & `swarms-5.0.7/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/models/zeroscope.py` & `swarms-5.0.7/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/__init__.py` & `swarms-5.0.7/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/accountant_swarm_prompts.py` & `swarms-5.0.7/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/aga.py` & `swarms-5.0.7/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/agent_output_parser.py` & `swarms-5.0.7/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/agent_prompt.py` & `swarms-5.0.7/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/agent_prompts.py` & `swarms-5.0.7/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/agent_system_prompts.py` & `swarms-5.0.7/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/ai_research_team.py` & `swarms-5.0.7/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/aot_prompt.py` & `swarms-5.0.7/swarms/prompts/aot_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/autobloggen.py` & `swarms-5.0.7/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/autoswarm.py` & `swarms-5.0.7/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/base.py` & `swarms-5.0.7/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/chat_prompt.py` & `swarms-5.0.7/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/code_interpreter.py` & `swarms-5.0.7/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/code_spawner.py` & `swarms-5.0.7/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/debate.py` & `swarms-5.0.7/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/documentation.py` & `swarms-5.0.7/swarms/prompts/documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 def DOCUMENTATION_WRITER_SOP(
     task: str,
     module: str,
 ):
-    documentation = f"""Create multi-page long and explicit professional pytorch-like documentation for the {module} code below follow the outline for the {module} library,
+    documentation = f"""
+    Create multi-page long and explicit professional pytorch-like documentation for the {module} code below follow the outline for the {module} library,
     provide many examples and teach the user about the code, provide examples for every function, make the documentation 10,000 words,
     provide many usage examples and note this is markdown docs, create the documentation for the code to document,
     put the arguments and methods in a table in markdown to make it visually seamless
 
     Now make the professional documentation for this code, provide the architecture and how the class works and why it works that way,
     it's purpose, provide args, their types, 3 ways of usage examples, in examples show all the code like imports main example etc
```

### Comparing `swarms-5.0.5/swarms/prompts/education.py` & `swarms-5.0.7/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/finance_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/growth_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/idea2img.py` & `swarms-5.0.7/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/legal_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/logistics.py` & `swarms-5.0.7/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/meta_system_prompt.py` & `swarms-5.0.7/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-5.0.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/multi_modal_prompts.py` & `swarms-5.0.7/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-5.0.7/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/operations_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/personal_stylist.py` & `swarms-5.0.7/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/product_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/programming.py` & `swarms-5.0.7/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/project_manager.py` & `swarms-5.0.7/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/python.py` & `swarms-5.0.7/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/react.py` & `swarms-5.0.7/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/sales.py` & `swarms-5.0.7/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/sales_prompts.py` & `swarms-5.0.7/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/security_team.py` & `swarms-5.0.7/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/self_operating_prompt.py` & `swarms-5.0.7/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/summaries_prompts.py` & `swarms-5.0.7/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/support_agent_prompt.py` & `swarms-5.0.7/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/swarm_manager_agent.py` & `swarms-5.0.7/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/task_assignment_prompt.py` & `swarms-5.0.7/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/tests.py` & `swarms-5.0.7/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/urban_planning.py` & `swarms-5.0.7/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/visual_cot.py` & `swarms-5.0.7/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/worker_prompt.py` & `swarms-5.0.7/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/prompts/xray_swarm_prompt.py` & `swarms-5.0.7/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/schemas/schemas.py` & `swarms-5.0.7/swarms/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/schemas/step.py` & `swarms-5.0.7/swarms/schemas/step.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/__init__.py` & `swarms-5.0.7/swarms/structs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from swarms.structs.auto_swarm import AutoSwarm, AutoSwarmRouter
 from swarms.structs.base_structure import BaseStructure
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.structs.base_workflow import BaseWorkflow
 from swarms.structs.concurrent_workflow import ConcurrentWorkflow
 from swarms.structs.conversation import Conversation
 from swarms.structs.groupchat import GroupChat, GroupChatManager
-from swarms.structs.hiearchical_swarm import HiearchicalSwarm
 from swarms.structs.majority_voting import (
     MajorityVoting,
     majority_voting,
     most_frequent,
     parse_code_completion,
 )
 from swarms.structs.message import Message
@@ -80,14 +79,18 @@
 from swarms.structs.yaml_model import (
     YamlModel,
     create_yaml_schema_from_dict,
     get_type_name,
     pydantic_type_to_yaml_schema,
 )
 
+# New Swarms
+from swarms.structs.swarm_load_balancer import AgentLoadBalancer
+from swarms.structs.hiearchical_swarm import HiearchicalSwarm
+
 __all__ = [
     "Agent",
     "AgentJob",
     "AgentProcess",
     "AgentProcessQueue",
     "AutoSwarm",
     "AutoSwarmRouter",
```

### Comparing `swarms-5.0.5/swarms/structs/agent.py` & `swarms-5.0.7/swarms/structs/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,32 @@
 
 from swarms.memory.base_vectordb import BaseVectorDatabase
 from swarms.prompts.agent_system_prompts import AGENT_SYSTEM_PROMPT_3
 from swarms.prompts.aot_prompt import algorithm_of_thoughts_sop
 from swarms.prompts.multi_modal_autonomous_instruction_prompt import (
     MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1,
 )
-from swarms.prompts.worker_prompt import tool_usage_worker_prompt
 from swarms.structs.conversation import Conversation
 from swarms.structs.yaml_model import YamlModel
 from swarms.telemetry.user_utils import get_user_device_data
 from swarms.tools.base_tool import BaseTool
 from swarms.tools.code_interpreter import SubprocessCodeInterpreter
 from swarms.tools.pydantic_to_json import (
     base_model_to_openai_function,
     multi_base_model_to_openai_function,
 )
 from swarms.utils.data_to_text import data_to_text
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
-
+from swarms.tools.py_func_to_openai_func_str import (
+    get_openai_function_schema_from_func,
+)
+from swarms.tools.openai_tool_creator_decorator import openai_tool_executor
+from swarms.structs.base_structure import BaseStructure
+from swarms.prompts.tools import tool_sop_prompt
 
 # Utils
 # Custom stopping condition
 def stop_when_repeats(response: str) -> bool:
     # Stop if the word stop appears in the response
     return "stop" in response.lower()
 
@@ -72,15 +76,15 @@
 
 # Agent output types
 agent_output_type = Union[BaseModel, dict, str]
 ToolUsageType = Union[BaseModel, Dict[str, Any]]
 
 
 # [FEAT][AGENT]
-class Agent:
+class Agent(BaseStructure):
     """
     Agent is the backbone to connect LLMs with tools and long term memory. Agent also provides the ability to
     ingest any type of docs like PDFs, Txts, Markdown, Json, and etc for the agent. Here is a list of features.
 
     Args:
         llm (Any): The language model to use
         template (str): The template to use
@@ -178,15 +182,16 @@
         stopping_token: Optional[str] = None,
         dynamic_loops: Optional[bool] = False,
         interactive: Optional[bool] = False,
         dashboard: Optional[bool] = False,
         agent_name: Optional[str] = "swarm-worker-01",
         agent_description: Optional[str] = None,
         system_prompt: Optional[str] = AGENT_SYSTEM_PROMPT_3,
-        tools: List[BaseTool] = None,
+        # TODO: Change to callable, then parse the callable to a string
+        tools: List[Callable] = None,
         dynamic_temperature_enabled: Optional[bool] = False,
         sop: Optional[str] = None,
         sop_list: Optional[List[str]] = None,
         saved_state_path: Optional[str] = None,
         autosave: Optional[bool] = False,
         context_length: Optional[int] = 8192,
         user_name: Optional[str] = "Human:",
@@ -240,14 +245,15 @@
         rules: str = None,
         planning: Optional[str] = False,
         planning_prompt: Optional[str] = None,
         device: str = None,
         *args,
         **kwargs,
     ):
+        super().__init__(*args, **kwargs)
         self.id = id
         self.llm = llm
         self.template = template
         self.max_loops = max_loops
         self.stopping_condition = stopping_condition
         self.loop_interval = loop_interval
         self.retry_attempts = retry_attempts
@@ -372,39 +378,81 @@
         #     self.truncate_history()
 
         # If verbose is enabled then set the logger level to info
         # if verbose:
         #     logger.setLevel(logging.INFO)
 
         if tools is not None:
-            self.tool_executor = BaseTool(
-                verbose=True,
-                auto_execute_tool=execute_tool,
-                functions=tools,
+            
+            # Add the tool prompt to the memory
+            self.short_memory.add(
+                role="System", content=tool_sop_prompt()
             )
+            
 
-        # If tools are provided then set the tool prompt by adding to sop
-        if self.tools is not None:
-            if custom_tools_prompt is not None:
-                tools_prompt = custom_tools_prompt(tools=self.tools)
+            # # BaseTool
+            # self.base_tool = BaseTool(
+            #     functions=tools,
+            #     verbose=verbose,
+            #     auto_execute_tool=execute_tool,
+            #     autocheck=True,
+            #     base_models=list_base_models,
+            # )
 
-                # Append the tools prompt to the short_term_memory
-                self.short_memory.add(
-                    role=self.agent_name, content=tools_prompt
-                )
+            # Print number of tools
+            logger.info(f"Number of tools: {len(tools)}")
+            logger.info(
+                "Tools provided, Automatically converting to OpenAI function"
+            )
 
-            else:
-                # Default tool prompt
-                tools_prompt = tool_usage_worker_prompt(tools=self.tools)
+            # Now the names of the tools
+            for tool in tools:
+                logger.info(f"Tool: {tool.__name__}")
 
-                # Append the tools prompt to the short_term_memory
+            # Transform the tools into an openai schema
+            for tool in tools:
+
+                # Transform the tool into a openai function calling schema
+                tool_schema_list = get_openai_function_schema_from_func(
+                    tool,
+                    name=tool.__name__,
+                    description=tool.__doc__,
+                )
+                
+                # Transform the dictionary to a string
+                tool_schema_list = json.dumps(tool_schema_list, indent=4)
+                # print(tool_schema_list)
+
+                # Add the tool schema to the short memory
                 self.short_memory.add(
-                    role=self.agent_name, content=tools_prompt
+                    role="System", content=tool_schema_list
                 )
 
+            # Now create a function calling map for every tools
+            self.function_map = {tool.__name__: tool for tool in tools}
+
+        # # If tools are provided then set the tool prompt by adding to sop
+        # if self.tools is not None:
+        #     if custom_tools_prompt is not None:
+        #         tools_prompt = custom_tools_prompt(tools=self.tools)
+
+        #         # Append the tools prompt to the short_term_memory
+        #         self.short_memory.add(
+        #             role=self.agent_name, content=tools_prompt
+        #         )
+
+        #     else:
+        #         # Default tool prompt
+        #         tools_prompt = tool_usage_worker_prompt(tools=self.tools)
+
+        #         # Append the tools prompt to the short_term_memory
+        #         self.short_memory.add(
+        #             role=self.agent_name, content=tools_prompt
+        #         )
+
         # Set the logger handler
         if logger_handler:
             logger.add(
                 f"{self.agent_name}.log",
                 level="INFO",
                 colorize=True,
                 format=("<green>{time}</green> <level>{message}</level>"),
@@ -464,14 +512,16 @@
         if self.sop_list:
             self.sop = "\n".join(self.sop_list)
             self.short_memory.add(role=self.user_name, content=self.sop)
 
         if self.sop is not None:
             self.short_memory.add(role=self.user_name, content=self.sop)
 
+        # If the device is not provided then get the device data
+
     def set_system_prompt(self, system_prompt: str):
         """Set the system prompt"""
         self.system_prompt = system_prompt
 
     def provide_feedback(self, feedback: str) -> None:
         """Allow users to provide feedback on the responses."""
         self.feedback.append(feedback)
@@ -752,15 +802,14 @@
 
     ########################## FUNCTION CALLING ##########################
 
     def run(
         self,
         task: Optional[str] = None,
         img: Optional[str] = None,
-        function_map: Dict[str, Callable] = None,
         *args,
         **kwargs,
     ):
         """
         Run the autonomous agent loop
         """
         try:
@@ -821,33 +870,28 @@
                         # Add the response to the memory
                         self.short_memory.add(
                             role=self.agent_name, content=response
                         )
 
                         # Check if tools is not None
                         if self.tools is not None:
-                            # Extract code from markdown
-                            response = extract_code_from_markdown(response)
 
-                            # Execute the tool by name [OLD VERISON]
-                            # execute_tool_by_name(
-                            #     response,
-                            #     self.tools,
-                            #     stop_token=self.stopping_token,
-                            # )
+                            # Extract json from markdown
+                            response = extract_code_from_markdown(response)
 
                             # Try executing the tool
                             if self.execute_tool is not False:
                                 try:
                                     logger.info("Executing tool...")
 
-                                    # Execute the tool
-                                    out = self.tool_executor.execute_tool(
-                                        response,
-                                        function_map,
+                                    # try to Execute the tool and return a string
+                                    out = openai_tool_executor(
+                                        tools=response,
+                                        function_map=self.function_map,
+                                        return_as_string=True,
                                     )
 
                                     print(f"Tool Output: {out}")
 
                                     # Add the output to the memory
                                     self.short_memory.add(
                                         role=self.agent_name,
```

### Comparing `swarms-5.0.5/swarms/structs/agent_job.py` & `swarms-5.0.7/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/agent_process.py` & `swarms-5.0.7/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/async_workflow.py` & `swarms-5.0.7/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/auto_swarm.py` & `swarms-5.0.7/swarms/structs/auto_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/base_structure.py` & `swarms-5.0.7/swarms/structs/base_structure.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/base_swarm.py` & `swarms-5.0.7/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/base_workflow.py` & `swarms-5.0.7/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/company.py` & `swarms-5.0.7/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/concurrent_workflow.py` & `swarms-5.0.7/swarms/structs/concurrent_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/conversation.py` & `swarms-5.0.7/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/debate.py` & `swarms-5.0.7/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/groupchat.py` & `swarms-5.0.7/swarms/structs/groupchat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/majority_voting.py` & `swarms-5.0.7/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/message.py` & `swarms-5.0.7/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/message_pool.py` & `swarms-5.0.7/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/meta_system_prompt.py` & `swarms-5.0.7/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/multi_agent_collab.py` & `swarms-5.0.7/swarms/structs/multi_agent_collab.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 import json
 import random
 from typing import List
 
 import tenacity
-from langchain.output_parsers import RegexParser
-
 from swarms.structs.agent import Agent
 from swarms.utils.logger import logger
 from swarms.structs.base_swarm import BaseSwarm
 
 
-# utils
-class BidOutputParser(RegexParser):
-    def get_format_instructions(self) -> str:
-        return (
-            "Your response should be an integrater delimited by"
-            " angled brackets like this: <int>"
-        )
-
-
-bid_parser = BidOutputParser(
-    regex=r"<(\d+)>", output_keys=["bid"], default_output_key="bid"
-)
-
-
-# main
+# [TODO]: Add type hints
 class MultiAgentCollaboration(BaseSwarm):
     """
     Multi-agent collaboration class.
 
     Attributes:
         agents (List[Agent]): The agents in the collaboration.
         selection_function (callable): The function that selects the next speaker.
@@ -84,27 +68,33 @@
     >>> # Format the results of the multi-agent collaboration
     >>> swarm.format_results(swarm.results)
 
     """
 
     def __init__(
         self,
-        agents: List[Agent],
-        selection_function: callable = None,
+        name: str = "MultiAgentCollaboration",
+        description: str = "A multi-agent collaboration.",
+        director: Agent = None,
+        agents: List[Agent] = None,
+        select_next_speaker: callable = None,
         max_iters: int = 10,
         autosave: bool = True,
         saved_file_path_name: str = "multi_agent_collab.json",
         stopping_token: str = "<DONE>",
         logging: bool = True,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
+        self.name = name
+        self.description = description
+        self.director = director
         self.agents = agents
-        self.select_next_speaker = selection_function
+        self.select_next_speaker = select_next_speaker
         self._step = 0
         self.max_iters = max_iters
         self.autosave = autosave
         self.saved_file_path_name = saved_file_path_name
         self.stopping_token = stopping_token
         self.results = []
         self.logger = logger
@@ -117,15 +107,14 @@
         self._step += 1
 
     def step(self) -> tuple[str, str]:
         """Steps through the multi-agent collaboration."""
         speaker_idx = self.select_next_speaker(self._step, self.agents)
         speaker = self.agents[speaker_idx]
         message = speaker.send()
-        message = speaker.send()
 
         for receiver in self.agents:
             receiver.receive(speaker.name, message)
         self._step += 1
 
         if self.logging:
             self.log_step(speaker, message)
@@ -142,24 +131,18 @@
         retry=tenacity.retry_if_exception_type(ValueError),
         before_sleep=lambda retry_state: print(
             f"ValueError occured: {retry_state.outcome.exception()},"
             " retying..."
         ),
         retry_error_callback=lambda retry_state: 0,
     )
-    def ask_for_bid(self, agent) -> str:
-        """Asks an agent for a bid."""
-        bid_string = agent.bid()
-        bid = int(bid_parser.parse(bid_string)["bid"])
-        return bid
-
-    def select_next_speaker(
+    def select_next_speaker_bid(
         self,
         step: int,
-        agents,
+        agents: List[Agent],
     ) -> int:
         """Selects the next speaker."""
         bids = []
         for agent in agents:
             bid = self.ask_for_bid(agent)
             bids.append(bid)
         max_value = max(bids)
@@ -204,19 +187,22 @@
         # => director selects next speaker
         if step % 2 == 1:
             idx = 0
         else:
             idx = director.select_next_speaker() + 1
         return idx
 
-    def run(self, task: str):
+    def run(self, task: str, *args, **kwargs):
+        # [TODO]: Add type hints
+        # [TODO]: Implement the run method using step method
         conversation = task
+
         for _ in range(self.max_iters):
             for agent in self.agents:
-                result = agent.run(conversation)
+                result = agent.run(conversation, *args, **kwargs)
                 self.results.append({"agent": agent, "response": result})
                 conversation += result
 
                 if self.autosave:
                     self.save_state()
                 if result == self.stopping_token:
                     break
```

### Comparing `swarms-5.0.5/swarms/structs/multi_process_workflow.py` & `swarms-5.0.7/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/multi_threaded_workflow.py` & `swarms-5.0.7/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/rearrange.py` & `swarms-5.0.7/swarms/structs/rearrange.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/recursive_workflow.py` & `swarms-5.0.7/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/round_robin.py` & `swarms-5.0.7/swarms/structs/round_robin.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/sequential_workflow.py` & `swarms-5.0.7/swarms/structs/sequential_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/sermon_swarm.py` & `swarms-5.0.7/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/swarm_net.py` & `swarms-5.0.7/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/swarming_architectures.py` & `swarms-5.0.7/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/task.py` & `swarms-5.0.7/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/task_queue_base.py` & `swarms-5.0.7/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/structs/utils.py` & `swarms-5.0.7/swarms/structs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,28 +22,36 @@
         if line.startswith("<agent_id>") and line.endwith("</agent_id>"):
             agent_id, task = line[10:-11].split("><")
             tasks[agent_id] = task
     return tasks
 
 
 def find_agent_by_id(
-    agent_id: str = None, agents: List[Agent] = None, *args, **kwargs
+    agent_id: str = None,
+    agents: List[Agent] = None,
+    task: str = None,
+    *args,
+    **kwargs,
 ) -> Agent:
     """Find agent by id
 
     Args:
         agent_id (str, optional): _description_. Defaults to None.
         agents (List[Agent], optional): _description_. Defaults to None.
 
     Returns:
         Agent: _description_
     """
     for agent in agents:
         if agent.id == agent_id:
-            return agent
+            if task:
+                return agent.run(task, *args, **kwargs)
+            else:
+                return agent
+
     return None
 
 
 def distribute_tasks(
     task: str = None, agents: List[Agent] = None, *args, **kwargs
 ):
     """Distribute tasks to agents
```

### Comparing `swarms-5.0.5/swarms/structs/yaml_model.py` & `swarms-5.0.7/swarms/structs/yaml_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/telemetry/__init__.py` & `swarms-5.0.7/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-5.0.7/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/telemetry/check_update.py` & `swarms-5.0.7/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/telemetry/log_all.py` & `swarms-5.0.7/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/telemetry/sys_info.py` & `swarms-5.0.7/swarms/telemetry/sys_info.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/telemetry/user_utils.py` & `swarms-5.0.7/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/__init__.py` & `swarms-5.0.7/swarms/tools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from swarms.tools.exec_tool import (
-    AgentAction,
-    AgentOutputParser,
-    BaseAgentOutputParser,
-    execute_tool_by_name,
-    preprocess_json_input,
-)
+#
 from swarms.tools.tool_utils import (
     execute_tools,
     extract_tool_commands,
     parse_and_execute_tools,
     scrape_tool_func_docs,
     tool_find_by_name,
 )
 from swarms.tools.pydantic_to_json import (
     _remove_a_key,
     base_model_to_openai_function,
     multi_base_model_to_openai_function,
     function_to_str,
     functions_to_str,
 )
-from swarms.tools.openai_func_calling_schema import (
+from swarms.tools.openai_func_calling_schema_pydantic import (
     OpenAIFunctionCallSchema as OpenAIFunctionCallSchemaBaseModel,
 )
 from swarms.tools.py_func_to_openai_func_str import (
     get_openai_function_schema_from_func,
     load_basemodels_if_needed,
     get_load_param_if_needed_function,
     get_parameters,
@@ -31,19 +25,14 @@
     Function,
     ToolFunction,
 )
 from swarms.tools.openai_tool_creator_decorator import tool
 from swarms.tools.base_tool import BaseTool
 
 __all__ = [
-    "AgentAction",
-    "AgentOutputParser",
-    "BaseAgentOutputParser",
-    "execute_tool_by_name",
-    "preprocess_json_input",
     "execute_tools",
     "extract_tool_commands",
     "parse_and_execute_tools",
     "scrape_tool_func_docs",
     "tool_find_by_name",
     "_remove_a_key",
     "base_model_to_openai_function",
@@ -56,8 +45,8 @@
     "get_load_param_if_needed_function",
     "get_parameters",
     "get_required_params",
     "Function",
     "ToolFunction",
     "tool",
     "BaseTool",
-]
+]
```

### Comparing `swarms-5.0.5/swarms/tools/base_tool.py` & `swarms-5.0.7/swarms/tools/base_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,14 +327,48 @@
             raise TypeError(
                 f"Tool '{tool_name}' is not mapped to a function"
             )
 
         # Execute the tool
         return func(**tool_params)
 
+    def check_str_for_functions_valid(
+        self, output: str, function_map: Dict[str, Callable]
+    ):
+        """
+        Check if the output is a valid JSON string, and if the function name in the JSON matches any name in the function map.
+
+        Args:
+            output (str): The output to check.
+            function_map (dict): A dictionary mapping function names to functions.
+
+        Returns:
+            bool: True if the output is valid and the function name matches, False otherwise.
+        """
+        try:
+            # Parse the output as JSON
+            data = json.loads(output)
+
+            # Check if the output matches the schema
+            if (
+                data.get("type") == "function"
+                and "function" in data
+                and "name" in data["function"]
+            ):
+
+                # Check if the function name matches any name in the function map
+                function_name = data["function"]["name"]
+                if function_name in function_map:
+                    return True
+
+        except json.JSONDecodeError:
+            pass
+
+        return False
+
 
 # # Example function definitions and mappings
 # def get_current_weather(location, unit='celsius'):
 #     return f"Weather in {location} is likely sunny and 75° {unit.title()}"
 
 # def add(a, b):
 #     return a + b
```

### Comparing `swarms-5.0.5/swarms/tools/code_interpreter.py` & `swarms-5.0.7/swarms/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/function_util.py` & `swarms-5.0.7/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/json_former.py` & `swarms-5.0.7/swarms/tools/json_former.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/json_utils.py` & `swarms-5.0.7/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/logits_processor.py` & `swarms-5.0.7/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/math_eval.py` & `swarms-5.0.7/swarms/tools/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/openai_func_calling_schema.py` & `swarms-5.0.7/swarms/tools/openai_func_calling_schema_pydantic.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/openai_tool_creator_decorator.py` & `swarms-5.0.7/swarms/tools/openai_tool_creator_decorator.py`

 * *Files 27% similar despite different names*

```diff
@@ -48,16 +48,17 @@
                     verbose, bool
                 ), "verbose must be a boolean"
 
                 # Call the function
                 func(*args, **kwargs)
 
                 # Get the openai function schema
+                tool_name = name if not None else func.__name__
                 schema = get_openai_function_schema_from_func(
-                    func, name=name, description=description
+                    func, name=tool_name, description=description
                 )
 
                 # Return the schema
                 if return_dict:
                     return schema
                 elif return_string is True:
                     return str(schema)
@@ -82,67 +83,55 @@
     return decorator
 
 
 def openai_tool_executor(
     tools: List[Dict[str, Any]],
     function_map: Dict[str, Callable],
     verbose: bool = True,
+    return_as_string: bool = False,
     *args,
     **kwargs,
 ) -> Callable:
     """
     Creates a function that dynamically and concurrently executes multiple functions based on parameters specified
     in a list of tool dictionaries, with extensive error handling and validation.
 
     Args:
         tools (List[Dict[str, Any]]): A list of dictionaries, each containing configuration for a tool, including parameters.
         function_map (Dict[str, Callable]): A dictionary mapping function names to their corresponding callable functions.
+        verbose (bool): If True, enables verbose logging.
+        return_as_string (bool): If True, returns the results as a concatenated string.
 
     Returns:
         Callable: A function that, when called, executes the specified functions concurrently with the parameters given.
 
     Examples:
-    >>> from swarms.tools.openai_tool_creator_decorator import openai_tool_executor
-    >>> from swarms.tools.py_func_to_openai_func_str import get_openai_function_schema_from_func
-    >>> from swarms.utils.loguru_logger import logger
-    >>>
     >>> def test_function(param1: int, param2: str) -> str:
     ...     return f"Test function called with parameters: {param1}, {param2}"
-    ...
-    >>> @openai_tool_executor(
+
+    >>> tool_executor = openai_tool_executor(
     ...     tools=[
     ...         {
     ...             "type": "function",
     ...             "function": {
     ...                 "name": "test_function",
     ...                 "parameters": {
-    ...                     "properties": {
-    ...                         "param1": {
-    ...                             "type": "int",
-    ...                             "description": "An integer parameter."
-    ...                         },
-    ...                         "param2": {
-    ...                             "type": "str",
-    ...                             "description": "A string parameter."
-    ...                         },
-    ...                     }
+    ...                     "param1": 1,
+    ...                     "param2": "example"
     ...                 }
     ...             }
     ...         }
     ...     ],
     ...     function_map={
     ...         "test_function": test_function
-    ...     }
+    ...     },
+    ...     return_as_string=True
     ... )
-    ... def tool_executor():
-    ...     pass
-    ...
     >>> results = tool_executor()
-    >>> logger.info(results)
-
+    >>> print(results)
     """
 
     def tool_executor():
         # Prepare tasks for concurrent execution
         results = []
         logger.info(f"Executing {len(tools)} tools concurrently.")
         with concurrent.futures.ThreadPoolExecutor() as executor:
@@ -153,188 +142,58 @@
 
                 function_info = tool.get("function", {})
                 func_name = function_info.get("name")
                 logger.info(f"Executing function: {func_name}")
 
                 # Check if the function name is mapped to an actual function
                 if func_name not in function_map:
-                    raise KeyError(
-                        f"Function '{func_name}' not found in function map."
-                    )
+                    error_message = f"Function '{func_name}' not found in function map."
+                    logger.error(error_message)
+                    results.append(error_message)
+                    continue
 
                 # Validate parameters
-                params = function_info.get("parameters", {}).get(
-                    "properties", {}
-                )
+                params = function_info.get("parameters", {})
                 if not params:
-                    raise ValueError(
-                        f"No parameters specified for function '{func_name}'."
-                    )
+                    error_message = f"No parameters specified for function '{func_name}'."
+                    logger.error(error_message)
+                    results.append(error_message)
+                    continue
 
                 # Submit the function for execution
                 try:
                     future = executor.submit(
                         function_map[func_name], **params
                     )
-                    futures.append(future)
+                    futures.append((func_name, future))
                 except Exception as e:
-                    print(
-                        f"Failed to submit the function '{func_name}' for execution: {e}"
-                    )
+                    error_message = f"Failed to submit the function '{func_name}' for execution: {e}"
+                    logger.error(error_message)
+                    results.append(error_message)
 
             # Gather results from all futures
-            for future in futures:
+            for func_name, future in futures:
                 try:
                     result = future.result()  # Collect result from future
-                    results.append(result)
+                    results.append(f"{func_name}: {result}")
                 except Exception as e:
-                    print(f"Error during execution of a function: {e}")
+                    error_message = f"Error during execution of function '{func_name}': {e}"
+                    logger.error(error_message)
+                    results.append(error_message)
+
+        if return_as_string:
+            return "\n".join(results)
 
         logger.info(f"Results: {results}")
 
         return results
 
     return tool_executor
 
 
-# def openai_tool_executor(
-#     tools: List[Dict[str, Any]],
-#     function_map: Dict[str, Callable],
-#     verbose: bool = True,
-#     concurrent_execution: bool = True,
-#     retry_on_error: bool = False,
-#     retry_attempts: int = 3,
-#     max_loops: int = 1,
-#     max_workers: int = 10,
-#     *args,
-#     **kwargs,
-# ) -> Callable:
-#     """
-#     Creates a function that dynamically and concurrently executes multiple functions based on parameters specified
-#     in a list of tool dictionaries, with extensive error handling and validation.
-
-#     Args:
-#         tools (List[Dict[str, Any]]): A list of dictionaries, each containing configuration for a tool, including parameters.
-#         function_map (Dict[str, Callable]): A dictionary mapping function names to their corresponding callable functions.
-
-#     Returns:
-#         Callable: A function that, when called, executes the specified functions concurrently with the parameters given.
-
-#     Examples:
-#     >>> from swarms.tools.openai_tool_creator_decorator import openai_tool_executor
-#     >>> from swarms.tools.py_func_to_openai_func_str import get_openai_function_schema_from_func
-#     >>> from swarms.utils.loguru_logger import logger
-#     >>>
-#     >>> def test_function(param1: int, param2: str) -> str:
-#     ...     return f"Test function called with parameters: {param1}, {param2}"
-#     ...
-#     >>> @openai_tool_executor(
-#     ...     tools=[
-#     ...         {
-#     ...             "type": "function",
-#     ...             "function": {
-#     ...                 "name": "test_function",
-#     ...                 "parameters": {
-#     ...                     "properties": {
-#     ...                         "param1": {
-#     ...                             "type": "int",
-#     ...                             "description": "An integer parameter."
-#     ...                         },
-#     ...                         "param2": {
-#     ...                             "type": "str",
-#     ...                             "description": "A string parameter."
-#     ...                         },
-#     ...                     }
-#     ...                 }
-#     ...             }
-#     ...         }
-#     ...     ],
-#     ...     function_map={
-#     ...         "test_function": test_function
-#     ...     }
-#     ... )
-#     ... def tool_executor():
-#     ...     pass
-#     ...
-#     >>> results = tool_executor()
-#     >>> logger.info(results)
-
-#     """
-
-#     def tool_executor():
-#         logger.info(
-#             f"Starting execution of tools with {max_loops} loops and concurrency set to {concurrent_execution}."
-#         )
-
-#         results = []
-
-#         def execute_function(func_name, params):
-#             try:
-#                 logger.debug(
-#                     f"Executing function: {func_name} with params: {params}"
-#                 )
-#                 return function_map[func_name](**params)
-#             except Exception as e:
-#                 logger.error(
-#                     f"Error executing function {func_name}: {str(e)}"
-#                 )
-#                 if retry_on_error:
-#                     for attempt in range(retry_attempts):
-#                         try:
-#                             logger.debug(
-#                                 f"Retrying function: {func_name}, attempt {attempt+1}"
-#                             )
-#                             return function_map[func_name](**params)
-#                         except Exception as e:
-#                             logger.error(
-#                                 f"Retry {attempt+1} for function {func_name} failed: {str(e)}"
-#                             )
-#                     raise
-#                 else:
-#                     raise
-
-#         for loop in range(max_loops):
-
-#             logger.info(f"Executing loop {loop + 1}/{max_loops}")
-
-#             with concurrent.futures.ThreadPoolExecutor(
-#                 max_workers=max_workers
-#             ) as executor:
-#                 future_to_function = {
-#                     executor.submit(
-#                         execute_function,
-#                         tool["function"]["name"],
-#                         tool["function"]["parameters"]["properties"],
-#                     ): tool
-#                     for tool in tools
-#                     if tool.get("type") == "function"
-#                 }
-
-#                 for future in concurrent.futures.as_completed(
-#                     future_to_function
-#                 ):
-#                     try:
-#                         result = future.result()
-#                         results.append(result)
-#                         logger.debug(
-#                             f"Function completed with result: {result}"
-#                         )
-#                     except Exception as e:
-#                         logger.error(
-#                             f"Execution failed with error: {str(e)}"
-#                         )
-#                         continue
-
-#             logger.info(f"All loops completed. Results: {results}")
-
-#             return results
-
-#     return tool_executor
-
-
 # # Example
 # @tool(
 #     name="test_function",
 #     description="A test function that takes two parameters and returns a string.",
 # )
 # def test_function(param1: int, param2: str) -> str:
 #     return f"Test function called with parameters: {param1}, {param2}"
@@ -384,10 +243,14 @@
 #                             "description": "A string parameter.",
 #                         },
 #                     }
 #                 },
 #             },
 #         },
 #     ],
-#     function_map={"test_function": test_function, "test_function2": test_function2},
+#     function_map={
+#         "test_function": test_function,
+#         "test_function2": test_function2,
+#     },
+#     return_as_string=True,
 # )
 # print(out)
```

### Comparing `swarms-5.0.5/swarms/tools/py_func_to_openai_func_str.py` & `swarms-5.0.7/swarms/tools/py_func_to_openai_func_str.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/pydantic_to_json.py` & `swarms-5.0.7/swarms/tools/pydantic_to_json.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/tools/tool_utils.py` & `swarms-5.0.7/swarms/tools/tool_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,7 +176,38 @@
     ‘‘‘
     {docs}
     ‘‘‘
     # Response
     ‘‘‘
     """
     return PROMPT
+
+
+def is_str_valid_func_output(output: str = None, function_map: callable = None):
+    """
+    Check if the output is a valid JSON string, and if the function name in the JSON matches any name in the function map.
+
+    Args:
+        output (str): The output to check.
+        function_map (dict): A dictionary mapping function names to functions.
+
+    Returns:
+        bool: True if the output is valid and the function name matches, False otherwise.
+    """
+    try:
+        # Parse the output as JSON
+        data = json.loads(output)
+
+        # Check if the output matches the schema
+        if (data.get('type') == 'function' and 
+            'function' in data and 
+            'name' in data['function']):
+
+            # Check if the function name matches any name in the function map
+            function_name = data['function']['name']
+            if function_name in function_map:
+                return True
+
+    except json.JSONDecodeError:
+        pass
+
+    return False
```

### Comparing `swarms-5.0.5/swarms/utils/README.md` & `swarms-5.0.7/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/__init__.py` & `swarms-5.0.7/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/apa.py` & `swarms-5.0.7/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/check_function_result.py` & `swarms-5.0.7/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/class_args_wrapper.py` & `swarms-5.0.7/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/concurrent_utils.py` & `swarms-5.0.7/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/data_to_text.py` & `swarms-5.0.7/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/decorators.py` & `swarms-5.0.7/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/disable_logging.py` & `swarms-5.0.7/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/download_img.py` & `swarms-5.0.7/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/execute_futures.py` & `swarms-5.0.7/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/exponential_backoff.py` & `swarms-5.0.7/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/fetch_init_params.py` & `swarms-5.0.7/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/file_processing.py` & `swarms-5.0.7/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/find_img_path.py` & `swarms-5.0.7/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/get_logger.py` & `swarms-5.0.7/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/get_total_gpus.py` & `swarms-5.0.7/swarms/utils/get_total_gpus.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/json_output_parser.py` & `swarms-5.0.7/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/jsonl_utils.py` & `swarms-5.0.7/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/llm_metrics_decorator.py` & `swarms-5.0.7/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/logger.py` & `swarms-5.0.7/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/loggers.py` & `swarms-5.0.7/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/markdown_message.py` & `swarms-5.0.7/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/parse_code.py` & `swarms-5.0.7/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/pdf_to_text.py` & `swarms-5.0.7/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/remove_json_whitespace.py` & `swarms-5.0.7/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/save_logs.py` & `swarms-5.0.7/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/serializable.py` & `swarms-5.0.7/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/try_except_wrapper.py` & `swarms-5.0.7/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/swarms/utils/yaml_output_parser.py` & `swarms-5.0.7/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.5/PKG-INFO` & `swarms-5.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 5.0.5
+Version: 5.0.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

