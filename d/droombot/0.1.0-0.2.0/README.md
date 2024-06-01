# Comparing `tmp/droombot-0.1.0.tar.gz` & `tmp/droombot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droombot-0.1.0.tar", max compression
+gzip compressed data, was "droombot-0.2.0.tar", max compression
```

## Comparing `droombot-0.1.0.tar` & `droombot-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-04-04 18:28:42.131894 droombot-0.1.0/LICENSE
--rw-r--r--   0        0        0     2933 2023-04-04 19:18:04.624911 droombot-0.1.0/README.md
--rw-r--r--   0        0        0     1019 2023-04-04 18:48:29.641494 droombot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:27:49.224688 droombot-0.1.0/src/droombot/__init__.py
--rw-r--r--   0        0        0     3138 2023-04-04 18:36:21.362402 droombot-0.1.0/src/droombot/api.py
--rw-r--r--   0        0        0     5161 2023-04-04 18:36:21.402402 droombot-0.1.0/src/droombot/bot.py
--rw-r--r--   0        0        0     1115 2023-04-04 18:36:21.390402 droombot-0.1.0/src/droombot/cli.py
--rw-r--r--   0        0        0     1460 2023-04-04 18:36:21.382402 droombot-0.1.0/src/droombot/config.py
--rw-r--r--   0        0        0     1650 2023-04-04 18:36:21.394402 droombot-0.1.0/src/droombot/log.py
--rw-r--r--   0        0        0     4300 2023-04-04 18:36:21.358402 droombot-0.1.0/src/droombot/models.py
--rw-r--r--   0        0        0        0 2023-04-04 18:46:12.560545 droombot-0.1.0/src/droombot/py.typed
--rw-r--r--   0        0        0     1093 2023-04-04 18:36:21.370402 droombot-0.1.0/src/droombot/utils.py
--rw-r--r--   0        0        0     1619 2023-04-04 18:36:21.374402 droombot-0.1.0/src/droombot/version.py
--rw-r--r--   0        0        0     3302 2023-04-04 18:36:21.350401 droombot-0.1.0/src/droombot/worker.py
--rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 droombot-0.1.0/setup.py
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 droombot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-04 18:28:42.131894 droombot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3487 2024-06-01 14:06:39.223330 droombot-0.2.0/README.md
+-rw-r--r--   0        0        0     1034 2024-06-01 14:06:39.227330 droombot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 19:27:49.224688 droombot-0.2.0/src/droombot/__init__.py
+-rw-r--r--   0        0        0     3506 2024-06-01 14:06:39.227330 droombot-0.2.0/src/droombot/api.py
+-rw-r--r--   0        0        0     5212 2024-06-01 14:06:39.227330 droombot-0.2.0/src/droombot/bot.py
+-rw-r--r--   0        0        0     1120 2024-06-01 14:06:39.227330 droombot-0.2.0/src/droombot/cli.py
+-rw-r--r--   0        0        0     1465 2024-06-01 14:06:39.227330 droombot-0.2.0/src/droombot/config.py
+-rw-r--r--   0        0        0     1655 2024-06-01 14:06:39.227330 droombot-0.2.0/src/droombot/log.py
+-rw-r--r--   0        0        0     3899 2024-06-01 14:06:39.227330 droombot-0.2.0/src/droombot/models.py
+-rw-r--r--   0        0        0        0 2023-04-04 18:46:12.560545 droombot-0.2.0/src/droombot/py.typed
+-rw-r--r--   0        0        0     1098 2024-06-01 14:06:39.231330 droombot-0.2.0/src/droombot/utils.py
+-rw-r--r--   0        0        0     1624 2024-06-01 14:06:39.231330 droombot-0.2.0/src/droombot/version.py
+-rw-r--r--   0        0        0     3824 2024-06-01 14:06:39.231330 droombot-0.2.0/src/droombot/worker.py
+-rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 droombot-0.2.0/PKG-INFO
```

### Comparing `droombot-0.1.0/LICENSE` & `droombot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `droombot-0.1.0/pyproject.toml` & `droombot-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "droombot"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Discord Bot for generating images from text prompts"
 authors = ["Sander Bollen <sander@sndrtj.eu>"]
 readme = "README.md"
 packages = [
     {include = "droombot", from = "src" }
 ]
 license = "Apache-2.0"
@@ -13,34 +13,32 @@
     "Development Status :: 3 - Alpha",
     "Topic :: Communications :: Chat",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = {version ="^3.8.4", extras = ['speedups'] }
-pydantic = "^1.10.7"
+pydantic = "^2.7.2"
 click = "^8.1.3"
 py-cord = {extras = ["speed"], version = "^2.4.1"}
 redis = {extras = ["hiredis"], version = "^4.5.4"}
 aiolimiter = "^1.0.0"
+typing-extensions = "^4.12.0"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
 mypy = "^1.1.1"
-isort = "^5.12.0"
-ruff = "^0.0.259"
+ruff = "^0.4.7"
 pytest = "^7.2.2"
 pre-commit = "^3.2.1"
 types-redis = "^4.5.4.1"
 
 [tool.poetry.scripts]
 droombot = 'droombot.cli:cli'
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-
-[tool.isort]
-profile = "black"
+[tool.ruff.lint]
+select =  ["E4", "E7", "E9", "F", "I"]
```

