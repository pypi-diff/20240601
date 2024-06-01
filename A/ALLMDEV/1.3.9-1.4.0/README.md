# Comparing `tmp/ALLMDEV-1.3.9-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,27 @@
-Zip file size: 39024 bytes, number of entries: 24
+Zip file size: 40622 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
--rw-rw-rw-  2.0 fat    34900 b- defN 24-May-31 13:56 ALLMDEV/api.py
+-rw-rw-rw-  2.0 fat    35243 b- defN 24-Jun-01 11:46 ALLMDEV/api.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
 -rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
 -rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
--rw-rw-rw-  2.0 fat    35338 b- defN 24-May-31 13:56 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat    38780 b- defN 24-Jun-01 18:04 ALLMDEV/backend.py
 -rw-rw-rw-  2.0 fat     4952 b- defN 24-May-25 12:45 ALLMDEV/chat_history.py
 -rw-rw-rw-  2.0 fat     3221 b- defN 24-May-15 11:30 ALLMDEV/cli.py
+-rw-rw-rw-  2.0 fat     1314 b- defN 24-Jun-01 13:45 ALLMDEV/email_test.py
 -rw-rw-rw-  2.0 fat    12685 b- defN 24-May-15 08:32 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
 -rw-rw-rw-  2.0 fat     2231 b- defN 24-May-22 04:35 ALLMDEV/serve.py
 -rw-rw-rw-  2.0 fat     1932 b- defN 24-May-15 12:35 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
 -rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
 -rw-rw-rw-  2.0 fat     2826 b- defN 24-May-14 10:42 ALLMDEV/vertexagentchat.py
 -rw-rw-rw-  2.0 fat     2126 b- defN 24-May-14 10:42 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     6145 b- defN 24-May-31 14:28 ALLMDEV-1.3.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-31 14:28 ALLMDEV-1.3.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      589 b- defN 24-May-31 14:28 ALLMDEV-1.3.9.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-31 14:28 ALLMDEV-1.3.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1850 b- defN 24-May-31 14:28 ALLMDEV-1.3.9.dist-info/RECORD
-24 files, 138204 bytes uncompressed, 36094 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat     6145 b- defN 24-Jun-01 18:06 ALLMDEV-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-01 18:06 ALLMDEV-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      589 b- defN 24-Jun-01 18:06 ALLMDEV-1.4.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Jun-01 18:06 ALLMDEV-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1928 b- defN 24-Jun-01 18:06 ALLMDEV-1.4.0.dist-info/RECORD
+25 files, 143381 bytes uncompressed, 37574 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: ALLMDEV/chat_history.py
 Comment: 
 
 Filename: ALLMDEV/cli.py
 Comment: 
 
+Filename: ALLMDEV/email_test.py
+Comment: 
+
 Filename: ALLMDEV/instruct.py
 Comment: 
 
 Filename: ALLMDEV/newagent.py
 Comment: 
 
 Filename: ALLMDEV/serve.py
@@ -51,23 +54,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.9.dist-info/METADATA
+Filename: ALLMDEV-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.9.dist-info/WHEEL
+Filename: ALLMDEV-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.9.dist-info/entry_points.txt
+Filename: ALLMDEV-1.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.9.dist-info/top_level.txt
+Filename: ALLMDEV-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.9.dist-info/RECORD
+Filename: ALLMDEV-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/api.py

```diff
@@ -1,14 +1,12 @@
-from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form, Request, HTTPException
-from flask import request, jsonify
+from fastapi import FastAPI, WebSocket, Request, Request, HTTPException
 from pydantic import BaseModel
 from llama_index.llms.llama_cpp import LlamaCPP
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
-import asyncio
 import os
 import json
 from fastapi.middleware.cors import CORSMiddleware
 import vertexai
 from vertexai.generative_models import GenerativeModel
 from openai import AzureOpenAI
 from fastapi.responses import JSONResponse
@@ -19,14 +17,15 @@
 import sqlite3
 import hashlib
 import re
 from datetime import datetime, timedelta
 import jwt
 
 
+
 SECRET="!az$y#5%"
 
 print("Secret key!!",SECRET)
 
 
 app = FastAPI()
 
@@ -398,17 +397,24 @@
                 print("Exiting chat.")
                 return
             if prompt.lower() == "exit":
                 print("Exiting chat.")
                 break
 
             agent = data['agent']
-            projectid=config["project_id"]
-            region=config["region"]
-            model=config["model"]
+            projectid=data["project_id"]
+            region=data["region"]
+            model=data["model"]
+
+            configuration = {
+                "project_id": projectid,
+                "region": region,
+                "model": model
+            }
+            save_vertex_config(configuration)
             vertexai.init(project=projectid, location=region)
             multimodal_model = GenerativeModel(model_name=model)
             if agent == "None":
                 response = multimodal_model.generate_content(prompt)
                 # await websocket.send_text(response.text)
                 # await websocket.close()
                 return JSONResponse(content={'response': response.text })
@@ -443,18 +449,27 @@
                     raise HTTPException(status_code=401, detail="You are not authorized to access this API")
             
             if prompt.lower() == "exit":
                 print("Exiting chat.")
                 break
 
             agent = data['agent']
-            key=config['apikey']
-            version=config['version']
-            model=config['modelInput']
-            endpoint=config['endpoint']
+            key=data['apikey']
+            version=data['version']
+            model=data['modelInput']
+            endpoint=data['endpoint']
+
+            configuration={
+                "key":key,
+                "version":version,
+                "model":model,
+                "endpoint":endpoint
+            }
+
+            save_azure_config(configuration)
 
 
             client = AzureOpenAI(
                 api_key = (key),
                 api_version = version,
                 azure_endpoint = (endpoint)
             )
```

