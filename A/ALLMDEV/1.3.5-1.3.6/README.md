# Comparing `tmp/ALLMDEV-1.3.5-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 26441 bytes, number of entries: 22
+Zip file size: 26891 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
 -rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
 -rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
--rw-rw-rw-  2.0 fat    21304 b- defN 24-May-22 04:58 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat    19203 b- defN 24-May-24 17:34 ALLMDEV/backend.py
 -rw-rw-rw-  2.0 fat     3221 b- defN 24-May-15 11:30 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat    12685 b- defN 24-May-15 08:32 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
 -rw-rw-rw-  2.0 fat     2231 b- defN 24-May-22 04:35 ALLMDEV/serve.py
 -rw-rw-rw-  2.0 fat     1932 b- defN 24-May-15 12:35 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
 -rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
 -rw-rw-rw-  2.0 fat     2826 b- defN 24-May-14 10:42 ALLMDEV/vertexagentchat.py
 -rw-rw-rw-  2.0 fat     2126 b- defN 24-May-14 10:42 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     6093 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      591 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1698 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/RECORD
-22 files, 84116 bytes uncompressed, 23737 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat     6093 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      591 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1698 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/RECORD
+22 files, 82015 bytes uncompressed, 24187 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.5.dist-info/METADATA
+Filename: ALLMDEV-1.3.6.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.5.dist-info/WHEEL
+Filename: ALLMDEV-1.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.5.dist-info/entry_points.txt
+Filename: ALLMDEV-1.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.5.dist-info/top_level.txt
+Filename: ALLMDEV-1.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.5.dist-info/RECORD
+Filename: ALLMDEV-1.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/backend.py