### Comparing `droombot-0.1.0/src/droombot/api.py` & `droombot-0.2.0/src/droombot/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,103 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import asyncio
-import json
 import logging
 
 import aiohttp
 
 from .config import STABILITY_API_KEY
-from .models import TextToImageRequest, TextToImageResponse
+from .models import (
+    TextToImageRequestV2Core,
+    TextToImageRequestV2SD3,
+    TextToImageResponse,
+)
 from .version import VERSION
 
 logger = logging.getLogger(__name__)
 
-TEX_TO_IMAGE_BASE_URL = "https://api.stability.ai/v1/generation"
+CORE_TEXT_TO_IMAGE_BASE_URL = (
+    "https://api.stability.ai/v2beta/stable-image/generate/core"
+)
+SD3_TEXT_TO_IMAGE_BASE_URL = "https://api.stability.ai/v2beta/stable-image/generate/sd3"
 
 
 async def text_to_image(
-    session: aiohttp.ClientSession, request: TextToImageRequest, timeout: int = 300
+    session: aiohttp.ClientSession,
+    request: TextToImageRequestV2Core | TextToImageRequestV2SD3,
+    timeout: int = 300,
 ) -> list[TextToImageResponse]:
     """Call Stability with a text to image request
 
     :param session: AIOhttp session
     :param request: the incoming request
     :param timeout: timeout in seconds, defaults to 300. Don't set too low, as
         image generation takes some time.
     :return: list of responses, one for each text prompt
     :raises: timeout
     """
-    logger.info(
-        "Incoming call for text-to-image generation with "
-        f"engine id {request.engine_id}"
-    )
+    match request:
+        case TextToImageRequestV2Core():
+            logger.info("Incoming call for text-to-image generation for Core")
+            url = CORE_TEXT_TO_IMAGE_BASE_URL
+        case TextToImageRequestV2SD3():
+            logger.info("Incoming call for text-to-image generation for SD3")
+            url = SD3_TEXT_TO_IMAGE_BASE_URL
+        case _:
+            raise ValueError(f"Unsupported request: {type(request)}")
+
     user_agent = f"droombot/{VERSION}"
-    headers = {"Authorization": f"Bearer {STABILITY_API_KEY}", "User-Agent": user_agent}
-    url = f"{TEX_TO_IMAGE_BASE_URL}/{request.engine_id}/text-to-image"
-    logger.debug(f"Generated url: {url}")
-
-    # FIXME: need to load json serialized because enums.
-    raw_post_data = json.loads(request.json())
-    # need to filter out engine_id and sampler if it is none
-    post_data = {}
+    headers = {
+        "Authorization": f"Bearer {STABILITY_API_KEY}",
+        "User-Agent": user_agent,
+        "accept": "application/json",
+    }
+
+    raw_post_data = request.model_dump(mode="json")
+    writer = aiohttp.MultipartWriter("form-data")
+    # filter out values that are None
     for k, v in raw_post_data.items():
-        if k == "engine_id":
-            continue
-        if k == "sampler" and v is None:
+        if v is None:
             continue