## ALLMDEV/backend.py

```diff
@@ -1,10 +1,10 @@
-from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form, Request, HTTPException, Header
+from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form, Request, HTTPException, Header,WebSocketDisconnect
 from flask import request, jsonify
-from pydantic import BaseModel
+from pydantic import BaseModel, EmailStr
 from llama_index.llms.llama_cpp import LlamaCPP
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import asyncio
 import os
 import json
 from fastapi.middleware.cors import CORSMiddleware
@@ -17,14 +17,17 @@
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 import sqlite3
 import hashlib
 import re
 from datetime import datetime, timedelta
 import jwt
+import smtplib
+from email.mime.text import MIMEText
+from email.mime.multipart import MIMEMultipart
 
 SECRET="!az$y#5%"
 
 app = FastAPI()
 
 
 
@@ -38,14 +41,15 @@
 
 
 max_new_tokens = 512
 prompt_template = "<s>[INST] {prompt} [/INST]"
 config_path = "model/config.json"
 vertex_config_path = "model/vertex_config.json"
 azure_config_path = "model/azure_config.json"
+email_config_path = "model/email_config.json"
 
 class Message(BaseModel):
     userInput: str
     model: str
     temperature: float
 
 class Response(BaseModel):
@@ -87,24 +91,54 @@
     else:
         return {
             "apikey": "",
             "modelInput": "gemini-1.0-pro-002",
             "version": "",
             "endpoint": ""
         }
-
+def load_email_config():
+    if os.path.exists(email_config_path):
+        with open(email_config_path, "r") as f:
+            return json.load(f)
+    else:
+        return{
+            "smtp_server": "",
+            "smtp_port": "",
+            "smtp_username": "",
+            "smtp_password": "",
+            "sender_email": "",
+            "recipient_emails": "",
+            "user_creation" : "",
+            "user_deletion" : "",
+            "feedback" : "",
+            "password_change" : "",
+            "model_change" : "",
+            "feedback_email_subject": "Feedback received",
+            "password_change_email_subject": "Password changed",
+            "model_change_email_subject": "Model changed",
+            "user_creation_email_subject": "New user added to Database",
+            "user_deletion_email_subject": "User deleted from Database",
+            "user_creation_email_body": "Dear admin, \n A new user has been added to the database, kindly take a note of the same.",
+            "user_deletion_email_body": "Dear admin, \n A user has been deleted from the database, kindly take a note of the same.",
+            "feedback_email_body": "Dear admin, \n Feedback received for a response",
+            "password_change_email_body": "Your password has been changed",
+            "model_change_email_body": "The global model configuration has changed, kindly take a note of the same.",
+        }
 def save_config(config):
     with open(config_path, "w") as f:
         json.dump(config, f, indent=4)
 def save_azure_config(config):
     with open(azure_config_path, "w") as f:
         json.dump(config, f, indent=4)
 def save_vertex_config(config):
     with open(vertex_config_path, "w") as f:
         json.dump(config, f, indent=4)
+def save_emails_config(config):
+    with open(email_config_path, "w") as f:
+        json.dump(config, f, indent=4)
 
 # Database setup function
 def setup_database():
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
     cursor.execute('''
@@ -1026,14 +1060,62 @@
         conn.close()
     else:
         raise HTTPException(status_code=404, detail="Organization details not found")
     # except Exception as e:
         # raise HTTPException(status_code=500, detail="Database query failed: " + str(e))
     # finally:
 
+class SMTPParams(BaseModel):
+    smtp_server: str
+    smtp_port: int
+    smtp_username: str
+    smtp_password: str
+    sender_email: EmailStr
+    recipient_emails: list[EmailStr]
+    user_creation : bool
+    user_deletion : bool
+    feedback : bool
+    password_change : bool
+    model_change : bool
+
+@app.websocket("/send-email")
+async def websocket_endpoint(websocket: WebSocket):
+    await websocket.accept()
+    try:
+        while True:
+            data = await websocket.receive_text()
+            smtp_params = SMTPParams(**json.loads(data))
+            save_emails_config(smtp_params)
+
+            # Create a multipart message
+            msg = MIMEMultipart()
+            msg['From'] = smtp_params.sender_email
+            msg['To'] = ", ".join(smtp_params.recipient_emails)
+            msg['Subject'] = smtp_params.subject
+
+            # Attach the body with the msg instance
+            msg.attach(MIMEText(smtp_params.body, 'plain'))
+
+            try:
+                # Connect to the server
+                server = smtplib.SMTP(smtp_params.smtp_server, smtp_params.smtp_port)
+                server.starttls()  # Secure the connection
+                server.login(smtp_params.smtp_username, smtp_params.smtp_password)
+
+                # Send the email
+                server.sendmail(smtp_params.sender_email, smtp_params.recipient_emails, msg.as_string())
+                server.quit()
+
+                await websocket.send_text("Email sent successfully")
+            except Exception as e:
+                await websocket.send_text(f"Failed to send email: {str(e)}")
+    except WebSocketDisconnect:
+        print("Client disconnected")
+
+
 def main():
     import uvicorn
     setup_database()
     uvicorn.run(app, host="0.0.0.0", port=8000)
 
 if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV-1.3.9.dist-info/METADATA` & `ALLMDEV-1.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.9
+Version: 1.4.0
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
```