```diff
@@ -1,9 +1,9 @@
-from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form
-from flask import request
+from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form, Request, HTTPException
+from flask import request, jsonify
 from pydantic import BaseModel
 from llama_index.llms.llama_cpp import LlamaCPP
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import asyncio
 import os
 import json
@@ -12,14 +12,16 @@
 from vertexai.generative_models import GenerativeModel
 from openai import AzureOpenAI
 from fastapi.responses import JSONResponse
 from langchain.document_loaders import CSVLoader, PDFMinerLoader, TextLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
+import sqlite3
+import hashlib
 
 
 
 app = FastAPI()
 
 
 
@@ -93,14 +95,31 @@
 def save_azure_config(config):
     with open(azure_config_path, "w") as f:
         json.dump(config, f, indent=4)
 def save_vertex_config(config):
     with open(vertex_config_path, "w") as f:
         json.dump(config, f, indent=4)
 
+# Database setup function
+def setup_database():
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    cursor.execute('''
+    CREATE TABLE IF NOT EXISTS users (
+        id INTEGER PRIMARY KEY AUTOINCREMENT,
+        username TEXT UNIQUE NOT NULL,
+        password TEXT NOT NULL,
+        fullname TEXT NOT NULL           
+    )
+    ''')
+
+    conn.commit()
+    conn.close()
+
 config = load_config()
 
 @app.websocket("/model_config")
 async def websocket_model_config(websocket: WebSocket):
     await websocket.accept()
     try:
         while True:
@@ -155,61 +174,54 @@
 
     except Exception as e:
         print(e)
     # finally:
     #     await websocket.close()
 
 
-
-
+    
 @app.websocket("/ws")
 async def websocket_endpoint(websocket: WebSocket):
     await websocket.accept()
     try:
         while True:
             data = await websocket.receive_json()
             print("ws route")
             user_input = data["userInput"]
-            
+            print(user_input)
             if user_input.lower() == "exit":
                 print("Exiting chat.")
                 break
-            
-            # Update config if model or temperature changes
-            # if data["model"] != config["model"] or temp != config["temperature"]:
-            #     config["model"] = data["model"]
-            #     config["temperature"] = temp
-
-            #     model_directory = "model"
-            #     for file in os.listdir(model_directory):
-            #         if file.endswith('.gguf') and config["model"].lower() in file:
-            #             config["model_path"] = os.path.join(model_directory, file)
-            #             break
-
-            #     save_config(config)
 
             prompt = prompt_template.format(prompt=user_input)
-            model_kwargs = {"n_gpu_layers" : -1 if config["gpu"] else 0}
+            model_kwargs = {"n_gpu_layers": -1 if config["gpu"] else 0}
             llm = LlamaCPP(
                 model_path=config["model_path"],
                 temperature=config["temperature"],
                 max_new_tokens=max_new_tokens,
                 context_window=3900,
                 model_kwargs=model_kwargs,
                 verbose=False,
             )
             response_iter = llm.stream_complete(prompt)
 
             for response in response_iter:
                 await websocket.send_text(response.delta)
                 await asyncio.sleep(0)
+                if websocket.client_state.name != 'CONNECTED':
+                    break
+
+            await websocket.close()
+            
 
     except Exception as e:
         print(e)
-    
+    # finally:
+    #     await websocket.close()
+
 
 @app.websocket("/available_agents")
 async def agentinfo(websocket: WebSocket):
     await websocket.accept()
     agents = os.listdir('db')
     dict = {
         'agentinfo': agents
@@ -262,70 +274,43 @@
 
             response_iter = llm.stream_complete(prompt)
 
             for response in response_iter:
                 await websocket.send_text(response.delta)
                 await asyncio.sleep(0)
 
-            # if data["model"] != config["model"] or temp != config["temperature"]:
-            #     config["model"] = data["model"]
-            #     config["temperature"] = temp
-
-            #     model_directory = "model"
-            #     for file in os.listdir(model_directory):
-            #         if file.endswith('.gguf') and config["model"].lower() in file:
-            #             config["model_path"] = os.path.join(model_directory, file)
-            #             break
 
                 save_config(config)
+            await websocket.close()
 
-           
-
+        
     except Exception as e:
         print(e)
-    finally:
-        await websocket.close()
+    # finally:
+    #     await websocket.close()
 
 @app.websocket("/vertex")
 async def websocket_endpoint(websocket: WebSocket):
     await websocket.accept()
     try:
         config=load_vertex_config()
-        # model_kwargs = {"n_gpu_layers" : -1 if config["gpu"] else 0}
-        # llm = LlamaCPP(
-        #     model_path=config["model_path"],
-        #     temperature=config["temperature"],
-        #     max_new_tokens=max_new_tokens,
-        #     context_window=3900,
-        #     model_kwargs=model_kwargs,
-        #     verbose=False,
-        # )
         while True:
             data = await websocket.receive_json()
             print(data)
             print("vertex route")
             prompt = data["userInput"]
             
             if prompt.lower() == "exit":
                 print("Exiting chat.")
                 break
 
             agent = data['agent']
             projectid=config["project_id"]
             region=config["region"]
             model=config["model"]
-            # projectid=data['projectId']
-            # region=data['region']
-            # model=data['modelInput']
-
-            # if model != config["model"] or projectid!= config["projectId"]:
-            #     config["model"] = model
-            #     config["projectId"] = projectid
-            #     config["region"] = region
-            #     save_vertex_config(config)
             vertexai.init(project=projectid, location=region)
             multimodal_model = GenerativeModel(model_name=model)
             if agent == "None":
                 response = multimodal_model.generate_content(prompt)
                 await websocket.send_text(response.text)
             else:
 
@@ -335,66 +320,28 @@
 
                 docs = db.similarity_search(prompt, k=3)
                 context = docs[0].page_content
                 prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query:<s>[INST] {prompt} [/INST]"
                 prompt = prompt_template.format(context=context, prompt=prompt)
                 response = multimodal_model.generate_content(prompt)
                 await websocket.send_text(response.text)
-
-            
-
-
-            # model_kwargs = {"n_gpu_layers" : -1 if config["gpu"] else 0}
-            # llm = LlamaCPP(
-            #     model_path=config["model_path"],
-            #     temperature=config["temperature"],
-            #     max_new_tokens=max_new_tokens,
-            #     context_window=3900,
-            #     model_kwargs=model_kwargs,
-            #     verbose=False,
-            # )
-
-            # response_iter = llm.stream_complete(prompt)
-
-            # for response in response_iter:
-            #     await websocket.send_text(response.delta)
-            await asyncio.sleep(0)
-
-            # if data["model"] != config["model"] or temp != config["temperature"]:
-            #     config["model"] = data["model"]
-            #     config["temperature"] = temp
-
-            #     model_directory = "model"
-            #     for file in os.listdir(model_directory):
-            #         if file.endswith('.gguf') and config["model"].lower() in file:
-            #             config["model_path"] = os.path.join(model_directory, file)
-            #             break
-
+                await websocket.close()
            
 
     except Exception as e:
         print(e)
-    finally:
-        await websocket.close()
+    # finally:
+    #     await websocket.close()
 
 @app.websocket("/azure")
 async def websocket_endpoint(websocket: WebSocket):
     await websocket.accept()
     try:
         config=load_azure_config()
 
-        # model_kwargs = {"n_gpu_layers" : -1 if config["gpu"] else 0}
-        # llm = LlamaCPP(
-        #     model_path=config["model_path"],
-        #     temperature=config["temperature"],
-        #     max_new_tokens=max_new_tokens,
-        #     context_window=3900,
-        #     model_kwargs=model_kwargs,
-        #     verbose=False,
-        # )
         while True:
             data = await websocket.receive_json()
             print(data)
             print("azure route")
             prompt = data["userInput"]
             
             if prompt.lower() == "exit":
@@ -403,20 +350,15 @@
 
             agent = data['agent']
             key=config['apikey']
             version=config['version']
             model=config['modelInput']
             endpoint=config['endpoint']
 
-            # if model != config["model"] or endpoint!= config["endpoint"]:
-            #     config["model"] = model
-            #     config["endpoint"] = endpoint
-            #     config["version"] = version
-            #     config["key"] = key
-            #     save_azure_config(config)
+
             client = AzureOpenAI(
                 api_key = (key),
                 api_version = version,
                 azure_endpoint = (endpoint)
             )
 
             if agent == "None":
@@ -444,49 +386,25 @@
                             messages=[
                                 {"role": "system", "content": "Assistant is a large language model trained by OpenAI."},
                                 {"role": "user", "content": prompt}
                                 
                             ]
                         )
                     for choice in response.choices:
-                            await websocket.send_text(choice.message.content)
-
-
-            # model_kwargs = {"n_gpu_layers" : -1 if config["gpu"] else 0}
-            # llm = LlamaCPP(
-            #     model_path=config["model_path"],
-            #     temperature=config["temperature"],
-            #     max_new_tokens=max_new_tokens,
-            #     context_window=3900,
-            #     model_kwargs=model_kwargs,
-            #     verbose=False,
-            # )
-
-            # response_iter = llm.stream_complete(prompt)
+                        await websocket.send_text(choice.message.content)
+                    await websocket.close()
+                        
 
-            # for response in response_iter:
-            #     await websocket.send_text(response.delta)
-            await asyncio.sleep(0)
-
-            # if data["model"] != config["model"] or temp != config["temperature"]:
-            #     config["model"] = data["model"]
-            #     config["temperature"] = temp
-
-            #     model_directory = "model"
-            #     for file in os.listdir(model_directory):
-            #         if file.endswith('.gguf') and config["model"].lower() in file:
-            #             config["model_path"] = os.path.join(model_directory, file)
-            #             break
 
            
 
     except Exception as e:
         print(e)
-    finally:
-        await websocket.close()
+    # finally:
+    #     await websocket.close()
 
 
 # class RequestData(BaseModel):
 #     agent: str
 #     file: UploadFile
 @app.post("/create_agent")
 async def upload_file(name: str = Form(...),file: UploadFile = File(...)):
@@ -561,14 +479,73 @@
             await websocket.send_json(config)
 
     except Exception as e:
         print(e)
     finally:
         await websocket.close()
 
+@app.route('/signup', methods=['POST'])
+async def signup(request: Request):
+    data = await request.json()
+    print(data)
+    fullname = data.get('fullname')
+    username = data.get('username')
+    password = data.get('password')
+
+    hashed_password = hashlib.sha256(password.encode()).hexdigest()
+
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    if '@' in username:
+        try:
+            cursor.execute('''
+            INSERT INTO users (username, password, fullname) VALUES (?, ?, ?)
+            ''', (username, hashed_password, fullname))
+            conn.commit()
+            response = {'message': 'User signed up successfully!'}
+        except sqlite3.IntegrityError:
+            response = {'message': 'Username already exists!'}
+    else:
+        response = {'message': 'Invalid email format.'}
+    
+    
+
+    conn.close()
+    return JSONResponse(content=response)
+
+# Route for user login
+@app.route('/login', methods=['POST'])
+async def login(request: Request):
+    data = await request.json()
+    username = data.get('username')
+    password = data.get('password')
+
+    if not username or not password:
+        raise HTTPException(status_code=400, detail="Username and password required")
+
+    hashed_password = hashlib.sha256(password.encode()).hexdigest()
+
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    cursor.execute('''
+    SELECT * FROM users WHERE username = ? AND password = ?
+    ''', (username, hashed_password))
+
+    user = cursor.fetchone()
+
+    if user:
+        response = {'message': 'Login successful!'}
+    else:
+        response = {'message': 'Invalid username or password.'}
+
+    conn.close()
+    return JSONResponse(content=response)
+
 def main():
     import uvicorn
-
+    setup_database()
     uvicorn.run(app, host="0.0.0.0", port=8000)
 
 if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV-1.3.5.dist-info/METADATA` & `ALLMDEV-1.3.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.5
+Version: 1.3.6
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
```