-        post_data[k] = v
+        writer.append(
+            aiohttp.StringPayload(value=str(v)),
+            headers={aiohttp.hdrs.CONTENT_DISPOSITION: f'form-data; name="{k}"'},
+        )
 
     async with session.post(
-        url=url, json=post_data, timeout=timeout, headers=headers
+        url=url, data=writer, timeout=timeout, headers=headers
     ) as resp:
         results = await resp.json()
         if resp.status >= 400:
             logger.error(f"Call to Stability errored. Response: {results}")
             raise ValueError("An error occurred")
 
     # responses are encoded in an 'artifacts' item, but this is NOT
     # mentioned in the docs.
     logger.info("Received a successful response from text-to-image generation.")
-    return [TextToImageResponse.from_raw_api(r) for r in results["artifacts"]]
+    return [TextToImageResponse.from_raw_api(results)]
 
 
 if __name__ == "__main__":
     # for testing
     async def main():
-        request = TextToImageRequest(
-            text_prompts=[
-                {
-                    "text": "Green trees in a forest with ferns, oil painting",
-                    "weight": 0.5,
-                }
-            ],
+        request = TextToImageRequestV2Core(
+            prompt="Green trees in a forest with ferns, oil painting"
         )
         async with aiohttp.ClientSession() as session:
             results = await text_to_image(session, request)
 
-        print(results)
+        print(results[0].model_dump_json())
 
     asyncio.run(main())
```

### Comparing `droombot-0.1.0/src/droombot/bot.py` & `droombot-0.2.0/src/droombot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -51,15 +51,17 @@
             logger.debug(f"Polling for {interaction_key}")
             raw_results = await redis_connection.get(interaction_key)
         if raw_results is None:
             logger.debug(f"Interaction {interaction_key} not found, trying again")
             continue
 
         logger.debug("Found results, parsing to response")
-        return pydantic.parse_raw_as(list[TextToImageResponse], raw_results)
+        return pydantic.TypeAdapter(list[TextToImageResponse]).validate_json(
+            raw_results
+        )
 
 
 def create_bot() -> discord.Bot:
     """Create the discord bot
 
     :return:
     """
@@ -92,15 +94,15 @@
         )
 
         logger.info("Sending message to redis for worker to pick up")
         message = PubSubMessage(
             interaction_id=str(ctx.interaction.id), text_prompt=text
         )
 
-        await redis_connection.publish("droombot-prompts", message.json())
+        await redis_connection.publish("droombot-prompts", message.model_dump_json())
         logger.info("Polling for result")
 
         try:
             image_results = await poll_interaction_result(
                 redis_connection, str(ctx.interaction.id)
             )
         except TimeoutError:
```

### Comparing `droombot-0.1.0/src/droombot/cli.py` & `droombot-0.2.0/src/droombot/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `droombot-0.1.0/src/droombot/config.py` & `droombot-0.2.0/src/droombot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `droombot-0.1.0/src/droombot/log.py` & `droombot-0.2.0/src/droombot/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `droombot-0.1.0/src/droombot/models.py` & `droombot-0.2.0/src/droombot/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,159 +1,130 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-
-
+import argparse
 import enum
-from typing import Literal, TypedDict, cast
+import logging
+import shlex
+from typing import Annotated, Literal
 
 import pydantic
 
-EngineId = Literal[
-    "Stable Diffusion v1.4",
-    "stable-diffusion-v1-5",
-    "stable-diffusion-512-v2-0",
-    "stable-diffusion-768-v2-0",
-    "stable-diffusion-512-v2-1",
-    "stable-diffusion-768-v2-1",
-]
-
-
-class TextPrompt(TypedDict):
-    text: str
-    weight: float
-
-
-class ClipGuidancePreset(enum.Enum):
-    NONE = "NONE"
-    FAST_BLUE = "FAST_BLUE"
-    FAST_GREEN = "FAST_GREEN"
-    SIMPLE = "SIMPLE"
-    SLOW = "SLOW"
-    SLOWER = "SLOWER"
-    SLOWEST = "SLOWEST"
-
-
-class Sampler(enum.Enum):
-    DDIM = "DDIM"
-    DDPM = "DDPM"
-    K_DPMPP_2M = "K_DPMPP_2M"
-    K_DPMPP_2S_ANCESTRAL = "K_DPMPP_2S_ANCESTRAL"
-    K_DPM_2 = "K_DPM_2"
-    K_DPM_2_ANCESTRAL = "K_DPM_2_ANCESTRAL"
-    K_EULER = "K_EULER"
-    K_EULER_ANCESTRAL = "K_EULER_ANCESTRAL"
-    K_HEUN = "K_HEUN"
-    K_LMS = "K_LMS"
+logger = logging.getLogger(__name__)
 
 
 class FinishReason(enum.Enum):
     CONTENT_FILTERED = "CONTENT_FILTERED"
     ERROR = "ERROR"
     SUCCESS = "SUCCESS"
 
 
-# It's 2023, and `pydantic.conint / conlist` still doesn't work nicely with mypy.
-# https://github.com/pydantic/pydantic/issues/156
-class SizeType(pydantic.ConstrainedInt):
-    multiple_of = 64
-    ge = 128
-
-
-class CfgScaleType(pydantic.ConstrainedInt):
-    ge = 0
-    le = 35
-
-
-class SeedType(pydantic.ConstrainedInt):
-    ge = 0
-    le = 4294967295
-
-
-class StepsType(pydantic.ConstrainedInt):
-    ge = 10
-    le = 150
-
-
-# Docs: https://platform.stability.ai/rest-api#tag/v1generation/operation/textToImage
-class TextToImageRequest(pydantic.BaseModel):
-    engine_id: EngineId = "stable-diffusion-512-v2-1"
-
-    height: SizeType = cast(SizeType, 512)
-    width: SizeType = cast(SizeType, 512)
-
-    text_prompts: list[TextPrompt]
-    cfg_scale: CfgScaleType = cast(CfgScaleType, 7)
-    clip_guidance_present: ClipGuidancePreset = ClipGuidancePreset.NONE
-
-    # None should indicate omit from api call
-    sampler: Sampler | None = None
-
-    # 0 = random
-    seed: SeedType = cast(SeedType, 0)
-
-    # number of diffusion steps
-    steps: StepsType = cast(StepsType, 50)
-
-    @pydantic.validator("width")
-    def image_size_must_be_within_bounds(cls, v, values, **kwargs):
-        # height and width must be between 589,824 and ≤ 1,048,576 if model is 768
-        # else between 262,144 and  1,048,576
-        engine_id = values["engine_id"]
-        height = values["height"]
-
-        image_size = height * v
-
-        if "768" in engine_id:
-            min_bound = 589_824
-        else:
-            min_bound = 262_144
-
-        if min_bound <= image_size <= 1_048_576:
-            return v
+ASPECT_RATIOS = Literal["16:9", "1:1", "21:9", "2:3", "3:2", "4:5", "9:16", "9:21"]
+STYLE_PRESETS = Literal[
+    "3d-model",
+    "analog-film",
+    "anime",
+    "cinematic",
+    "comic-book",
+    "digital-art",
+    "enhance",
+    "fantasy-art",
+    "isometric",
+    "line-art",
+    "low-poly",
+    "modeling-compound",
+    "neon-punk",
+    "origami",
+    "photographic",
+    "pixel-art",
+    "tile-texture",
+]
 
-        raise ValueError(f"Image size {image_size} is out of bounds.")
 
-    @pydantic.validator("text_prompts")
-    def text_prompts_must_be_at_least_one(cls, v):
-        # conlist can't seem to cope well with typedicts
-        # thus doing it with manual validator
-        if len(v) == 0:
-            raise ValueError("Text prompts must have at least one member")
-        return v
+SeedType = Annotated[int, pydantic.Field(ge=0, le=4294967295)]
+PromptType = Annotated[str, pydantic.Field(min_length=1, max_length=10_000)]
+NegativePromptType = Annotated[str, pydantic.Field(min_length=0, max_length=10_000)]
 
 
 class TextToImageResponse(pydantic.BaseModel):
     # base-64 encoded image or null if finish reason is not success
     base64: str | None
     # the finish reason
     finish_reason: FinishReason
     # What seed ended up being used for this
     seed: int
 
     @classmethod
     def from_raw_api(cls, raw_api_response: dict) -> "TextToImageResponse":
         return cls(
-            base64=raw_api_response["base64"],
-            finish_reason=raw_api_response["finishReason"],
+            base64=raw_api_response["image"],
+            finish_reason=raw_api_response["finish_reason"],
             seed=raw_api_response["seed"],
         )
 
 
+class TextToImageRequestV2Core(pydantic.BaseModel):
+    """TextToImage request for the core v2 api of Stability AI"""
+
+    prompt: PromptType
+    aspect_ratio: ASPECT_RATIOS = "1:1"
+    negative_prompt: NegativePromptType | None = None
+    seed: SeedType = 0
+    style_preset: STYLE_PRESETS | None = None
+    output_format: Literal["jpeg", "png", "webp"] = "png"
+
+
+class TextToImageRequestV2SD3(pydantic.BaseModel):
+    """TextToImage request for the Stable Diffusion 3 api of Stability AI"""
+
+    prompt: PromptType
+    aspect_ratio: ASPECT_RATIOS = "1:1"
+    negative_prompt: NegativePromptType | None = None
+    model: Literal["sd3", "sd3-turbo"] = "sd3"
+    seed: SeedType = 0
+    output_format: Literal["jpeg", "png"] = "png"
+
+
 class PubSubMessage(pydantic.BaseModel):
     """Message used for passing in pub/sub"""
 
     # the discord interaction id
     interaction_id: str
 
     # The text prompt used
     text_prompt: str
+
+
+def pubsub_to_t2i(
+    message: PubSubMessage,
+) -> TextToImageRequestV2Core | TextToImageRequestV2SD3:
+    """Convert a pubsub message to a text 2 image request
+
+    :param message: the message
+    :return: text to image request
+    """
+    parser = argparse.ArgumentParser(exit_on_error=False)
+    parser.add_argument(
+        "-m", "--model", choices=["core", "sd3", "sd3-turbo"], default="core"
+    )
+
+    # we want to consider everything before a `-` as the text prompt, without quoting.
+    prompt, maybe_dash, options = message.text_prompt.partition("-")
+
+    args, failures = parser.parse_known_args(shlex.split(maybe_dash + options), None)
+    if failures:
+        logger.warning(f"Unrecognized arguments: {''.join(failures)}, ignoring...")
+
+    if args.model == "core":
+        return TextToImageRequestV2Core(prompt=prompt.strip())
+
+    return TextToImageRequestV2SD3(prompt=prompt.strip(), model=args.model)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `droombot-0.1.0/src/droombot/utils.py` & `droombot-0.2.0/src/droombot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `droombot-0.1.0/src/droombot/version.py` & `droombot-0.2.0/src/droombot/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `droombot-0.1.0/src/droombot/worker.py` & `droombot-0.2.0/src/droombot/worker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,82 @@
-#    Copyright 2023 Sander Bollen
+#    Copyright 2023-2024 Sander Bollen
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-
 import asyncio
 import json
 import logging