## Comparing `ALLMDEV-1.3.9.dist-info/entry_points.txt` & `ALLMDEV-1.4.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ALLMDEV-1.3.9.dist-info/RECORD` & `ALLMDEV-1.4.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
 ALLMDEV/agentapi.py,sha256=vnkpCaviW0w5EQTE99els4Nb8QABv0TgNoP2FdFsWVQ,3706
 ALLMDEV/agentchat.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
-ALLMDEV/api.py,sha256=B2wfma6owAZ8Fxy3fc4i63z4ZfvCJdDYCpkUAEq4_AM,34900
+ALLMDEV/api.py,sha256=DfU-EjYRpGHwAknSVCexYCW9f6lA3Kc_gWfbSKBTaFc,35243
 ALLMDEV/azureagentapi.py,sha256=dzMwkJHfRBqRxYAwpe_aQRgASqnsNBaEzT9jsc791QQ,4986
 ALLMDEV/azureagentchat.py,sha256=6L9m2B6dfe9LUWdd_Vj6_TT1n1GBXxVvqOeA-yTuV_Q,3298
 ALLMDEV/azurecli.py,sha256=nLoSVPpxWwIJWhiddB0_qzNw53hrAE6ijK0diDlaGYs,2435
-ALLMDEV/backend.py,sha256=L07ajpk3twXIHr-zyfPTOeWaldGdHj7Tfc5ig9Sbl7o,35338
+ALLMDEV/backend.py,sha256=oeEkCt8C6cQiovJ5LmUFtGRSB6s1B--ZSLai0l2U27w,38780
 ALLMDEV/chat_history.py,sha256=Et8kDK4RKdIr-v4CoYdvd5yb37GxTHpu4U1gHw5C2GY,4952
 ALLMDEV/cli.py,sha256=13o2i7g_DtOyP8N8x7QdMr8iUGr4raJX26NJ9oqpgNw,3221
+ALLMDEV/email_test.py,sha256=9HWnhQWZq4lBe1PmgGffcwMsyRIZT3OU3dRCK65e7CE,1314
 ALLMDEV/instruct.py,sha256=-3ybhrmAwgLy_MptpJHhFnbQq1NcT4DHeMV2-46Tzl8,12685
 ALLMDEV/newagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/serve.py,sha256=RUKwji_795izII7XlYku1KUK6bvgR_SYBB9N34GwqUA,2231
 ALLMDEV/studio.py,sha256=LlrIEWcs-o8cIjnprJVijR8cNxrOsnFvl9AgTrk43iw,1932
 ALLMDEV/test.py,sha256=CxP_WW9ZXEiLCJh_9MLdieFU-yfNMwWlXrcrs7gtXx8,683
 ALLMDEV/updateagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/vertexagentapi.py,sha256=fPbLJoy8Wirh7wPc31EzlgLSqfF2e4PkEwYCO9h4yqk,4530
 ALLMDEV/vertexagentchat.py,sha256=dYvJ2_teBGeEN3TTrXq4pSulYJW5kmNPKFa9xg9ec9s,2826
 ALLMDEV/vertexcli.py,sha256=-5BgOKO7oMsjcsJRluAM0ivWllzpBpWmVQIzHbq_Xrk,2126
-ALLMDEV-1.3.9.dist-info/METADATA,sha256=BcK-onZHO-rLxVDpvdieOTrrRZLK_JbTw0HElbCo9wQ,6145
-ALLMDEV-1.3.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.3.9.dist-info/entry_points.txt,sha256=pjURSzuC4nj_kFl775kwqXRV2icVzPLAt9uTPNSUwig,589
-ALLMDEV-1.3.9.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.3.9.dist-info/RECORD,,
+ALLMDEV-1.4.0.dist-info/METADATA,sha256=UU5SqA1ZfC7BZGLEvrUbmvbE_fCDaiZ7dsm5CFtuauQ,6145
+ALLMDEV-1.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.4.0.dist-info/entry_points.txt,sha256=pjURSzuC4nj_kFl775kwqXRV2icVzPLAt9uTPNSUwig,589
+ALLMDEV-1.4.0.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.4.0.dist-info/RECORD,,
```

