# Comparing `tmp/chatmemoryc-0.1.4rc1.tar.gz` & `tmp/chatmemoryc-0.1.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatmemoryc-0.1.4rc1.tar", last modified: Tue Apr 16 01:04:40 2024, max compression
+gzip compressed data, was "chatmemoryc-0.1.4rc2.tar", last modified: Sat Jun  1 00:55:36 2024, max compression
```

## Comparing `chatmemoryc-0.1.4rc1.tar` & `chatmemoryc-0.1.4rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:40.969101 chatmemoryc-0.1.4rc1/
--rw-rw-rw-   0        0        0    11324 2024-04-15 03:15:05.000000 chatmemoryc-0.1.4rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     8021 2024-04-16 01:04:40.968100 chatmemoryc-0.1.4rc1/PKG-INFO
--rw-rw-rw-   0        0        0     7392 2024-04-15 03:59:14.000000 chatmemoryc-0.1.4rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:40.949479 chatmemoryc-0.1.4rc1/chatmemoryc/
--rw-rw-rw-   0        0        0        0 2024-01-24 23:42:20.000000 chatmemoryc-0.1.4rc1/chatmemoryc/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-04-13 02:14:36.000000 chatmemoryc-0.1.4rc1/chatmemoryc/__main__.py
--rw-rw-rw-   0        0        0    14963 2024-04-10 05:54:33.000000 chatmemoryc-0.1.4rc1/chatmemoryc/chatmemoryc.py
--rw-rw-rw-   0        0        0     3279 2024-03-19 10:01:43.000000 chatmemoryc-0.1.4rc1/chatmemoryc/client.py
--rw-rw-rw-   0        0        0    12092 2024-04-09 07:27:57.000000 chatmemoryc-0.1.4rc1/chatmemoryc/server.py
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:40.967098 chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/
--rw-rw-rw-   0        0        0     8021 2024-04-16 01:04:40.000000 chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-16 01:04:40.000000 chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 01:04:40.000000 chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-16 01:04:40.000000 chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 01:04:40.000000 chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 01:04:40.969101 chatmemoryc-0.1.4rc1/setup.cfg
--rw-rw-rw-   0        0        0      753 2024-04-16 01:04:29.000000 chatmemoryc-0.1.4rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:55:36.819504 chatmemoryc-0.1.4rc2/
+-rw-rw-rw-   0        0        0    11324 2024-04-15 03:15:05.000000 chatmemoryc-0.1.4rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     8021 2024-06-01 00:55:36.819504 chatmemoryc-0.1.4rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     7392 2024-04-15 03:59:14.000000 chatmemoryc-0.1.4rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 00:55:36.803882 chatmemoryc-0.1.4rc2/chatmemoryc/
+-rw-rw-rw-   0        0        0        0 2024-01-24 23:42:20.000000 chatmemoryc-0.1.4rc2/chatmemoryc/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-04-16 02:40:33.000000 chatmemoryc-0.1.4rc2/chatmemoryc/__main__.py
+-rw-rw-rw-   0        0        0    15289 2024-06-01 00:49:29.000000 chatmemoryc-0.1.4rc2/chatmemoryc/chatmemoryc.py
+-rw-rw-rw-   0        0        0     3279 2024-03-19 10:01:43.000000 chatmemoryc-0.1.4rc2/chatmemoryc/client.py
+-rw-rw-rw-   0        0        0    12330 2024-06-01 00:48:06.000000 chatmemoryc-0.1.4rc2/chatmemoryc/server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:55:36.819504 chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/
+-rw-rw-rw-   0        0        0     8021 2024-06-01 00:55:36.000000 chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-06-01 00:55:36.000000 chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:55:36.000000 chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-06-01 00:55:36.000000 chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 00:55:36.000000 chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 00:55:36.819504 chatmemoryc-0.1.4rc2/setup.cfg
+-rw-rw-rw-   0        0        0      753 2024-06-01 00:42:00.000000 chatmemoryc-0.1.4rc2/setup.py
```

### Comparing `chatmemoryc-0.1.4rc1/LICENSE.txt` & `chatmemoryc-0.1.4rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc1/PKG-INFO` & `chatmemoryc-0.1.4rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: chatmemoryc
-Version: 0.1.4rc1
+Version: 0.1.4rc2
 Summary: Long-term and medium-term memories between you and chatbot
 Home-page: https://github.com/f6844710/chatmemoryc
 Author: pino
 Author-email: f6844710@nifty.com
 Maintainer: pino
 Maintainer-email: f6844710@nifty.com
 License: Apache v2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: fastapi==0.105.0
-Requires-Dist: anthropic==0.23.0
+Requires-Dist: fastapi==0.110.0
+Requires-Dist: anthropic==0.28.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: SQLAlchemy==2.0.20
-Requires-Dist: uvicorn==0.23.1
-Requires-Dist: pycryptodome==3.18.0
+Requires-Dist: SQLAlchemy==2.0.28
+Requires-Dist: uvicorn==0.28.1
+Requires-Dist: pycryptodome==3.20.0
 
 # chatmemory
 
 Long-term and medium-term memories between you and chatbot💕
 
 # 🚀 Quick start
