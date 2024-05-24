# Comparing `tmp/taskgen_ai-2.3.0.tar.gz` & `tmp/taskgen_ai-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-2.3.0.tar", last modified: Sat May 18 07:31:41 2024, max compression
+gzip compressed data, was "taskgen_ai-2.3.1.tar", last modified: Fri May 24 15:49:40 2024, max compression
```

## Comparing `taskgen_ai-2.3.0.tar` & `taskgen_ai-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-18 07:31:41.566524 taskgen_ai-2.3.0/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.3.0/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-18 07:31:41.565792 taskgen_ai-2.3.0/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    21057 2024-05-18 07:30:29.000000 taskgen_ai-2.3.0/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      684 2024-05-18 07:30:38.000000 taskgen_ai-2.3.0/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-18 07:31:41.566612 taskgen_ai-2.3.0/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      230 2024-05-18 07:30:34.000000 taskgen_ai-2.3.0/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-18 07:31:41.561894 taskgen_ai-2.3.0/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      237 2024-05-17 02:04:12.000000 taskgen_ai-2.3.0/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    34907 2024-05-18 07:25:50.000000 taskgen_ai-2.3.0/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33048 2024-05-18 07:30:18.000000 taskgen_ai-2.3.0/taskgen/base.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    19279 2024-05-17 05:44:25.000000 taskgen_ai-2.3.0/taskgen/function.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-18 07:31:41.564751 taskgen_ai-2.3.0/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-18 07:31:41.000000 taskgen_ai-2.3.0/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      283 2024-05-18 07:31:41.000000 taskgen_ai-2.3.0/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-18 07:31:41.000000 taskgen_ai-2.3.0/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       43 2024-05-18 07:31:41.000000 taskgen_ai-2.3.0/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-18 07:31:41.000000 taskgen_ai-2.3.0/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-24 15:49:40.000617 taskgen_ai-2.3.1/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.3.1/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-24 15:49:39.999879 taskgen_ai-2.3.1/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    21057 2024-05-24 15:27:57.000000 taskgen_ai-2.3.1/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      684 2024-05-24 15:27:59.000000 taskgen_ai-2.3.1/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-24 15:49:40.000748 taskgen_ai-2.3.1/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      230 2024-05-24 15:28:00.000000 taskgen_ai-2.3.1/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-24 15:49:39.995235 taskgen_ai-2.3.1/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      237 2024-05-17 02:04:12.000000 taskgen_ai-2.3.1/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    36778 2024-05-24 15:26:23.000000 taskgen_ai-2.3.1/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    33671 2024-05-24 15:28:06.000000 taskgen_ai-2.3.1/taskgen/base.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    19279 2024-05-24 04:30:41.000000 taskgen_ai-2.3.1/taskgen/function.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-24 15:49:39.999001 taskgen_ai-2.3.1/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      283 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       43 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-2.3.0/LICENSE` & `taskgen_ai-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-2.3.0/PKG-INFO` & `taskgen_ai-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.3.0
+Version: 2.3.1
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 Requires-Dist: termcolor>=2.3.0
 
-# TaskGen v2.3.0
+# TaskGen v2.3.1
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

### Comparing `taskgen_ai-2.3.0/README.md` & `taskgen_ai-2.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TaskGen v2.3.0
+# TaskGen v2.3.1
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