## Comparing `ALLMDEV-1.3.5.dist-info/entry_points.txt` & `ALLMDEV-1.3.6.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ALLMDEV-1.3.5.dist-info/RECORD` & `ALLMDEV-1.3.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
 ALLMDEV/agentapi.py,sha256=vnkpCaviW0w5EQTE99els4Nb8QABv0TgNoP2FdFsWVQ,3706
 ALLMDEV/agentchat.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
 ALLMDEV/azureagentapi.py,sha256=dzMwkJHfRBqRxYAwpe_aQRgASqnsNBaEzT9jsc791QQ,4986
 ALLMDEV/azureagentchat.py,sha256=6L9m2B6dfe9LUWdd_Vj6_TT1n1GBXxVvqOeA-yTuV_Q,3298
 ALLMDEV/azurecli.py,sha256=nLoSVPpxWwIJWhiddB0_qzNw53hrAE6ijK0diDlaGYs,2435
-ALLMDEV/backend.py,sha256=01c2CYAhM4jdKfld2A06i0UnfL-48bfEy-9QR8MIaVU,21304
+ALLMDEV/backend.py,sha256=b2GcDlcgeyMbwMcyLtrYGCTPS8v68NAylj9LMXqBdt0,19203
 ALLMDEV/cli.py,sha256=13o2i7g_DtOyP8N8x7QdMr8iUGr4raJX26NJ9oqpgNw,3221
 ALLMDEV/instruct.py,sha256=-3ybhrmAwgLy_MptpJHhFnbQq1NcT4DHeMV2-46Tzl8,12685
 ALLMDEV/newagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/serve.py,sha256=RUKwji_795izII7XlYku1KUK6bvgR_SYBB9N34GwqUA,2231
 ALLMDEV/studio.py,sha256=LlrIEWcs-o8cIjnprJVijR8cNxrOsnFvl9AgTrk43iw,1932
 ALLMDEV/test.py,sha256=CxP_WW9ZXEiLCJh_9MLdieFU-yfNMwWlXrcrs7gtXx8,683
 ALLMDEV/updateagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/vertexagentapi.py,sha256=fPbLJoy8Wirh7wPc31EzlgLSqfF2e4PkEwYCO9h4yqk,4530
 ALLMDEV/vertexagentchat.py,sha256=dYvJ2_teBGeEN3TTrXq4pSulYJW5kmNPKFa9xg9ec9s,2826
 ALLMDEV/vertexcli.py,sha256=-5BgOKO7oMsjcsJRluAM0ivWllzpBpWmVQIzHbq_Xrk,2126
-ALLMDEV-1.3.5.dist-info/METADATA,sha256=Rcy8ENFYB-53J9q82bog0Jl3TR8W9VAPTz-R1hC46KU,6093
-ALLMDEV-1.3.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.3.5.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
-ALLMDEV-1.3.5.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.3.5.dist-info/RECORD,,
+ALLMDEV-1.3.6.dist-info/METADATA,sha256=QA5iZEbmyTb4ZhlkxjmrD8iQaTthyZp1ju4eAqS_57Y,6093
+ALLMDEV-1.3.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.3.6.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
+ALLMDEV-1.3.6.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.3.6.dist-info/RECORD,,
```

