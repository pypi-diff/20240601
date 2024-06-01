# Comparing `tmp/spot_llm-0.2.0.tar.gz` & `tmp/spot_llm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spot_llm-0.2.0.tar", max compression
+gzip compressed data, was "spot_llm-0.3.0.tar", max compression
```

## Comparing `spot_llm-0.2.0.tar` & `spot_llm-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2107 2024-05-31 18:45:19.328686 spot_llm-0.2.0/README.md
--rw-r--r--   0        0        0      540 2024-05-31 18:45:19.329686 spot_llm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      149 2024-05-31 18:45:19.329686 spot_llm-0.2.0/spot_llm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 18:45:19.363686 spot_llm-0.2.0/spot_llm/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 18:45:19.363686 spot_llm-0.2.0/spot_llm/models/gemma7b.py
--rw-r--r--   0        0        0      978 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/hf_model.py
--rw-r--r--   0        0        0      223 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/mistral7b.py
--rw-r--r--   0        0        0      239 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/opt125.py
--rw-r--r--   0        0        0     1657 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/spotter.py
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 spot_llm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2107 2024-05-31 19:54:00.094945 spot_llm-0.3.0/README.md
+-rw-r--r--   0        0        0      540 2024-05-31 19:54:00.095945 spot_llm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-05-31 19:54:00.095945 spot_llm-0.3.0/spot_llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 19:54:00.127945 spot_llm-0.3.0/spot_llm/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 19:54:00.127945 spot_llm-0.3.0/spot_llm/models/gemma7b.py
+-rw-r--r--   0        0        0     1025 2024-05-31 19:54:00.095945 spot_llm-0.3.0/spot_llm/models/hf_model.py
+-rw-r--r--   0        0        0      223 2024-05-31 19:54:00.096945 spot_llm-0.3.0/spot_llm/models/mistral7b.py
+-rw-r--r--   0        0        0      239 2024-05-31 19:54:00.096945 spot_llm-0.3.0/spot_llm/models/opt125.py
+-rw-r--r--   0        0        0     1646 2024-05-31 19:54:00.096945 spot_llm-0.3.0/spot_llm/models/spotter.py
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 spot_llm-0.3.0/PKG-INFO
```

### Comparing `spot_llm-0.2.0/README.md` & `spot_llm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spot_llm-0.2.0/pyproject.toml` & `spot_llm-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spot-llm"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Edouard Yvinec <edouardyvinec@hotmail.fr>", "Gabriel Kasser <gabriel.kasser@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 torch = "^2.3.0"
```

### Comparing `spot_llm-0.2.0/spot_llm/models/hf_model.py` & `spot_llm-0.3.0/spot_llm/models/hf_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from transformers import AutoTokenizer, AutoModelForCausalLM  # type: ignore
 
 from spot_llm.models.spotter import Spotter
 
 
 class HFSpotter(Spotter):
     def __init__(self, model_id: str, token: Optional[str] = None):
+        torch.set_default_dtype(torch.float16)
         super().__init__(model_id=model_id, token=token)
 
     def initialize(self) -> None:
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_id, token=self.token)
         self.model = AutoModelForCausalLM.from_pretrained(
             self.model_id, token=self.token, device_map="auto"
         )
```

### Comparing `spot_llm-0.2.0/spot_llm/models/spotter.py` & `spot_llm-0.3.0/spot_llm/models/spotter.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class Spotter:
     def __init__(
         self,
         model_id: str,
         token: Optional[str] = None,
-        base_token_count: int = 24,
+        base_token_count: int = 10,
     ) -> None:
         self.model_id = model_id
         self.token = token
         self.base_token_count = base_token_count
         self.tokenizer: Any
         self.model: Any
         self.initialize()
@@ -34,24 +34,24 @@
     @abstractmethod
     def _get_lazy_logits(
         self,
         inputs: Tensor,
     ) -> Tensor:
         raise NotImplementedError()
 
-    def score(self, text: str, num_tokens: int = 24) -> float:
+    def score(self, text: str) -> float:
 
         outputs, tokenz = self.predict_logits_and_tokenz(text)
 
         output = outputs[0][0]
         rankings: List[int] = []
         for i in range(output.shape[0] - 1):
-            if i < num_tokens:
+            if i < self.base_token_count:
                 continue
-            logit = output[i + 1, :]
+            logit = output[i - 1, :]
             actual_token = tokenz[0, i]
             rankings.append(int((logit > logit[actual_token]).sum().item()))
 
         if len(rankings) == 0:
             return -1.0
         return float(np.mean(rankings) / output.shape[1])
```

### Comparing `spot_llm-0.2.0/PKG-INFO` & `spot_llm-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spot-llm
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Edouard Yvinec
 Author-email: edouardyvinec@hotmail.fr
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