### Comparing `taskgen_ai-2.3.0/pyproject.toml` & `taskgen_ai-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "2.3.0"
+version = "2.3.1"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `taskgen_ai-2.3.0/taskgen/agent.py` & `taskgen_ai-2.3.1/taskgen/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,18 +143,19 @@
         ''' Returns whether or not the memory is empty '''
         return self.memory == []
     
 class Agent:
     def __init__(self, agent_name: str = 'Helpful Assistant',
                  agent_description: str = 'A generalist agent meant to help solve problems',
                  max_subtasks: int = 5,
-                 summarise_subtasks_count: int = 3,
+                 summarise_subtasks_count: int = 5,
                  memory_bank = None,
                  shared_variables = None,
                  get_global_context = None,
+                 global_context = '',
                  default_to_llm = True,
                  verbose: bool = True,
                  debug: bool = False,
                  llm = None,
                  **kwargs):
         ''' 
         Creates an LLM-based agent using description and outputs JSON based on output_format. 
@@ -171,14 +172,15 @@
         - memory_bank: class Dict[Memory]. Stores multiple types of memory for use by the agent. Customise the Memory config within the Memory class.
             - Key: `Function` (Already Implemented Natively) - Does RAG over Task -> Function mapping
             - Can add in more keys that would fit your use case. Retrieves similar items to task / overall plan (if able) for additional context in `get_next_subtasks()` and `use_llm()` function
             - For RAG over Documents, it is best done in a function of the Agent to retrieve more information when needed (so that we do not overload the Agent with information)
         - shared_variables. Dict. Default: None. Stores the variables to be shared amongst inner functions and agents. 
             If not empty, will pass this dictionary by reference down to the inner agents and functions
         - get_global_context. Function. Takes in self (agent variable) and returns the additional prompt (str) to be appended to `get_next_subtask` and `use_llm`. Allows for persistent agent states to be added to the prompt
+        - global_context. String. Additional global context in string form. Put in variables to substitute for shared_variables using <>
         - default_to_llm. Bool. Default: True. Whether to default to use_llm function if there is no match to other functions. If False, use_llm will not be given to Agent
         - verbose: Bool. Default: True. Whether to print out intermediate thought processes of the Agent
         - debug: Bool. Default: False. Whether to debug StrictJSON messages
         - llm: Function. The llm parameter that gets passed into Function/strict_json
         
         Inputs (optional):
         - **kwargs: Dict. Additional arguments you would like to pass on to the strict_json function
@@ -187,23 +189,27 @@
         self.agent_name = agent_name
         self.agent_description = agent_description
         self.max_subtasks = max_subtasks
         self.summarise_subtasks_count = summarise_subtasks_count
         self.verbose = verbose
         self.default_to_llm = default_to_llm
         self.get_global_context = get_global_context
+        self.global_context = global_context
 
         self.debug = debug
         self.llm = llm
         
         # set shared variables
         if shared_variables is None:
             self.shared_variables = {}
         else:
             self.shared_variables = shared_variables
+        # append agent to shared variables, so that functions have access to it
+        self.shared_variables['agent'] = self
+        
         # set memory bank
         if memory_bank is None:
             self.memory_bank = {'Function': Memory(top_k = 5, mapper = lambda x: x.fn_name + ': ' + x.fn_description, approach = 'retrieve_by_ranker')}
             self.memory_bank['Function'].reset()
         else:
             self.memory_bank = memory_bank
             
@@ -221,15 +227,15 @@
         if self.default_to_llm:
             self.assign_functions([Function(fn_name = 'use_llm', 
                                         fn_description = f'For general tasks. Used only when no other function can do the task', 
                                         is_compulsory = True,
                                         output_format = {"Output": "Output of LLM"})])
         # adds the end task function
         self.assign_functions([Function(fn_name = 'end_task',
-                                       fn_description = 'Use only after task is completed',
+                                       fn_description = 'Passes the final output to the user',
                                        is_compulsory = True,
                                        output_format = {})])
         
     def save_agent(self, filename: str):
         ''' Saves the entire agent to filename for reuse next time '''
         
         if not isinstance(filename, str):
@@ -287,26 +293,35 @@
             filtered_fn_list = self.memory_bank['Function'].retrieve(task)
             
             # add back compulsory functions (default: use_llm, end_task) if present in function_map
             for name, function in self.function_map.items():
                 if function.is_compulsory:
                     filtered_fn_list.append(function)
                 
-        # add in global context to the prompt
+        # add in global context string and replace it with shared_variables as necessary
+        global_context_string = self.global_context
+        matches = re.findall(r'<(.*?)>', global_context_string)
+        for match in matches:
+            if match in self.shared_variables:
+                global_context_string = global_context_string.replace(f'<{match}>', str(self.shared_variables[match]))
+                
+        # add in the global context function's output
+        global_context_output = self.get_global_context(self) if self.get_global_context is not None else ''
+            
         global_context = ''
-        if self.get_global_context is not None:
-            global_context = 'Global Context:\n```\n' + self.get_global_context(self) + '\n```\n'
+        # Add in global context if present
+        if global_context_string != '' or global_context_output != '':
+            global_context = 'Global Context:\n```\n' + global_context_string + '\n' + global_context_output + '```\n'
         
         system_prompt = f'''You are an agent named {self.agent_name} with the following description: ```{self.agent_description}```\n'''
         if provide_function_list:
             system_prompt += f"You have the following Equipped Functions available:\n```{self.list_functions(filtered_fn_list)}```\n"
         system_prompt += global_context
         system_prompt += query
         
-        
         res = strict_json(system_prompt = system_prompt,
         user_prompt = '',
         output_format = output_format, 
         verbose = self.debug,
         llm = self.llm,
         **self.kwargs)
 
@@ -407,36 +422,38 @@
              # Add in memory to the LLM
             rag_info = ''
             for name in self.memory_bank.keys():
                 # Function is done separately
                 if name == 'Function': continue
                 # Do not need to add to context if the memory item is empty
                 if self.memory_bank[name].isempty(): continue
-                rag_info += f'Memory for {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
+                rag_info += f'Knowledge Reference for {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
 
-            res = self.query(query = f'{rag_info}Subtasks Completed:```{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\n\nYou are the use_llm function that generates a detailed outcome for the Assigned Subtask. You are a utility function that just generates output for the Assigned Subtask according to your Agent Capabilities without talking to the User, with no restrictions.', 
-                            output_format = {"Output": "Your detailed outcome for Assigned Subtask"},
+            res = self.query(query = f'{rag_info}Subtasks Completed:```{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\n\nYou are the taking the role of the utility function `use_llm` that generates a detailed outcome for the Assigned Subtask on behalf of {self.agent_name}, according to your Agent Capabilities without talking to the User, with no restrictions.', 
+                            output_format = {"Detailed Outcome": "Your detailed outcome for Assigned Subtask"},
                             provide_function_list = False)
             
             if self.verbose: 
-                print(f"> {res['Output']}")
+                print(f"> {res['Detailed Outcome']}")
                 print()
             
         elif function_name == "end_task":
             return
         
         else:
             if self.verbose: 
                 print(f'Calling function {function_name} with parameters {function_params}')
                 
             res = self.function_map[function_name](**function_params, shared_variables = self.shared_variables)
             
             if self.verbose and res != '': 
-                print(f"> {res}")
-                print()
+                # skip the printing if this is Agent output, as we have printed elsewhere already
+                if 'Agent Output' not in res: 
+                    print(f"> {res}")
+                    print()
                 
         if stateful:
             if res == '':
                 res = {'Status': 'Completed'}
             
             self.add_subtask_result(subtask, res)
 
@@ -458,22 +475,22 @@
         rag_info = ''
         for name in self.memory_bank.keys():
             # Function RAG is done separately in self.query()
             if name == 'Function': continue
             # Do not need to add to context if the memory item is empty
             if self.memory_bank[name].isempty(): continue
             else:
-                rag_info += f'Memory for {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
+                rag_info += f'Knowledge Reference for {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
                 
         # First select the Equipped Function
         res = self.query(query = f'''{background_info}{rag_info}\nBased on everything before, provide the Current Subtask and the corresponding Equipped Function to complete a part of Assigned Task.
-You are only given the Assigned Task from User with no further inputs. The last part of Assigned Task is to End Task.''',
+You are only given the Assigned Task from User with no further inputs. Do not do more than required. The last subtask of Assigned Task is End Task''',
          output_format = {"Observation": "Reflect on what has been done in Subtasks Completed for Assigned Task", 
-                          "Thoughts": "Brainstorm on how to complete remainder of Assigned Task in detail given Observation and Subtasks Completed", 
-                          "Current Subtask": "What to do now in detail that can be done by one Equipped Function for Assigned Task", 
+                          "Thoughts": "Brainstorm how to complete remainder of Assigned Task only given Observation, End Task if completed", 
+                          "Current Subtask": "What to do now in detail with all context provided that can be done by one Equipped Function for Assigned Task", 
                           "Equipped Function": "Name of Equipped Function to use for Current Subtask"},
              provide_function_list = True,
              task = task)
 
         if self.verbose:
             print(colored(f"Observation: {res['Observation']}", 'black', attrs = ['bold']))
             print(colored(f"Thoughts: {res['Thoughts']}", 'green', attrs = ['bold']))
@@ -510,17 +527,17 @@
             input_format["Actual Subtask"] = "Edit Current Subtask to suit actual function call"
                     
             # if there is no input, then do not need LLM to extract out function's input
             if input_format == {}:
                 res["Equipped Function Inputs"] = {}
                     
             else:    
-                res2 = self.query(query = f'''{background_info}{rag_info}\n\nThoughts: {res["Thoughts"]}\nCurrent Subtask: {res["Current Subtask"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask.
-Write a Actual Subtask stating the actual input values input parameters according to what is actually done for the Equipped Function.
-Make sure the Actual Subtask is detailed and can be interpreted without reference to any context.''',
+                res2 = self.query(query = f'''{background_info}{rag_info}\n\nThoughts: {res["Thoughts"]}\nCurrent Subtask: {res["Current Subtask"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for {matches} to fulfil Current Subtask.
+Write an Updated Subtask stating the actual input values according to what is actually done for the Equipped Function.
+Make sure the Updated Subtask is detailed and can be interpreted without reference to any context.''',
                              output_format = input_format,
                              provide_function_list = False)
                 
                 # Rephrase the Current Subtask to suit what is actually done
                 res["Current Subtask"] = res2["Actual Subtask"]
                 
                 # store the rest of the function parameters
@@ -552,27 +569,28 @@
     def summarise_subtasks_completed(self, task: str = ''):
         ''' Summarise the subtasks_completed list according to task '''
 
         output = self.reply_user(task)
         # Create a new summarised subtasks completed list
         self.subtasks_completed = {f"Current Results for '{task}'": output}
         
-    def reply_user(self, query: str = '', stateful: bool = True):
+    def reply_user(self, query: str = '', stateful: bool = True, verbose: bool = True):
         ''' Generate a reply to the user based on the query / agent task and subtasks completed
-        If stateful, also store this interaction into the subtasks_completed'''
+        If stateful, also store this interaction into the subtasks_completed
+        If verbose is given, can also override the verbosity of this function'''
         
         my_query = self.task if query == '' else query
             
-        res = self.query(query = f'Subtasks Completed: ```{self.subtasks_completed}```\nAssigned Task: ```{my_query}```\nRespond to the Assigned Task in detail using information from Global Context and Subtasks Completed only. Do not generate anything new.', 
+        res = self.query(query = f'Subtasks Completed: ```{self.subtasks_completed}```\nAssigned Task: ```{my_query}```\nRespond to the Assigned Task in detail using information from Global Context and Subtasks Completed only. Be factual and do not generate any new information.', 
                                     output_format = {"Response to Assigned Task": "Detailed Response"},
                                     provide_function_list = False)
         
         res = res["Response to Assigned Task"]
         
-        if self.verbose:
+        if self.verbose and verbose:
             print(res)
         
         if stateful:
             self.add_subtask_result(my_query, res)
         
         return res
 
@@ -623,29 +641,29 @@
                     print(colored(f"Subtask identified: {subtask}", "blue", attrs=['bold']))
 
                 # Execute the function for next step
                 res = self.use_function(function_name, function_params, subtask)
                 
                 # Summarise Subtasks Completed if necessary
                 if len(self.subtasks_completed) > self.summarise_subtasks_count:
-                    print('### Auto-summarising Subtasks Completed ###')
+                    print('### Auto-summarising Subtasks Completed (Change frequency via `summarise_subtasks_count` variable) ###')
                     self.summarise_subtasks_completed(f'progress for {self.overall_task}')
                     print('### End of Auto-summary ###\n')
           
         return list(self.subtasks_completed.values())
     
     ## This is for Multi-Agent uses
     def to_function(self, meta_agent):
         ''' Converts the agent to a function so that it can be called by another agent
         The agent will take in an instruction, and output the result after processing'''
 
         # makes the agent appear as a function that takes in an instruction and outputs the executed instruction
         my_fn = Function(fn_name = self.agent_name,
                              fn_description = f'Agent Description: ```{self.agent_description}```\nExecutes the given <instruction>',
-                             output_format = {"Output": "Output of instruction"},
+                             output_format = {"Agent Output": "Output of instruction"},
                              external_fn = Agent_External_Function(self, meta_agent))
         
         return my_fn
     
     def assign_agents(self, agent_list: list):
         ''' Assigns a list of Agents to the main agent, passing in the meta agent as well '''
         if not isinstance(agent_list, list):
@@ -674,13 +692,24 @@
             print(f'\n### Start of Inner Agent: {self.agent.agent_name} ###')
         agent_copy = copy.deepcopy(self.agent)
         
         # take the shared variables from the meta agent
         agent_copy.shared_variables = self.meta_agent.shared_variables
         
         # provide the subtasks completed and debug capabilities to the inner agents too
+        agent_copy.reset()
         agent_copy.debug = self.meta_agent.debug
-        agent_copy.subtasks_completed = self.meta_agent.subtasks_completed
+        if len(self.meta_agent.subtasks_completed) > 0:
+            agent_copy.global_context += f'Related Subtasks Completed: {self.meta_agent.subtasks_completed}'
+        agent_copy.subtasks_completed = {}
 
         output = agent_copy.run(instruction, self.meta_agent.overall_task)
+        
+        # append result of inner agent to meta agent
+        agent_copy.verbose = False
+        agent_reply = agent_copy.reply_user()
+        
         if self.agent.verbose:
+            print(colored(f'###\nReply from {self.agent.agent_name} to {self.meta_agent.agent_name}:\n{agent_reply}\n###\n', 'magenta', attrs = ['bold']))
             print(f'### End of Inner Agent: {self.agent.agent_name} ###\n')
+            
+        return agent_reply
```

### Comparing `taskgen_ai-2.3.0/taskgen/base.py` & `taskgen_ai-2.3.1/taskgen/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,21 @@
     match = re.search(r"list\[(.*)\]", data_type, re.IGNORECASE)
     if match:
         internal_data_type = match.group(1)  # Extract the content inside the brackets
         # do processing for internal elements
         for num in range(len(field)):
             field[num] = check_datatype(field[num], 'array element of '+key, internal_data_type, **kwargs)
             
+    match = re.search(r"array\[(.*)\]", data_type, re.IGNORECASE)
+    if match:
+        internal_data_type = match.group(1)  # Extract the content inside the brackets
+        # do processing for internal elements
+        for num in range(len(field)):
+            field[num] = check_datatype(field[num], 'array element of '+key, internal_data_type, **kwargs)
+            
     # if it is not nested, check individually
     else:
         # check for string
         if data_type.lower() == 'str':
             try:
                 # convert to string and remove escape characters from indents and quotations
                 field = str(field)
@@ -156,14 +163,18 @@
                 pass
             if not isinstance(field, str):
                 raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
             # do decoding for double backslashes
             field = bytes(field, "utf-8").decode("unicode_escape")
             # replace aprostrophes
             field = field.replace("â\x80\x99", "'")
+            # remove the python and ```, whitespace at the front and back of code if any
+            field = re.sub(r"^(\s|`)*(?i:python)?\s*", "", field)
+            # Removes whitespace & ` from end
+            field = re.sub(r"(\s|`)*$", "", field)
                 
         # check for int
         if data_type.lower() == 'int':
             try:
                 field = int(field)
             except Exception as e:
                 pass
```

### Comparing `taskgen_ai-2.3.0/taskgen/function.py` & `taskgen_ai-2.3.1/taskgen/function.py`

 * *Files identical despite different names*

### Comparing `taskgen_ai-2.3.0/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-2.3.1/taskgen_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.3.0
+Version: 2.3.1
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 Requires-Dist: termcolor>=2.3.0
 
-# TaskGen v2.3.0
+# TaskGen v2.3.1
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