+import traceback
 
 import aiohttp
 import pydantic
 import pydantic.json
 import redis.asyncio as redis
 from aiolimiter import AsyncLimiter
 
 from .api import text_to_image
 from .config import MAX_REQUESTS_PER_MINUTE, REDIS_HOST, REDIS_KEY_LIFETIME, REDIS_PORT
-from .models import PubSubMessage, TextPrompt, TextToImageRequest
+from .models import PubSubMessage, pubsub_to_t2i
 
 logger = logging.getLogger(__name__)
 
 
 class Worker:
     def __init__(self):
         self._redis_connection = redis.Redis(host=REDIS_HOST, port=REDIS_PORT)
 
+        self._running_tasks: set[asyncio.Task] = set()
+        self._wait_lock = asyncio.Lock()
+
     def run(self):
         logger.info("Starting worker...")
         asyncio.run(self.loop())
 
+    def _done_callback(self, t: asyncio.Task) -> None:
+        if (exc := t.exception()) is not None:
+            logger.error(
+                f"Task {t.get_name()} raised an exception during execution...: {exc} "
+                f"\n \n {''.join(traceback.format_tb(exc.__traceback__))}"
+            )
+        self._running_tasks.discard(t)
+
     async def loop(self):
         """Main application loop"""
         http_client = aiohttp.ClientSession()
         limiter = AsyncLimiter(MAX_REQUESTS_PER_MINUTE)
         async with self._redis_connection.pubsub() as pubsub:
             await pubsub.subscribe("droombot-prompts")
             while True:
                 async with limiter:
-                    asyncio.ensure_future(self.read_and_run(pubsub, http_client))
+                    task = asyncio.create_task(self.read_and_run(pubsub, http_client))
+                    self._running_tasks.add(task)
+                    task.add_done_callback(self._done_callback)
 
     async def read_and_run(
         self, channel: redis.client.PubSub, session: aiohttp.ClientSession
     ) -> None:
         """Read redis channel for new message, and run text-to-image if there is one.
 
         The result is stored back into redis by the interaction id
 
         :return: None
         """
-        message = await channel.get_message(ignore_subscribe_messages=True)
+        async with self._wait_lock:
+            message = await channel.get_message(ignore_subscribe_messages=True)
+
         if message is None:
             logger.debug("No message to process...")
             return
 
         try:
             deserialized_message = PubSubMessage.parse_raw(message["data"])
         except pydantic.ValidationError as e:
@@ -70,17 +85,15 @@
 
         logger.info(
             "Received message with for interaction "
             f"{deserialized_message.interaction_id} with prompt: "
             f"'{deserialized_message.text_prompt}'"
         )
 
-        text_to_image_request = TextToImageRequest(
-            text_prompts=[TextPrompt(text=deserialized_message.text_prompt, weight=1.0)]
-        )
+        text_to_image_request = pubsub_to_t2i(deserialized_message)
 
         logger.info("Running text-to-image conversion")
         responses = await text_to_image(session, text_to_image_request)
         logger.info("Received response from text-to-image conversion")
         serialized_responses = json.dumps(
             responses, default=pydantic.json.pydantic_encoder
         )
```

### Comparing `droombot-0.1.0/PKG-INFO` & `droombot-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: droombot
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Discord Bot for generating images from text prompts
 Home-page: https://github.com/sndrtj/droombot
 License: Apache-2.0
 Author: Sander Bollen
 Author-email: sander@sndrtj.eu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Chat
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
 Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: py-cord[speed] (>=2.4.1,<3.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.7.2,<3.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0)
+Requires-Dist: typing-extensions (>=4.12.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Droombot
 
 Droombot is a discord bot for generating images from text prompts.
 
 At current, it uses an API call to Stability.ai to generate images.
 A future version may support running Stable Diffusion directly.
 
+
+https://user-images.githubusercontent.com/7782240/229916443-2cc0aa4d-188b-47c1-947e-9fd1708f4fba.mp4
+
+
 ## Installing
 
 :zap: Note: this step is not necessary if using a Container (see below)
 
 Run the following, preferably in a virtual environment, to install droombot
 
 ```console
@@ -52,14 +59,25 @@
 
 To start a worker, run the following in the virtual environment
 
 ```console
 droombot worker
 ```
 
+## How to use in discord
+
+Use the `/prompt` command to type your prompt. This by default uses whatever model
+Stability AI now considers its "core". You can also select Stable Diffusion 3 and
+Stable Diffusion 3 Turbo models by appending `-m sd3` or `-m sd3-turbo` to your
+prompt.
+
+You can give individual words in your prompt more some weight by doing something like
+the following;
+``A table with (red:0.5) raspberries and (purple:0.5) blueberries.``
+
 ## Components
 
 Droombot consists of two components:
 
 1. The `server`, this handles interaction with the user. I.e., it handles incoming
    prompts and replies. It provides the Discord bot users interact with.
 2. One or more `worker`s. These handle the actual image generation.
@@ -79,15 +97,15 @@
 | `REDIS_PORT`              | Port of Redis instance                                                         | No, defaults to 6379      |
 | `REDIS_KEY_LIFETIME`      | Number of seconds for keys to expire                                           | No, defaults to 300       |
 | `MAX_REQUESTS_PER_MINUTE` | Maximum number of requests per minute to any remote services                   | No, defaults to 100       |
 
 
 ## Container
 
-Droombot can run as a container. For a howto using Docker or Podman, see the 
+Droombot can run as a container. For a howto using Docker or Podman, see the
 [container docs](docs/containers.md).
 
 ## Future plans
 
 1. Expose additional options, such as multiple images and model selection.
 2. Ability to run Stable Diffusion directly, with a separate worker class
 3. Prompt translations, allowing users to use prompts in their own language.
```