```

### Comparing `chatmemoryc-0.1.4rc1/README.md` & `chatmemoryc-0.1.4rc2/README.md`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc1/chatmemoryc/__main__.py` & `chatmemoryc-0.1.4rc2/chatmemoryc/__main__.py`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc1/chatmemoryc/chatmemoryc.py` & `chatmemoryc-0.1.4rc2/chatmemoryc/chatmemoryc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,348 +1,348 @@
-import os
-from datetime import datetime, date, time, timedelta, timezone
-import base64
-import json
-import hashlib
-from logging import getLogger, NullHandler
-import traceback
-from sqlalchemy import Column, Integer, String, DateTime, Date
-from sqlalchemy.orm import Session, declarative_base
-from Crypto.Cipher import AES  # pycryptodome
-import anthropic
-
-logger = getLogger(__name__)
-logger.addHandler(NullHandler())
-
-# Models
-Base = declarative_base()
-
-
-class History(Base):
-    __tablename__ = "histories"
-
-    id = Column(Integer, primary_key=True, index=True)
-    timestamp = Column(DateTime, default=datetime.utcnow)
-    user_id = Column(String)
-    role = Column(String)
-    content = Column(String)
-
-
-class Archive(Base):
-    __tablename__ = "archives"
-
-    timestamp = Column(DateTime, default=datetime.utcnow)
-    user_id = Column(String, primary_key=True, index=True)
-    archive_date = Column(Date, primary_key=True, index=True)
-    archive = Column(String)
-
-
-class Entity(Base):
-    __tablename__ = "entities"
-
-    timestamp = Column(DateTime, default=datetime.utcnow)
-    user_id = Column(String, primary_key=True, index=True)
-    last_target_date = Column(Date, nullable=False)
-    serialized_entities = Column(String)
-
-
-# Archiver
-class HistoryArchiver:
-    PROMPT_EN = "Please summarize the content of the following conversation in the original language of the content(e.g. content in Japanese should be summarize in Japanese), in about {archive_length} words, paying attention to the topics discussed. Write the summary in third-person perspective, with 'user' and 'assistant' as the subjects.\n\n{histories_text}"
-    PROMPT_JA = "以下の会話の内容を、話題等に注目して{archive_length}文字以内程度の日本語で要約してください。要約した文章は第三者視点で、主語はuserとasssitantとします。\n\n{histories_text}"
-
-    def __init__(self, api_key: str, model: str = "claude-3-haiku-20240307", archive_length: int = 100,
-                 prompt: str = PROMPT_EN):
-        self.api_key = api_key
-        self.model = model
-        self.archive_length = archive_length
-        self.archive_prompt = prompt
-
-    def archive(self, messages: list):
-        histories_text = ""
-        for m in messages:
-            if m["role"] == "user" or m["role"] == "assistant":
-                histories_text += f'- {m["role"]}: {m["content"]}\n'
-
-        histories = [
-            {"role": "user",
-             "content": self.archive_prompt.format(archive_length=self.archive_length, histories_text=histories_text)}
-        ]
-
-        # prompt = self.archive_prompt.format(archive_length=self.archive_length, histories_text=histories_text)
-
-        # LLMに読み込ませるツールの定義
-        tools = [{
-            "name": "save_summarized_histories",
-            "description": "Summarize the content of the conversation.",
-            "input_schema": {
-                "type": "object",
-                "properties": {
-                    "summarized_text": {
-                        "type": "string",
-                        "description": "要約した会話の内容"
-                    },
-                },
-                "required": ["summarized_text"]
-            }
-        }, ]
-
-        client = anthropic.Anthropic(api_key=self.api_key)
-        resp = client.beta.tools.messages.create(
-            model=self.model,
-            messages=histories,
-            max_tokens=2000,
-            tools=tools
-        )
-        client.close()
-        # messages += [{"role": "user", "content": prompt}]
-
-        try:
-            return json.loads(str(resp.content[0].input).replace("\'", "\""))["summarized_text"]
-
-        except json.decoder.JSONDecodeError:
-            logger.warning(f"Retry parsing JSON: {resp}")
-            jstr = str(resp.content[0].input).replace("\'", "\"").replace("\",\n}", "\"\n}")
-            return json.loads(jstr)["summarized_text"]
-
-        except Exception as ex:
-            logger.error(f"Invalid response form Claude3 at archive: {resp}\n{ex}\n{traceback.format_exc()}")
-            raise ex
-
-
-class EntityExtractor:
-    PROMPT_EN = "From the conversation history, please extract any information that should be remembered about the user in original language. If there are already stored items, overwrite the new information with the same item key."
-    PROMPT_JA = "会話の履歴の中から、ユーザーに関して覚えておくべき情報があれば抽出してください。既に記憶している項目があれば、同じ項目名を使用して新しい情報で上書きします。"
-
-    def __init__(self, api_key: str, model: str = "claude-3-haiku-20240307", prompt: str = PROMPT_EN):
-        self.api_key = api_key
-        self.model = model
-        self.extract_prompt = prompt
-
-    def extract(self, messages: list, entities: dict = None):
-        histories = [m for m in messages if m["role"] == "user" or m["role"] == "assistant"]
-
-        prompt = self.extract_prompt
-        if entities:
-            prompt = self.extract_prompt + "\n\nEntities that you already know:\n"
-            for k, v in entities.items():
-                prompt += f"- {k}: {v}\n"
-
-        histories.append({"role": "user", "content": prompt})
-
-        # LLMに読み込ませるツールの定義
-        tools2 = [{"name": "save_entities",
-                   "description": "Extract and save any information that should be remembered about the user.",
-                   "input_schema": {
-                       "type": "object",
-                       "properties": {
-                           "entities": {
-                               "type": "array",
-                               "items": {
-                                   "type": "object",
-                                   "properties": {
-                                       "name": {"type": "string",
-                                                "description": "name of entity. use snake case. 'examples: [birthday_date]"},
-                                       "value": {"type": "string"},
-                                   }
-                               }
-                           }
-                       }, "required": ["entities"]
-                   }
-                }
-            ]
-
-        # prompt += "\nPlease provide the extracted entities in the following JSON format:\n```json\n{\n  \"entities\": [\n    {\"name\": \"entity_name\", \"value\": \"entity_value\"},\n    ...\n  ]\n}\n```"
-
-        client = anthropic.Anthropic(api_key=self.api_key)
-        resp = client.beta.tools.messages.create(
-            model=self.model,
-            messages=histories,
-            max_tokens=2000,
-            tools=tools2
-        )
-        client.close()
-        # messages += [{"role": "user", "content": prompt}]
-        try:
-            return {
-                e["name"]: e["value"] for e
-                in json.loads(
-                    str(resp.content[0].input).replace("\'", "\"")
-                ).get("entities") or []
-            }
-
-        except json.decoder.JSONDecodeError:
-            logger.warning(f"Retry parsing JSON: {resp}")
-            jstr = str(resp.content[0].input).replace("\'", "\"").replace("\",\n}", "\"\n}")
-            return {
-                e["name"]: e["value"] for e in json.loads(jstr).get("entities") or []
-            }
-
-        except Exception as ex:
-            logger.error(f"Invalid response form Claude3 at extract: {resp}\n{ex}\n{traceback.format_exc()}")
-            raise ex
-
-
-# Memory manager
-class ChatMemory:
-    def __init__(self, api_key: str = None, model: str = "claude-3-haiku-20240307",
-                 history_archiver: HistoryArchiver = None,
-                 entity_extractor: EntityExtractor = None):
-        self.history_archiver = history_archiver or HistoryArchiver(api_key, model)
-        self.entity_extractor = entity_extractor or EntityExtractor(api_key, model)
-        self.history_max_count = 100
-        self.archive_retrive_count = 5
-
-    def date_to_utc_datetime(self, d) -> datetime:
-        return datetime.combine(d, time()).replace(tzinfo=timezone.utc)
-
-    def encrypt(self, text: str, password: str = None):
-        if not password:
-            return text
-
-        salt = os.urandom(16)
-        key = hashlib.scrypt(password=password.encode("utf-8"), salt=salt, n=2 ** 5, r=8, p=1, dklen=32)
-        cipher = AES.new(key, AES.MODE_GCM)
-        cipher_text, tag = cipher.encrypt_and_digest(text.encode("utf-8"))
-        return "-".join([base64.b64encode(item).decode("utf-8") for item in [salt, cipher.nonce, cipher_text, tag]])
-
-    def decrypt(self, encrypted_text: str, password: str = None):
-        if not password:
-            return encrypted_text
-
-        salt, cipher_nonce, cipher_text, tag = [base64.b64decode(item) for item in encrypted_text.split("-")]
-        key = hashlib.scrypt(password=password.encode("utf-8"), salt=salt, n=2 ** 5, r=8, p=1, dklen=32)
-        cipher = AES.new(key, AES.MODE_GCM, cipher_nonce)
-        return cipher.decrypt_and_verify(cipher_text, tag).decode("utf-8")
-
-    def create_database(self, engine):
-        Base.metadata.create_all(bind=engine)
-
-    def add_histories(self, session: Session, user_id: str, messages: list, password: str = None):
-        histories = [
-            History(user_id=user_id, role=m["role"], content=self.encrypt(m["content"], password))
-            for m in messages if m["role"] == "user" or m["role"] == "assistant"
-        ]
-        session.bulk_save_objects(histories)
-
-    def get_histories(self, session: Session, user_id: str, since: datetime = None, until: datetime = None,
-                      password: str = None) -> list:
-        histories = session.query(History).filter(
-            History.user_id == user_id,
-            History.timestamp >= (since or datetime.min),
-            History.timestamp <= (until or datetime.max)
-        ).order_by(History.id).limit(self.history_max_count).all()
-
-        return [{"role": h.role, "content": self.decrypt(h.content, password)} for h in histories]
-
-    def delete_histories(self, session: Session, user_id: str):
-        session.query(History).filter(History.user_id == user_id).delete()
-
-    def archive_histories(self, session: Session, user_id: str, target_date: date, password: str = None):
-        since_dt = self.date_to_utc_datetime(target_date)
-        conversation_history = self.get_histories(
-            session,
-            user_id,
-            since_dt,
-            since_dt + timedelta(days=1),
-            password
-        )
-
-        if len(conversation_history) == 0:
-            logger.info(f"No histories found on {target_date} to archive")
-            return
-
-        # Get stored archive
-        stored_archive = session.query(Archive).filter(
-            Archive.user_id == user_id,
-            Archive.archive_date == target_date
-        ).first() or Archive(
-            user_id=user_id,
-            timestamp=datetime.min,
-            archive_date=target_date
-        )
-
-        # Skip if already archived
-        if stored_archive:
-            if stored_archive.timestamp.date() > target_date:
-                logger.info(f"Histories on {target_date} are already archived")
-                return
-
-        summarized_archive = self.history_archiver.archive(conversation_history)
-
-        stored_archive.timestamp = datetime.utcnow()
-        stored_archive.archive = self.encrypt(summarized_archive, password)
-
-        session.merge(stored_archive)
-
-    def get_archives(self, session: Session, user_id: str, since: date = None, until: date = None,
-                     password: str = None) -> list:
-        archives = session.query(Archive.archive_date, Archive.archive).filter(
-            Archive.user_id == user_id,
-            Archive.archive_date >= (since or date.min),
-            Archive.archive_date <= (until or date.max)
-        ).order_by(Archive.archive_date.desc()).limit(self.archive_retrive_count).all()
-
-        return [{"date": a.archive_date, "archive": self.decrypt(a.archive, password)} for a in archives]
-
-    def delete_archives(self, session: Session, user_id: str):
-        session.query(Archive).filter(Archive.user_id == user_id).delete()
-
-    def extract_entities(self, session: Session, user_id: str, target_date: date, password: str = None):
-        # Get histories on target_date
-        since_dt = self.date_to_utc_datetime(target_date)
-        until_dt = since_dt + timedelta(days=1)
-        conversation_history = self.get_histories(session, user_id, since_dt, until_dt, password)
-        if len(conversation_history) == 0:
-            logger.info(f"No histories found on {target_date} for extracting entities")
-            return
-
-        # Get stored entities or new entities
-        stored_entites = session.query(Entity).filter(
-            Entity.user_id == user_id,
-        ).first() or Entity(user_id=user_id, last_target_date=date.min)
-
-        # Skip extraction if already extracted (larger than target_date because some histories on last_target_date may be not processed)
-        if stored_entites.last_target_date > target_date:
-            logger.info(f"Entities in histories on {target_date} are already extracted")
-            return
-
-        if stored_entites.serialized_entities:
-            entities_json = json.loads(self.decrypt(stored_entites.serialized_entities, password))
-        else:
-            entities_json = {}
-
-        new_entities = self.entity_extractor.extract(conversation_history, entities_json)
-        for k, v in new_entities.items():
-            entities_json[k] = v
-
-        now = datetime.utcnow()
-        self.save_entities(session, user_id, now, now.date(), entities_json, password)
-
-    def save_entities(self, session: Session, user_id: str, timestamp: datetime, last_target_date: date, entities: dict,
-                      password: str = None):
-        new_entities = Entity(
-            user_id=user_id,
-            timestamp=timestamp,
-            serialized_entities=self.encrypt(json.dumps(entities, ensure_ascii=False), password),
-            last_target_date=last_target_date if entities else date.min
-        )
-
-        session.merge(new_entities)
-
-    def get_entities(self, session: Session, user_id: str, password: str = None) -> dict:
-        entities = session.query(Entity).filter(
-            Entity.user_id == user_id,
-        ).first()
-
-        if entities and entities.serialized_entities:
-            return json.loads(self.decrypt(entities.serialized_entities, password))
-        else:
-            return {}
-
-    def delete_entities(self, session: Session, user_id: str):
-        session.query(Entity).filter(Entity.user_id == user_id).delete()
-
-    def delete_all(self, session: Session, user_id: str):
-        session.query(History).filter(History.user_id == user_id).delete()
-        session.query(Archive).filter(Archive.user_id == user_id).delete()
-        session.query(Entity).filter(Entity.user_id == user_id).delete()
+import os
+from datetime import datetime, date, time, timedelta, timezone
+import base64
+import json
+import hashlib
+from logging import getLogger, NullHandler
+import traceback
+from sqlalchemy import Column, Integer, String, DateTime, Date
+from sqlalchemy.orm import Session, declarative_base
+from Crypto.Cipher import AES  # pycryptodome
+import anthropic
+
+logger = getLogger(__name__)
+logger.addHandler(NullHandler())
+
+# Models
+Base = declarative_base()
+
+
+class History(Base):
+    __tablename__ = "histories"
+
+    id = Column(Integer, primary_key=True, index=True)
+    timestamp = Column(DateTime, default=datetime.utcnow)
+    user_id = Column(String)
+    role = Column(String)
+    content = Column(String)
+
+
+class Archive(Base):
+    __tablename__ = "archives"
+
+    timestamp = Column(DateTime, default=datetime.utcnow)
+    user_id = Column(String, primary_key=True, index=True)
+    archive_date = Column(Date, primary_key=True, index=True)
+    archive = Column(String)
+
+
+class Entity(Base):
+    __tablename__ = "entities"
+
+    timestamp = Column(DateTime, default=datetime.utcnow)
+    user_id = Column(String, primary_key=True, index=True)
+    last_target_date = Column(Date, nullable=False)
+    serialized_entities = Column(String)
+
+
+# Archiver
+class HistoryArchiver:
+    PROMPT_EN = "Please summarize the content of the following conversation in the original language of the content(e.g. content in Japanese should be summarize in Japanese), in about {archive_length} words, paying attention to the topics discussed. Write the summary in third-person perspective, with 'user' and 'assistant' as the subjects.\n\n{histories_text}"
+    PROMPT_JA = "以下の会話の内容を、話題等に注目して{archive_length}文字以内程度の日本語で要約してください。要約した文章は第三者視点で、主語はuserとasssitantとします。\n\n{histories_text}"
+
+    def __init__(self, api_key: str, model: str = "claude-3-haiku-20240307", archive_length: int = 100,
+                 prompt: str = PROMPT_EN):
+        self.api_key = api_key
+        self.model = model
+        self.archive_length = archive_length
+        self.archive_prompt = prompt
+
+    def archive(self, messages: list):
+        histories_text = ""
+        for m in messages:
+            if m["role"] == "user" or m["role"] == "assistant":
+                histories_text += f'- {m["role"]}: {m["content"]}\n'
+
+        histories = [
+            {"role": "user",
+             "content": self.archive_prompt.format(archive_length=self.archive_length, histories_text=histories_text)}
+        ]
+
+        # prompt = self.archive_prompt.format(archive_length=self.archive_length, histories_text=histories_text)
+
+        # LLMに読み込ませるツールの定義
+        tools = [{
+            "name": "save_summarized_histories",
+            "description": "Summarize the content of the conversation.",
+            "input_schema": {
+                "type": "object",
+                "properties": {
+                    "summarized_text": {
+                        "type": "string",
+                        "description": "要約した会話の内容"
+                    },
+                },
+                "required": ["summarized_text"]
+            }
+        }, ]
+
+        client = anthropic.Anthropic(api_key=self.api_key)
+        resp = client.messages.create(
+            model=self.model,
+            messages=histories,
+            max_tokens=2000,
+            tools=tools
+        )
+        client.close()
+        # messages += [{"role": "user", "content": prompt}]
+
+        try:
+            return json.loads(str(resp.content[0].input).replace("\'", "\""))["summarized_text"]
+
+        except json.decoder.JSONDecodeError:
+            logger.warning(f"Retry parsing JSON: {resp}")
+            jstr = str(resp.content[0].input).replace("\'", "\"").replace("\",\n}", "\"\n}")
+            return json.loads(jstr)["summarized_text"]
+
+        except Exception as ex:
+            logger.error(f"Invalid response form Claude3 at archive: {resp}\n{ex}\n{traceback.format_exc()}")
+            raise ex
+
+
+class EntityExtractor:
+    PROMPT_EN = "From the conversation history, please extract any information that should be remembered about the user in original language. If there are already stored items, overwrite the new information with the same item key."
+    PROMPT_JA = "会話の履歴の中から、ユーザーに関して覚えておくべき情報があれば抽出してください。既に記憶している項目があれば、同じ項目名を使用して新しい情報で上書きします。"
+
+    def __init__(self, api_key: str, model: str = "claude-3-haiku-20240307", prompt: str = PROMPT_EN):
+        self.api_key = api_key
+        self.model = model
+        self.extract_prompt = prompt
+
+    def extract(self, messages: list, entities: dict = None):
+        histories = [m for m in messages if m["role"] == "user" or m["role"] == "assistant"]
+
+        prompt = self.extract_prompt
+        if entities:
+            prompt = self.extract_prompt + "\n\nEntities that you already know:\n"
+            for k, v in entities.items():
+                prompt += f"- {k}: {v}\n"
+
+        histories.append({"role": "user", "content": prompt})
+
+        # LLMに読み込ませるツールの定義
+        tools2 = [{"name": "save_entities",
+                   "description": "Extract and save any information that should be remembered about the user.",
+                   "input_schema": {
+                       "type": "object",
+                       "properties": {
+                           "entities": {
+                               "type": "array",
+                               "items": {
+                                   "type": "object",
+                                   "properties": {
+                                       "name": {"type": "string",
+                                                "description": "name of entity. use snake case. 'examples: [birthday_date]"},
+                                       "value": {"type": "string"},
+                                   }
+                               }
+                           }
+                       }, "required": ["entities"]
+                   }
+                }
+            ]
+
+        # prompt += "\nPlease provide the extracted entities in the following JSON format:\n```json\n{\n  \"entities\": [\n    {\"name\": \"entity_name\", \"value\": \"entity_value\"},\n    ...\n  ]\n}\n```"
+
+        client = anthropic.Anthropic(api_key=self.api_key)
+        resp = client.messages.create(
+            model=self.model,
+            messages=histories,
+            max_tokens=2000,
+            tools=tools2
+        )
+        client.close()
+        # messages += [{"role": "user", "content": prompt}]
+        try:
+            return {
+                e["name"]: e["value"] for e
+                in json.loads(
+                    str(resp.content[0].input).replace("\'", "\"")
+                ).get("entities") or []
+            }
+
+        except json.decoder.JSONDecodeError:
+            logger.warning(f"Retry parsing JSON: {resp}")
+            jstr = str(resp.content[0].input).replace("\'", "\"").replace("\",\n}", "\"\n}")
+            return {
+                e["name"]: e["value"] for e in json.loads(jstr).get("entities") or []
+            }
+
+        except Exception as ex:
+            logger.error(f"Invalid response form Claude3 at extract: {resp}\n{ex}\n{traceback.format_exc()}")
+            raise ex
+
+
+# Memory manager
+class ChatMemory:
+    def __init__(self, api_key: str = None, model: str = "claude-3-haiku-20240307",
+                 history_archiver: HistoryArchiver = None,
+                 entity_extractor: EntityExtractor = None):
+        self.history_archiver = history_archiver or HistoryArchiver(api_key, model)
+        self.entity_extractor = entity_extractor or EntityExtractor(api_key, model)
+        self.history_max_count = 100
+        self.archive_retrive_count = 5
+
+    def date_to_utc_datetime(self, d) -> datetime:
+        return datetime.combine(d, time()).replace(tzinfo=timezone.utc)
+
+    def encrypt(self, text: str, password: str = None):
+        if not password:
+            return text
+
+        salt = os.urandom(16)
+        key = hashlib.scrypt(password=password.encode("utf-8"), salt=salt, n=2 ** 5, r=8, p=1, dklen=32)
+        cipher = AES.new(key, AES.MODE_GCM)
+        cipher_text, tag = cipher.encrypt_and_digest(text.encode("utf-8"))
+        return "-".join([base64.b64encode(item).decode("utf-8") for item in [salt, cipher.nonce, cipher_text, tag]])
+
+    def decrypt(self, encrypted_text: str, password: str = None):
+        if not password:
+            return encrypted_text
+
+        salt, cipher_nonce, cipher_text, tag = [base64.b64decode(item) for item in encrypted_text.split("-")]
+        key = hashlib.scrypt(password=password.encode("utf-8"), salt=salt, n=2 ** 5, r=8, p=1, dklen=32)
+        cipher = AES.new(key, AES.MODE_GCM, cipher_nonce)
+        return cipher.decrypt_and_verify(cipher_text, tag).decode("utf-8")
+
+    def create_database(self, engine):
+        Base.metadata.create_all(bind=engine)
+
+    def add_histories(self, session: Session, user_id: str, messages: list, password: str = None):
+        histories = [
+            History(user_id=user_id, role=m["role"], content=self.encrypt(m["content"], password))
+            for m in messages if m["role"] == "user" or m["role"] == "assistant"
+        ]
+        session.bulk_save_objects(histories)
+
+    def get_histories(self, session: Session, user_id: str, since: datetime = None, until: datetime = None,
+                      password: str = None) -> list:
+        histories = session.query(History).filter(
+            History.user_id == user_id,
+            History.timestamp >= (since or datetime.min),
+            History.timestamp <= (until or datetime.max)
+        ).order_by(History.id).limit(self.history_max_count).all()
+
+        return [{"role": h.role, "content": self.decrypt(h.content, password)} for h in histories]
+
+    def delete_histories(self, session: Session, user_id: str):
+        session.query(History).filter(History.user_id == user_id).delete()
+
+    def archive_histories(self, session: Session, user_id: str, target_date: date, password: str = None):
+        since_dt = self.date_to_utc_datetime(target_date)
+        conversation_history = self.get_histories(
+            session,
+            user_id,
+            since_dt,
+            since_dt + timedelta(days=1),
+            password
+        )
+
+        if len(conversation_history) == 0:
+            logger.info(f"No histories found on {target_date} to archive")
+            return
+
+        # Get stored archive
+        stored_archive = session.query(Archive).filter(
+            Archive.user_id == user_id,
+            Archive.archive_date == target_date
+        ).first() or Archive(
+            user_id=user_id,
+            timestamp=datetime.min,
+            archive_date=target_date
+        )
+
+        # Skip if already archived
+        if stored_archive:
+            if stored_archive.timestamp.date() > target_date:
+                logger.info(f"Histories on {target_date} are already archived")
+                return
+
+        summarized_archive = self.history_archiver.archive(conversation_history)
+
+        stored_archive.timestamp = datetime.utcnow()
+        stored_archive.archive = self.encrypt(summarized_archive, password)
+
+        session.merge(stored_archive)
+
+    def get_archives(self, session: Session, user_id: str, since: date = None, until: date = None,
+                     password: str = None) -> list:
+        archives = session.query(Archive.archive_date, Archive.archive).filter(
+            Archive.user_id == user_id,
+            Archive.archive_date >= (since or date.min),
+            Archive.archive_date <= (until or date.max)
+        ).order_by(Archive.archive_date.desc()).limit(self.archive_retrive_count).all()
+
+        return [{"date": a.archive_date, "archive": self.decrypt(a.archive, password)} for a in archives]
+
+    def delete_archives(self, session: Session, user_id: str):
+        session.query(Archive).filter(Archive.user_id == user_id).delete()
+
+    def extract_entities(self, session: Session, user_id: str, target_date: date, password: str = None):
+        # Get histories on target_date
+        since_dt = self.date_to_utc_datetime(target_date)
+        until_dt = since_dt + timedelta(days=1)
+        conversation_history = self.get_histories(session, user_id, since_dt, until_dt, password)
+        if len(conversation_history) == 0:
+            logger.info(f"No histories found on {target_date} for extracting entities")
+            return
+
+        # Get stored entities or new entities
+        stored_entites = session.query(Entity).filter(
+            Entity.user_id == user_id,
+        ).first() or Entity(user_id=user_id, last_target_date=date.min)
+
+        # Skip extraction if already extracted (larger than target_date because some histories on last_target_date may be not processed)
+        if stored_entites.last_target_date > target_date:
+            logger.info(f"Entities in histories on {target_date} are already extracted")
+            return
+
+        if stored_entites.serialized_entities:
+            entities_json = json.loads(self.decrypt(stored_entites.serialized_entities, password))
+        else:
+            entities_json = {}
+
+        new_entities = self.entity_extractor.extract(conversation_history, entities_json)
+        for k, v in new_entities.items():
+            entities_json[k] = v
+
+        now = datetime.utcnow()
+        self.save_entities(session, user_id, now, now.date(), entities_json, password)
+
+    def save_entities(self, session: Session, user_id: str, timestamp: datetime, last_target_date: date, entities: dict,
+                      password: str = None):
+        new_entities = Entity(
+            user_id=user_id,
+            timestamp=timestamp,
+            serialized_entities=self.encrypt(json.dumps(entities, ensure_ascii=False), password),
+            last_target_date=last_target_date if entities else date.min
+        )
+
+        session.merge(new_entities)
+
+    def get_entities(self, session: Session, user_id: str, password: str = None) -> dict:
+        entities = session.query(Entity).filter(
+            Entity.user_id == user_id,
+        ).first()
+
+        if entities and entities.serialized_entities:
+            return json.loads(self.decrypt(entities.serialized_entities, password))
+        else:
+            return {}
+
+    def delete_entities(self, session: Session, user_id: str):
+        session.query(Entity).filter(Entity.user_id == user_id).delete()
+
+    def delete_all(self, session: Session, user_id: str):
+        session.query(History).filter(History.user_id == user_id).delete()
+        session.query(Archive).filter(Archive.user_id == user_id).delete()
+        session.query(Entity).filter(Entity.user_id == user_id).delete()
```

### Comparing `chatmemoryc-0.1.4rc1/chatmemoryc/client.py` & `chatmemoryc-0.1.4rc2/chatmemoryc/client.py`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc1/chatmemoryc/server.py` & `chatmemoryc-0.1.4rc2/chatmemoryc/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-from datetime import datetime, timedelta
-from fastapi import FastAPI, Depends, Header
-from fastapi.responses import JSONResponse
-from logging import getLogger
-from pydantic import BaseModel, Field
-import traceback
-from typing import List, Dict, Optional
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker, Session
-import uvicorn
-from .chatmemoryc import ChatMemory
-
-logger = getLogger(__name__)
-# logger
-
-class Message(BaseModel):
-    role: str = Field(..., title="role", description="The role of the author of this message.", example="user")
-    content: Optional[str] = Field(None, title="content", description="The contents of the message.", example="Hello!")
-
-
-class HistoriesRequest(BaseModel):
-    messages: List[Message] = Field(..., title="messages", description="A list of messages to store comprising the conversation so far.", example=[{"role": "user", "content": "Hello"}, {"role": "assistant", "content": "Hi there!"}])
-
-
-class HistoriesResponse(BaseModel):
-    messages: List[Message] = Field(..., title="messages", description="A list of retrieved messages comprising the conversation so far.", example=[{"role": "user", "content": "Hello"}, {"role": "assistant", "content": "Hi there!"}])
-
-class ArchivesRequest(BaseModel):
-    target_date: Optional[str] = Field(None, title="target_date", description="Target date in ISO8601 format for creating the summary of conversation.", example="2023-08-11")
-    days: int = Field(1, title="days", description="The number of days to go back in the conversation history for creating an archive.", example=1)
-
-
-class Archive(BaseModel):
-    date: str = Field(..., title="date", description="Date in ISO8601 format", example="2023-08-11")
-    archive: str = Field(..., title="archive", description="Summarized text of the conversation on the date.", example="user")
-
-
-class ArchivesResponse(BaseModel):
-    archives: List[Archive] = Field(..., title="archives", description="A list of summarized conversation texts.", example=[{"date": "2023-08-11", "archive": "User and assistant talk about lunch and user says that soba is nice."}, {"date": "2023-08-10", "archive": "User says she loves cats."}])
-
-
-class EntitiesRequest(BaseModel):
-    target_date: Optional[str] = Field(None, title="target_date", description="Target date in ISO8601 format to extract entities.", example="2023-08-11")
-    days: int = Field(1, title="days", description="The number of days to go back in the conversation history to extract entities.", example=1)
-    entities: Optional[Dict[str, object]] = Field(None, title="entities", description="Entities to store. All existing entities are replaced with this.", example={"nickname": "uezo", "age": 28, "favorite_food": "soba"})
-
-
-class EntitiesResponse(BaseModel):
-    entities: Dict[str, object] = Field(..., title="entities", description="Stored entities.", example={"nickname": "uezo", "age": 28, "favorite_food": "soba"})
-
-
-class ApiResponse(BaseModel):
-    message: str = Field(..., title="message", description="Message from API", example="Entities extracted and stored successfully")
-
-
-class ChatMemoryServer:
-    def __init__(self, api_key: str, database_url: str="sqlite:///chatmemoryc.db", server_args: dict=None):
-        self.database_url = database_url
-        self.engine = create_engine(self.database_url)
-        self.session_local = sessionmaker(autocommit=False, autoflush=False, bind=self.engine)
-
-        self.anthropic_apikey = api_key
-        self.chatmemoryc = ChatMemory(api_key=self.anthropic_apikey)
-        self.chatmemoryc.create_database(self.engine)
-
-        self.app = FastAPI(**(server_args or {"title": "ChatMemoryc", "version": "0.1.4"}))
-        self.setup_handlers()
-
-    def get_db(self):
-        db = self.session_local()
-        try:
-            yield db
-        finally:
-            db.close()
-
-    def setup_handlers(self):
-        app = self.app
-
-        @app.post("/histories/{user_id}", response_model=ApiResponse, tags=["History"])
-        async def add_histories(user_id: str, request: HistoriesRequest, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
-            try:
-                self.chatmemoryc.add_histories(
-                    db, user_id,
-                    [{"role": m.role, "content": m.content} for m in request.messages],
-                    encryption_key
-                )
-                db.commit()
-                return ApiResponse(message="Histories added successfully")
-            
-            except Exception as ex:
-                logger.error(f"Error at add_histories: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-        @app.get("/histories/{user_id}", response_model=HistoriesResponse, tags=["History"])
-        async def get_histories(user_id: str, since: str=None, until: str=None, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
-            try:
-                histories = self.chatmemoryc.get_histories(
-                    db, user_id,
-                    datetime.strptime(since, "%Y-%m-%d") if since else None,
-                    datetime.strptime(until, "%Y-%m-%d") if until else None,
-                    encryption_key
-                )
-                return HistoriesResponse(messages=[
-                    Message(role=h["role"], content=h["content"])
-                    for h in histories
-                ])
-
-            except ValueError as verr:
-                return JSONResponse("Invalid encryption key", 400)
-
-            except Exception as ex:
-                logger.error(f"Error at get_histories: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-
-        @app.delete("/histories/{user_id}", response_model=ApiResponse, tags=["History"])
-        async def delete_histories(user_id: str, db: Session = Depends(self.get_db)):
-            try:
-                self.chatmemoryc.delete_histories(db, user_id)
-                db.commit()
-                return ApiResponse(message="All histories are deleted successfully")
-
-            except Exception as ex:
-                logger.error(f"Error at delete_histories: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-        @app.post("/archives/{user_id}", response_model=ApiResponse, tags=["Archive"])
-        async def archive_histories(user_id: str, request: ArchivesRequest, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
-            try:
-                for i in range(request.days):
-                    self.chatmemoryc.archive_histories(
-                        db, user_id,
-                        (datetime.strptime(request.target_date, "%Y-%m-%d") if request.target_date
-                         else datetime.utcnow()).date() - timedelta(days=request.days - i - 1),
-                        encryption_key
-                    )
-                    db.commit()
-                return ApiResponse(message="Histories archived successfully")
-
-            except Exception as ex:
-                logger.error(f"Error at archive_histories: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-        @app.get("/archives/{user_id}", response_model=ArchivesResponse, tags=["Archive"])
-        async def get_archives(user_id: str, since: str=None, until: str=None, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
-            try:
-                archives = self.chatmemoryc.get_archives(
-                    db, user_id,
-                    datetime.strptime(since, "%Y-%m-%d") if since else None,
-                    datetime.strptime(until, "%Y-%m-%d") if until else None,
-                    encryption_key
-                )
-                return ArchivesResponse(archives=[
-                    Archive(date=a["date"].strftime("%Y-%m-%d"), archive=a["archive"])
-                    for a in archives
-                ])
-
-            except ValueError as verr:
-                return JSONResponse("Invalid encryption key", 400)
-
-            except Exception as ex:
-                logger.error(f"Error at get_archives: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-
-        @app.delete("/archives/{user_id}", response_model=ApiResponse, tags=["Archive"])
-        async def delete_archives(user_id: str, db: Session = Depends(self.get_db)):
-            try:
-                self.chatmemoryc.delete_archives(db, user_id)
-                db.commit()
-                return ApiResponse(message="All archives are deleted successfully")
-
-            except Exception as ex:
-                logger.error(f"Error at delete_archives: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-        @app.post("/entities/{user_id}", response_model=ApiResponse, tags=["Entity"])
-        async def save_entities(user_id: str, request: EntitiesRequest, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
-            try:
-                now = datetime.utcnow()
-                if request.entities is None:
-                    for i in range(request.days):
-                        self.chatmemoryc.extract_entities(
-                            db, user_id,
-                            (datetime.strptime(request.target_date, "%Y-%m-%d") if request.target_date
-                            else now).date() - timedelta(days=request.days - i - 1),
-                            encryption_key
-                        )
-                        db.commit()
-                    return ApiResponse(message="Entities extracted and stored successfully")
-            
-                else:
-                    self.chatmemoryc.save_entities(db, user_id, now, now.date(), request.entities, encryption_key)
-                    db.commit()
-                    return ApiResponse(message="Entities stored successfully")
-
-            except Exception as ex:
-                logger.error(f"Error at save_entities: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-
-        @app.get("/entities/{user_id}", response_model=EntitiesResponse, tags=["Entity"])
-        async def get_entities(user_id: str, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
-            try:
-                entities = self.chatmemoryc.get_entities(db, user_id, encryption_key)
-                return EntitiesResponse(entities=entities)
-
-            except ValueError as verr:
-                return JSONResponse("Invalid encryption key", 400)
-
-            except Exception as ex:
-                logger.error(f"Error at get_entities: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-        @app.delete("/entities/{user_id}", response_model=ApiResponse, tags=["Entity"])
-        async def delete_entities(user_id: str, db: Session = Depends(self.get_db)):
-            try:
-                self.chatmemoryc.delete_entities(db, user_id)
-                db.commit()
-                return ApiResponse(message="All entities are deleted successfully")
-
-            except Exception as ex:
-                logger.error(f"Error at delete_entities: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-        @app.delete("/all/{user_id}", response_model=ApiResponse, tags=["All"])
-        async def delete_all(user_id: str, db: Session = Depends(self.get_db)):
-            try:
-                self.chatmemoryc.delete_all(db, user_id)
-                db.commit()
-                return ApiResponse(message=f"Delete all data for {user_id} successfully")
-
-            except Exception as ex:
-                logger.error(f"Error at delete_all: {ex}\n{traceback.format_exc()}")
-                return JSONResponse("Internal server error", 500)
-
-
-    def start(self, host :str="127.0.0.1", port: int=8124):
-        uvicorn.run(self.app, host=host, port=port)
+from datetime import datetime, timedelta
+from fastapi import FastAPI, Depends, Header
+from fastapi.responses import JSONResponse
+from logging import getLogger
+from pydantic import BaseModel, Field
+import traceback
+from typing import List, Dict, Optional
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker, Session
+import uvicorn
+from chatmemoryc import ChatMemory
+
+logger = getLogger(__name__)
+# logger
+
+class Message(BaseModel):
+    role: str = Field(..., title="role", description="The role of the author of this message.", example="user")
+    content: Optional[str] = Field(None, title="content", description="The contents of the message.", example="Hello!")
+
+
+class HistoriesRequest(BaseModel):
+    messages: List[Message] = Field(..., title="messages", description="A list of messages to store comprising the conversation so far.", example=[{"role": "user", "content": "Hello"}, {"role": "assistant", "content": "Hi there!"}])
+
+
+class HistoriesResponse(BaseModel):
+    messages: List[Message] = Field(..., title="messages", description="A list of retrieved messages comprising the conversation so far.", example=[{"role": "user", "content": "Hello"}, {"role": "assistant", "content": "Hi there!"}])
+
+class ArchivesRequest(BaseModel):
+    target_date: Optional[str] = Field(None, title="target_date", description="Target date in ISO8601 format for creating the summary of conversation.", example="2023-08-11")
+    days: int = Field(1, title="days", description="The number of days to go back in the conversation history for creating an archive.", example=1)
+
+
+class Archive(BaseModel):
+    date: str = Field(..., title="date", description="Date in ISO8601 format", example="2023-08-11")
+    archive: str = Field(..., title="archive", description="Summarized text of the conversation on the date.", example="user")
+
+
+class ArchivesResponse(BaseModel):
+    archives: List[Archive] = Field(..., title="archives", description="A list of summarized conversation texts.", example=[{"date": "2023-08-11", "archive": "User and assistant talk about lunch and user says that soba is nice."}, {"date": "2023-08-10", "archive": "User says she loves cats."}])
+
+
+class EntitiesRequest(BaseModel):
+    target_date: Optional[str] = Field(None, title="target_date", description="Target date in ISO8601 format to extract entities.", example="2023-08-11")
+    days: int = Field(1, title="days", description="The number of days to go back in the conversation history to extract entities.", example=1)
+    entities: Optional[Dict[str, object]] = Field(None, title="entities", description="Entities to store. All existing entities are replaced with this.", example={"nickname": "uezo", "age": 28, "favorite_food": "soba"})
+
+
+class EntitiesResponse(BaseModel):
+    entities: Dict[str, object] = Field(..., title="entities", description="Stored entities.", example={"nickname": "uezo", "age": 28, "favorite_food": "soba"})
+
+
+class ApiResponse(BaseModel):
+    message: str = Field(..., title="message", description="Message from API", example="Entities extracted and stored successfully")
+
+
+class ChatMemoryServer:
+    def __init__(self, api_key: str, database_url: str="sqlite:///chatmemoryc.db", server_args: dict=None):
+        self.database_url = database_url
+        self.engine = create_engine(self.database_url)
+        self.session_local = sessionmaker(autocommit=False, autoflush=False, bind=self.engine)
+
+        self.anthropic_apikey = api_key
+        self.chatmemoryc = ChatMemory(api_key=self.anthropic_apikey)
+        self.chatmemoryc.create_database(self.engine)
+
+        self.app = FastAPI(**(server_args or {"title": "ChatMemoryc", "version": "0.1.4"}))
+        self.setup_handlers()
+
+    def get_db(self):
+        db = self.session_local()
+        try:
+            yield db
+        finally:
+            db.close()
+
+    def setup_handlers(self):
+        app = self.app
+
+        @app.post("/histories/{user_id}", response_model=ApiResponse, tags=["History"])
+        async def add_histories(user_id: str, request: HistoriesRequest, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
+            try:
+                self.chatmemoryc.add_histories(
+                    db, user_id,
+                    [{"role": m.role, "content": m.content} for m in request.messages],
+                    encryption_key
+                )
+                db.commit()
+                return ApiResponse(message="Histories added successfully")
+            
+            except Exception as ex:
+                logger.error(f"Error at add_histories: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+        @app.get("/histories/{user_id}", response_model=HistoriesResponse, tags=["History"])
+        async def get_histories(user_id: str, since: str=None, until: str=None, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
+            try:
+                histories = self.chatmemoryc.get_histories(
+                    db, user_id,
+                    datetime.strptime(since, "%Y-%m-%d") if since else None,
+                    datetime.strptime(until, "%Y-%m-%d") if until else None,
+                    encryption_key
+                )
+                return HistoriesResponse(messages=[
+                    Message(role=h["role"], content=h["content"])
+                    for h in histories
+                ])
+
+            except ValueError as verr:
+                return JSONResponse("Invalid encryption key", 400)
+
+            except Exception as ex:
+                logger.error(f"Error at get_histories: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+
+        @app.delete("/histories/{user_id}", response_model=ApiResponse, tags=["History"])
+        async def delete_histories(user_id: str, db: Session = Depends(self.get_db)):
+            try:
+                self.chatmemoryc.delete_histories(db, user_id)
+                db.commit()
+                return ApiResponse(message="All histories are deleted successfully")
+
+            except Exception as ex:
+                logger.error(f"Error at delete_histories: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+        @app.post("/archives/{user_id}", response_model=ApiResponse, tags=["Archive"])
+        async def archive_histories(user_id: str, request: ArchivesRequest, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
+            try:
+                for i in range(request.days):
+                    self.chatmemoryc.archive_histories(
+                        db, user_id,
+                        (datetime.strptime(request.target_date, "%Y-%m-%d") if request.target_date
+                         else datetime.utcnow()).date() - timedelta(days=request.days - i - 1),
+                        encryption_key
+                    )
+                    db.commit()
+                return ApiResponse(message="Histories archived successfully")
+
+            except Exception as ex:
+                logger.error(f"Error at archive_histories: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+        @app.get("/archives/{user_id}", response_model=ArchivesResponse, tags=["Archive"])
+        async def get_archives(user_id: str, since: str=None, until: str=None, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
+            try:
+                archives = self.chatmemoryc.get_archives(
+                    db, user_id,
+                    datetime.strptime(since, "%Y-%m-%d") if since else None,
+                    datetime.strptime(until, "%Y-%m-%d") if until else None,
+                    encryption_key
+                )
+                return ArchivesResponse(archives=[
+                    Archive(date=a["date"].strftime("%Y-%m-%d"), archive=a["archive"])
+                    for a in archives
+                ])
+
+            except ValueError as verr:
+                return JSONResponse("Invalid encryption key", 400)
+
+            except Exception as ex:
+                logger.error(f"Error at get_archives: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+
+        @app.delete("/archives/{user_id}", response_model=ApiResponse, tags=["Archive"])
+        async def delete_archives(user_id: str, db: Session = Depends(self.get_db)):
+            try:
+                self.chatmemoryc.delete_archives(db, user_id)
+                db.commit()
+                return ApiResponse(message="All archives are deleted successfully")
+
+            except Exception as ex:
+                logger.error(f"Error at delete_archives: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+        @app.post("/entities/{user_id}", response_model=ApiResponse, tags=["Entity"])
+        async def save_entities(user_id: str, request: EntitiesRequest, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
+            try:
+                now = datetime.utcnow()
+                if request.entities is None:
+                    for i in range(request.days):
+                        self.chatmemoryc.extract_entities(
+                            db, user_id,
+                            (datetime.strptime(request.target_date, "%Y-%m-%d") if request.target_date
+                            else now).date() - timedelta(days=request.days - i - 1),
+                            encryption_key
+                        )
+                        db.commit()
+                    return ApiResponse(message="Entities extracted and stored successfully")
+            
+                else:
+                    self.chatmemoryc.save_entities(db, user_id, now, now.date(), request.entities, encryption_key)
+                    db.commit()
+                    return ApiResponse(message="Entities stored successfully")
+
+            except Exception as ex:
+                logger.error(f"Error at save_entities: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+
+        @app.get("/entities/{user_id}", response_model=EntitiesResponse, tags=["Entity"])
+        async def get_entities(user_id: str, encryption_key: str = Header(default=None), db: Session = Depends(self.get_db)):
+            try:
+                entities = self.chatmemoryc.get_entities(db, user_id, encryption_key)
+                return EntitiesResponse(entities=entities)
+
+            except ValueError as verr:
+                return JSONResponse("Invalid encryption key", 400)
+
+            except Exception as ex:
+                logger.error(f"Error at get_entities: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+        @app.delete("/entities/{user_id}", response_model=ApiResponse, tags=["Entity"])
+        async def delete_entities(user_id: str, db: Session = Depends(self.get_db)):
+            try:
+                self.chatmemoryc.delete_entities(db, user_id)
+                db.commit()
+                return ApiResponse(message="All entities are deleted successfully")
+
+            except Exception as ex:
+                logger.error(f"Error at delete_entities: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+        @app.delete("/all/{user_id}", response_model=ApiResponse, tags=["All"])
+        async def delete_all(user_id: str, db: Session = Depends(self.get_db)):
+            try:
+                self.chatmemoryc.delete_all(db, user_id)
+                db.commit()
+                return ApiResponse(message=f"Delete all data for {user_id} successfully")
+
+            except Exception as ex:
+                logger.error(f"Error at delete_all: {ex}\n{traceback.format_exc()}")
+                return JSONResponse("Internal server error", 500)
+
+
+    def start(self, host :str="127.0.0.1", port: int=8124):
+        uvicorn.run(self.app, host=host, port=port)
```

### Comparing `chatmemoryc-0.1.4rc1/chatmemoryc.egg-info/PKG-INFO` & `chatmemoryc-0.1.4rc2/chatmemoryc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: chatmemoryc
-Version: 0.1.4rc1
+Version: 0.1.4rc2
 Summary: Long-term and medium-term memories between you and chatbot
 Home-page: https://github.com/f6844710/chatmemoryc
 Author: pino
 Author-email: f6844710@nifty.com
 Maintainer: pino
 Maintainer-email: f6844710@nifty.com
 License: Apache v2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: fastapi==0.105.0
-Requires-Dist: anthropic==0.23.0
+Requires-Dist: fastapi==0.110.0
+Requires-Dist: anthropic==0.28.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: SQLAlchemy==2.0.20
-Requires-Dist: uvicorn==0.23.1
-Requires-Dist: pycryptodome==3.18.0
+Requires-Dist: SQLAlchemy==2.0.28
+Requires-Dist: uvicorn==0.28.1
+Requires-Dist: pycryptodome==3.20.0
 
 # chatmemory
 
 Long-term and medium-term memories between you and chatbot💕
 
 # 🚀 Quick start
```

