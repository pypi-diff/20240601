# Comparing `tmp/dspy_ai-2.5.0rc2.tar.gz` & `tmp/dspy_ai-2.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspy_ai-2.5.0rc2.tar", max compression
+gzip compressed data, was "dspy_ai-2.5.0rc3.tar", max compression
```

## Comparing `dspy_ai-2.5.0rc2.tar` & `dspy_ai-2.5.0rc3.tar`

### file list

```diff
@@ -1,92 +1,146 @@
--rw-r--r--   0        0        0     1085 2024-01-27 20:16:46.845164 dspy_ai-2.5.0rc2/LICENSE
--rw-r--r--   0        0        0    35950 2024-05-27 13:53:59.380701 dspy_ai-2.5.0rc2/README.md
--rw-r--r--   0        0        0     1204 2024-05-29 20:05:59.696560 dspy_ai-2.5.0rc2/dspy/__init__.py
--rw-r--r--   0        0        0      122 2024-04-05 16:07:52.848121 dspy_ai-2.5.0rc2/dspy/datasets/__init__.py
--rw-r--r--   0        0        0     2986 2024-04-05 16:07:52.848222 dspy_ai-2.5.0rc2/dspy/datasets/colors.py
--rw-r--r--   0        0        0     5162 2024-05-29 20:05:59.696687 dspy_ai-2.5.0rc2/dspy/datasets/dataloader.py
--rw-r--r--   0        0        0     4098 2024-04-05 16:07:52.848414 dspy_ai-2.5.0rc2/dspy/datasets/dataset.py
--rw-r--r--   0        0        0     2618 2024-04-05 16:07:52.848498 dspy_ai-2.5.0rc2/dspy/datasets/gsm8k.py
--rw-r--r--   0        0        0     3286 2024-04-05 16:07:52.848598 dspy_ai-2.5.0rc2/dspy/datasets/hotpotqa.py
--rw-r--r--   0        0        0      127 2024-04-05 16:07:52.848699 dspy_ai-2.5.0rc2/dspy/evaluate/__init__.py
--rw-r--r--   0        0        0     1421 2024-04-05 16:07:52.848822 dspy_ai-2.5.0rc2/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0        0        0    11414 2024-05-27 13:53:59.390403 dspy_ai-2.5.0rc2/dspy/evaluate/evaluate.py
--rw-r--r--   0        0        0      882 2024-04-05 16:07:52.852527 dspy_ai-2.5.0rc2/dspy/evaluate/metrics.py
--rw-r--r--   0        0        0       57 2024-04-05 16:07:52.852610 dspy_ai-2.5.0rc2/dspy/experimental/__init__.py
--rw-r--r--   0        0        0       26 2024-04-05 16:07:52.852700 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0        0        0      834 2024-04-05 16:07:52.852759 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/config.py
--rw-r--r--   0        0        0      527 2024-04-05 16:07:52.852825 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0        0        0     5543 2024-04-05 16:07:52.852897 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0        0        0     9567 2024-05-29 20:05:59.696817 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0        0        0      599 2024-04-05 16:07:52.853143 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0        0        0     4237 2024-05-27 13:53:59.390647 dspy_ai-2.5.0rc2/dspy/experimental/synthetic_data.py
--rw-r--r--   0        0        0       94 2024-04-05 16:07:52.853820 dspy_ai-2.5.0rc2/dspy/functional/__init__.py
--rw-r--r--   0        0        0    20120 2024-05-29 20:05:59.696945 dspy_ai-2.5.0rc2/dspy/functional/functional.py
--rw-r--r--   0        0        0       47 2024-05-29 20:05:59.697246 dspy_ai-2.5.0rc2/dspy/modeling/__init__.py
--rw-r--r--   0        0        0       60 2024-05-29 20:05:59.697326 dspy_ai-2.5.0rc2/dspy/modeling/backends/__init__.py
--rw-r--r--   0        0        0     4724 2024-05-29 20:05:59.697392 dspy_ai-2.5.0rc2/dspy/modeling/backends/base.py
--rw-r--r--   0        0        0     3777 2024-05-29 20:05:59.697443 dspy_ai-2.5.0rc2/dspy/modeling/backends/json.py
--rw-r--r--   0        0        0     7459 2024-05-29 20:05:59.697507 dspy_ai-2.5.0rc2/dspy/modeling/backends/text.py
--rw-r--r--   0        0        0      348 2024-04-05 16:07:52.854456 dspy_ai-2.5.0rc2/dspy/predict/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-29 20:05:59.697772 dspy_ai-2.5.0rc2/dspy/predict/aggregation.py
--rw-r--r--   0        0        0     3589 2024-04-05 16:07:52.854648 dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought.py
--rw-r--r--   0        0        0     1527 2024-04-05 16:07:52.854742 dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0        0        0     1133 2024-05-27 13:53:59.392833 dspy_ai-2.5.0rc2/dspy/predict/knn.py
--rw-r--r--   0        0        0     6129 2024-05-27 13:53:59.392953 dspy_ai-2.5.0rc2/dspy/predict/langchain.py
--rw-r--r--   0        0        0     1659 2024-04-05 16:07:52.855060 dspy_ai-2.5.0rc2/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0        0        0       58 2024-01-27 20:16:47.215842 dspy_ai-2.5.0rc2/dspy/predict/parameter.py
--rw-r--r--   0        0        0     7252 2024-05-29 20:05:59.697915 dspy_ai-2.5.0rc2/dspy/predict/predict.py
--rw-r--r--   0        0        0     7598 2024-05-29 20:05:59.698038 dspy_ai-2.5.0rc2/dspy/predict/program_of_thought.py
--rw-r--r--   0        0        0     4614 2024-05-27 13:53:59.393278 dspy_ai-2.5.0rc2/dspy/predict/react.py
--rw-r--r--   0        0        0     3115 2024-05-29 20:05:59.698147 dspy_ai-2.5.0rc2/dspy/predict/retry.py
--rw-r--r--   0        0        0      132 2024-04-05 16:07:52.855575 dspy_ai-2.5.0rc2/dspy/primitives/__init__.py
--rw-r--r--   0        0        0    11319 2024-05-27 13:53:59.393559 dspy_ai-2.5.0rc2/dspy/primitives/assertions.py
--rw-r--r--   0        0        0     7779 2024-01-27 20:16:47.216399 dspy_ai-2.5.0rc2/dspy/primitives/box.py
--rw-r--r--   0        0        0     3416 2024-05-29 20:05:59.698251 dspy_ai-2.5.0rc2/dspy/primitives/example.py
--rw-r--r--   0        0        0     3831 2024-05-27 13:53:59.393756 dspy_ai-2.5.0rc2/dspy/primitives/module.py
--rw-r--r--   0        0        0     4836 2024-05-29 20:05:59.698359 dspy_ai-2.5.0rc2/dspy/primitives/prediction.py
--rw-r--r--   0        0        0     3366 2024-04-05 16:07:52.856229 dspy_ai-2.5.0rc2/dspy/primitives/program.py
--rw-r--r--   0        0        0    25710 2024-04-05 16:07:52.856677 dspy_ai-2.5.0rc2/dspy/primitives/python_interpreter.py
--rw-r--r--   0        0        0       30 2024-01-27 20:16:47.216808 dspy_ai-2.5.0rc2/dspy/retrieve/__init__.py
--rw-r--r--   0        0        0    17405 2024-05-27 13:53:59.393937 dspy_ai-2.5.0rc2/dspy/retrieve/azureaisearch_rm.py
--rw-r--r--   0        0        0     5683 2024-05-29 20:05:59.698525 dspy_ai-2.5.0rc2/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0        0        0     3264 2024-05-29 20:05:59.698629 dspy_ai-2.5.0rc2/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0        0        0     6604 2024-05-27 13:53:59.394297 dspy_ai-2.5.0rc2/dspy/retrieve/databricks_rm.py
--rw-r--r--   0        0        0     3804 2024-05-29 20:05:59.698742 dspy_ai-2.5.0rc2/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0        0        0     6605 2024-05-27 13:53:59.394532 dspy_ai-2.5.0rc2/dspy/retrieve/faiss_rm.py
--rw-r--r--   0        0        0     2937 2024-05-27 13:53:59.394597 dspy_ai-2.5.0rc2/dspy/retrieve/llama_index_rm.py
--rw-r--r--   0        0        0     3459 2024-04-05 16:07:52.857777 dspy_ai-2.5.0rc2/dspy/retrieve/marqo_rm.py
--rw-r--r--   0        0        0     3998 2024-05-27 13:53:59.394660 dspy_ai-2.5.0rc2/dspy/retrieve/milvus_rm.py
--rw-r--r--   0        0        0     3774 2024-04-05 16:07:52.857887 dspy_ai-2.5.0rc2/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0        0        0     6213 2024-04-05 16:07:52.857964 dspy_ai-2.5.0rc2/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0        0        0     5904 2024-05-29 20:05:59.698885 dspy_ai-2.5.0rc2/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0        0        0    10476 2024-04-05 16:07:52.858267 dspy_ai-2.5.0rc2/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0        0        0     4951 2024-05-27 13:53:59.394882 dspy_ai-2.5.0rc2/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0        0        0     2425 2024-05-27 13:53:59.394959 dspy_ai-2.5.0rc2/dspy/retrieve/ragatouille_rm.py
--rw-r--r--   0        0        0     1443 2024-05-29 20:05:59.698981 dspy_ai-2.5.0rc2/dspy/retrieve/retrieve.py
--rw-r--r--   0        0        0     4575 2024-05-27 13:53:59.395131 dspy_ai-2.5.0rc2/dspy/retrieve/snowflake_rm.py
--rw-r--r--   0        0        0     5923 2024-05-27 13:53:59.395244 dspy_ai-2.5.0rc2/dspy/retrieve/vectara_rm.py
--rw-r--r--   0        0        0     4373 2024-05-29 20:05:59.699111 dspy_ai-2.5.0rc2/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0        0        0      438 2024-02-10 21:45:26.556459 dspy_ai-2.5.0rc2/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0        0        0     1678 2024-04-05 16:07:52.859233 dspy_ai-2.5.0rc2/dspy/retrieve/you_rm.py
--rw-r--r--   0        0        0       46 2024-01-27 20:16:47.217346 dspy_ai-2.5.0rc2/dspy/signatures/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-05 16:07:52.859642 dspy_ai-2.5.0rc2/dspy/signatures/field.py
--rw-r--r--   0        0        0    14752 2024-05-29 20:05:59.699252 dspy_ai-2.5.0rc2/dspy/signatures/signature.py
--rw-r--r--   0        0        0      390 2024-04-05 16:07:52.860050 dspy_ai-2.5.0rc2/dspy/teleprompt/__init__.py
--rw-r--r--   0        0        0    11291 2024-05-29 20:05:59.699407 dspy_ai-2.5.0rc2/dspy/teleprompt/bootstrap.py
--rw-r--r--   0        0        0    17725 2024-05-29 20:05:59.699529 dspy_ai-2.5.0rc2/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0        0        0     1359 2024-04-05 16:07:52.860514 dspy_ai-2.5.0rc2/dspy/teleprompt/ensemble.py
--rw-r--r--   0        0        0     6292 2024-04-05 16:07:52.860625 dspy_ai-2.5.0rc2/dspy/teleprompt/finetune.py
--rw-r--r--   0        0        0     1002 2024-05-27 13:53:59.396186 dspy_ai-2.5.0rc2/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0        0        0    31024 2024-05-29 20:05:59.699712 dspy_ai-2.5.0rc2/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0        0        0     8130 2024-05-27 13:53:59.396477 dspy_ai-2.5.0rc2/dspy/teleprompt/random_search.py
--rw-r--r--   0        0        0     2673 2024-05-27 13:53:59.396900 dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt.py
--rw-r--r--   0        0        0     3878 2024-04-05 16:07:52.861256 dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0        0        0    11876 2024-04-05 16:07:52.861442 dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0        0        0       57 2024-04-05 16:07:52.861522 dspy_ai-2.5.0rc2/dspy/teleprompt/teleprompt.py
--rw-r--r--   0        0        0     3206 2024-05-27 13:53:59.397045 dspy_ai-2.5.0rc2/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0        0        0      948 2024-04-05 16:07:52.861703 dspy_ai-2.5.0rc2/dspy/teleprompt/vanilla.py
--rw-r--r--   0        0        0       46 2024-05-27 13:53:59.397185 dspy_ai-2.5.0rc2/dspy/utils/__init__.py
--rw-r--r--   0        0        0     7299 2024-05-29 20:05:59.699849 dspy_ai-2.5.0rc2/dspy/utils/dummies.py
--rw-r--r--   0        0        0     3193 2024-05-27 13:53:59.397403 dspy_ai-2.5.0rc2/dspy/utils/logging.py
--rw-r--r--   0        0        0     7736 2024-05-29 20:12:43.027428 dspy_ai-2.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0    38956 1970-01-01 00:00:00.000000 dspy_ai-2.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-01-27 20:16:46.845164 dspy_ai-2.5.0rc3/LICENSE
+-rw-r--r--   0        0        0    35950 2024-05-27 13:53:59.380701 dspy_ai-2.5.0rc3/README.md
+-rw-r--r--   0        0        0     1532 2024-04-05 16:07:52.842000 dspy_ai-2.5.0rc3/dsp/__init__.py
+-rw-r--r--   0        0        0        1 2024-01-27 20:16:47.211998 dspy_ai-2.5.0rc3/dsp/evaluation/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-05 16:07:52.842228 dspy_ai-2.5.0rc3/dsp/evaluation/utils.py
+-rw-r--r--   0        0        0      862 2024-05-27 13:53:59.386966 dspy_ai-2.5.0rc3/dsp/modules/__init__.py
+-rw-r--r--   0        0        0     4456 2024-05-29 20:05:59.695240 dspy_ai-2.5.0rc3/dsp/modules/anthropic.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:05:59.695266 dspy_ai-2.5.0rc3/dsp/modules/aws_lm.py
+-rw-r--r--   0        0        0    10409 2024-05-27 13:53:59.387252 dspy_ai-2.5.0rc3/dsp/modules/aws_models.py
+-rw-r--r--   0        0        0     5464 2024-05-27 13:53:59.387321 dspy_ai-2.5.0rc3/dsp/modules/aws_providers.py
+-rw-r--r--   0        0        0     9756 2024-05-27 13:53:59.387706 dspy_ai-2.5.0rc3/dsp/modules/azure_openai.py
+-rw-r--r--   0        0        0     3143 2024-05-29 20:05:59.695404 dspy_ai-2.5.0rc3/dsp/modules/azurecognitivesearch.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:05:59.695428 dspy_ai-2.5.0rc3/dsp/modules/bedrock.py
+-rw-r--r--   0        0        0     1018 2024-05-29 20:05:59.695535 dspy_ai-2.5.0rc3/dsp/modules/cache_utils.py
+-rw-r--r--   0        0        0     3008 2024-04-05 16:07:52.843839 dspy_ai-2.5.0rc3/dsp/modules/clarifai.py
+-rw-r--r--   0        0        0     4030 2024-05-27 13:53:59.388176 dspy_ai-2.5.0rc3/dsp/modules/cloudflare.py
+-rw-r--r--   0        0        0     4523 2024-05-29 20:05:59.695644 dspy_ai-2.5.0rc3/dsp/modules/cohere.py
+-rw-r--r--   0        0        0     2156 2024-04-05 16:07:52.844059 dspy_ai-2.5.0rc3/dsp/modules/colbertv2.py
+-rw-r--r--   0        0        0     5304 2024-05-29 20:05:59.695752 dspy_ai-2.5.0rc3/dsp/modules/databricks.py
+-rw-r--r--   0        0        0     3788 2024-05-27 13:53:59.388459 dspy_ai-2.5.0rc3/dsp/modules/dummy_lm.py
+-rw-r--r--   0        0        0       26 2024-01-27 20:16:47.212462 dspy_ai-2.5.0rc3/dsp/modules/finetuning/__init__.py
+-rw-r--r--   0        0        0    15071 2024-04-05 16:07:52.844302 dspy_ai-2.5.0rc3/dsp/modules/finetuning/finetune_hf.py
+-rw-r--r--   0        0        0     4552 2024-04-05 16:07:52.844428 dspy_ai-2.5.0rc3/dsp/modules/google.py
+-rw-r--r--   0        0        0     5992 2024-05-27 13:53:59.388532 dspy_ai-2.5.0rc3/dsp/modules/googlevertexai.py
+-rw-r--r--   0        0        0     8870 2024-05-29 20:05:59.695879 dspy_ai-2.5.0rc3/dsp/modules/gpt3.py
+-rw-r--r--   0        0        0     4859 2024-05-27 13:53:59.388786 dspy_ai-2.5.0rc3/dsp/modules/groq_client.py
+-rw-r--r--   0        0        0     8119 2024-05-27 13:53:59.388896 dspy_ai-2.5.0rc3/dsp/modules/hf.py
+-rw-r--r--   0        0        0    18878 2024-05-29 20:05:59.695996 dspy_ai-2.5.0rc3/dsp/modules/hf_client.py
+-rw-r--r--   0        0        0     2087 2024-01-27 20:16:47.212938 dspy_ai-2.5.0rc3/dsp/modules/hf_server.py
+-rw-r--r--   0        0        0     4421 2024-05-29 20:05:59.696107 dspy_ai-2.5.0rc3/dsp/modules/lm.py
+-rw-r--r--   0        0        0     3655 2024-05-27 13:53:59.389199 dspy_ai-2.5.0rc3/dsp/modules/mistral.py
+-rw-r--r--   0        0        0     7119 2024-05-27 13:53:59.389305 dspy_ai-2.5.0rc3/dsp/modules/ollama.py
+-rw-r--r--   0        0        0     5322 2024-05-27 13:53:59.389387 dspy_ai-2.5.0rc3/dsp/modules/premai.py
+-rw-r--r--   0        0        0     3152 2024-04-05 16:07:52.845476 dspy_ai-2.5.0rc3/dsp/modules/pyserini.py
+-rw-r--r--   0        0        0      693 2024-04-05 16:07:52.845555 dspy_ai-2.5.0rc3/dsp/modules/sbert.py
+-rw-r--r--   0        0        0    10179 2024-05-27 13:53:59.389530 dspy_ai-2.5.0rc3/dsp/modules/sentence_vectorizer.py
+-rw-r--r--   0        0        0     5330 2024-05-27 13:53:59.389604 dspy_ai-2.5.0rc3/dsp/modules/snowflake.py
+-rw-r--r--   0        0        0     4463 2024-05-27 13:53:59.389666 dspy_ai-2.5.0rc3/dsp/modules/watsonx.py
+-rw-r--r--   0        0        0      145 2024-04-05 16:07:52.845754 dspy_ai-2.5.0rc3/dsp/primitives/__init__.py
+-rw-r--r--   0        0        0     5185 2024-04-05 16:07:52.845851 dspy_ai-2.5.0rc3/dsp/primitives/compiler.py
+-rw-r--r--   0        0        0     5789 2024-04-05 16:07:52.845949 dspy_ai-2.5.0rc3/dsp/primitives/demonstrate.py
+-rw-r--r--   0        0        0     2471 2024-04-05 16:07:52.846037 dspy_ai-2.5.0rc3/dsp/primitives/inspect.py
+-rw-r--r--   0        0        0     8949 2024-05-29 20:05:59.696236 dspy_ai-2.5.0rc3/dsp/primitives/predict.py
+-rw-r--r--   0        0        0     1439 2024-04-05 16:07:52.846337 dspy_ai-2.5.0rc3/dsp/primitives/primitives.py
+-rw-r--r--   0        0        0     2735 2024-05-29 20:05:59.696332 dspy_ai-2.5.0rc3/dsp/primitives/search.py
+-rw-r--r--   0        0        0       76 2024-04-05 16:07:52.846520 dspy_ai-2.5.0rc3/dsp/templates/__init__.py
+-rw-r--r--   0        0        0    10226 2024-04-05 16:07:52.846745 dspy_ai-2.5.0rc3/dsp/templates/template_v2.py
+-rw-r--r--   0        0        0     2334 2024-04-05 16:07:52.846834 dspy_ai-2.5.0rc3/dsp/templates/template_v3.py
+-rw-r--r--   0        0        0     1900 2024-04-05 16:07:52.846926 dspy_ai-2.5.0rc3/dsp/templates/utils.py
+-rw-r--r--   0        0        0      123 2024-04-05 16:07:52.847031 dspy_ai-2.5.0rc3/dsp/utils/__init__.py
+-rw-r--r--   0        0        0     4903 2024-04-05 16:07:52.847141 dspy_ai-2.5.0rc3/dsp/utils/ann_utils.py
+-rw-r--r--   0        0        0     7110 2024-04-05 16:07:52.847247 dspy_ai-2.5.0rc3/dsp/utils/dpr.py
+-rw-r--r--   0        0        0     5933 2024-04-05 16:07:52.847337 dspy_ai-2.5.0rc3/dsp/utils/metrics.py
+-rw-r--r--   0        0        0     3279 2024-05-29 20:05:59.696435 dspy_ai-2.5.0rc3/dsp/utils/settings.py
+-rw-r--r--   0        0        0     2828 2024-04-05 16:07:52.847535 dspy_ai-2.5.0rc3/dsp/utils/settings_v2.py
+-rw-r--r--   0        0        0     5623 2024-04-05 16:07:52.847653 dspy_ai-2.5.0rc3/dsp/utils/utils.py
+-rw-r--r--   0        0        0     1204 2024-05-29 20:05:59.696560 dspy_ai-2.5.0rc3/dspy/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-05 16:07:52.848121 dspy_ai-2.5.0rc3/dspy/datasets/__init__.py
+-rw-r--r--   0        0        0     2986 2024-04-05 16:07:52.848222 dspy_ai-2.5.0rc3/dspy/datasets/colors.py
+-rw-r--r--   0        0        0     5162 2024-05-29 20:05:59.696687 dspy_ai-2.5.0rc3/dspy/datasets/dataloader.py
+-rw-r--r--   0        0        0     4098 2024-04-05 16:07:52.848414 dspy_ai-2.5.0rc3/dspy/datasets/dataset.py
+-rw-r--r--   0        0        0     2618 2024-04-05 16:07:52.848498 dspy_ai-2.5.0rc3/dspy/datasets/gsm8k.py
+-rw-r--r--   0        0        0     3286 2024-04-05 16:07:52.848598 dspy_ai-2.5.0rc3/dspy/datasets/hotpotqa.py
+-rw-r--r--   0        0        0      127 2024-04-05 16:07:52.848699 dspy_ai-2.5.0rc3/dspy/evaluate/__init__.py
+-rw-r--r--   0        0        0     1421 2024-04-05 16:07:52.848822 dspy_ai-2.5.0rc3/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0        0        0    11414 2024-05-27 13:53:59.390403 dspy_ai-2.5.0rc3/dspy/evaluate/evaluate.py
+-rw-r--r--   0        0        0      882 2024-04-05 16:07:52.852527 dspy_ai-2.5.0rc3/dspy/evaluate/metrics.py
+-rw-r--r--   0        0        0       57 2024-04-05 16:07:52.852610 dspy_ai-2.5.0rc3/dspy/experimental/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-05 16:07:52.852700 dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0        0        0      834 2024-04-05 16:07:52.852759 dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0        0        0      527 2024-04-05 16:07:52.852825 dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0        0        0     5543 2024-04-05 16:07:52.852897 dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0        0        0     9567 2024-05-29 20:05:59.696817 dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0        0        0      599 2024-04-05 16:07:52.853143 dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0        0        0     4237 2024-05-27 13:53:59.390647 dspy_ai-2.5.0rc3/dspy/experimental/synthetic_data.py
+-rw-r--r--   0        0        0       94 2024-04-05 16:07:52.853820 dspy_ai-2.5.0rc3/dspy/functional/__init__.py
+-rw-r--r--   0        0        0    20120 2024-05-29 20:05:59.696945 dspy_ai-2.5.0rc3/dspy/functional/functional.py
+-rw-r--r--   0        0        0       47 2024-05-29 20:05:59.697246 dspy_ai-2.5.0rc3/dspy/modeling/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-29 20:05:59.697326 dspy_ai-2.5.0rc3/dspy/modeling/backends/__init__.py
+-rw-r--r--   0        0        0     4724 2024-05-29 20:05:59.697392 dspy_ai-2.5.0rc3/dspy/modeling/backends/base.py
+-rw-r--r--   0        0        0     3777 2024-05-29 20:05:59.697443 dspy_ai-2.5.0rc3/dspy/modeling/backends/json.py
+-rw-r--r--   0        0        0     7459 2024-05-29 20:05:59.697507 dspy_ai-2.5.0rc3/dspy/modeling/backends/text.py
+-rw-r--r--   0        0        0      348 2024-04-05 16:07:52.854456 dspy_ai-2.5.0rc3/dspy/predict/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-29 20:05:59.697772 dspy_ai-2.5.0rc3/dspy/predict/aggregation.py
+-rw-r--r--   0        0        0     3589 2024-04-05 16:07:52.854648 dspy_ai-2.5.0rc3/dspy/predict/chain_of_thought.py
+-rw-r--r--   0        0        0     1527 2024-04-05 16:07:52.854742 dspy_ai-2.5.0rc3/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0        0        0     1133 2024-05-27 13:53:59.392833 dspy_ai-2.5.0rc3/dspy/predict/knn.py
+-rw-r--r--   0        0        0     6129 2024-05-27 13:53:59.392953 dspy_ai-2.5.0rc3/dspy/predict/langchain.py
+-rw-r--r--   0        0        0     1659 2024-04-05 16:07:52.855060 dspy_ai-2.5.0rc3/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0        0        0       58 2024-01-27 20:16:47.215842 dspy_ai-2.5.0rc3/dspy/predict/parameter.py
+-rw-r--r--   0        0        0     7252 2024-05-29 20:05:59.697915 dspy_ai-2.5.0rc3/dspy/predict/predict.py
+-rw-r--r--   0        0        0     7598 2024-05-29 20:05:59.698038 dspy_ai-2.5.0rc3/dspy/predict/program_of_thought.py
+-rw-r--r--   0        0        0     4614 2024-05-27 13:53:59.393278 dspy_ai-2.5.0rc3/dspy/predict/react.py
+-rw-r--r--   0        0        0     3115 2024-05-29 20:05:59.698147 dspy_ai-2.5.0rc3/dspy/predict/retry.py
+-rw-r--r--   0        0        0      132 2024-04-05 16:07:52.855575 dspy_ai-2.5.0rc3/dspy/primitives/__init__.py
+-rw-r--r--   0        0        0    11319 2024-05-27 13:53:59.393559 dspy_ai-2.5.0rc3/dspy/primitives/assertions.py
+-rw-r--r--   0        0        0     7779 2024-01-27 20:16:47.216399 dspy_ai-2.5.0rc3/dspy/primitives/box.py
+-rw-r--r--   0        0        0     3416 2024-05-29 20:05:59.698251 dspy_ai-2.5.0rc3/dspy/primitives/example.py
+-rw-r--r--   0        0        0     3831 2024-05-27 13:53:59.393756 dspy_ai-2.5.0rc3/dspy/primitives/module.py
+-rw-r--r--   0        0        0     4836 2024-05-29 20:05:59.698359 dspy_ai-2.5.0rc3/dspy/primitives/prediction.py
+-rw-r--r--   0        0        0     3366 2024-04-05 16:07:52.856229 dspy_ai-2.5.0rc3/dspy/primitives/program.py
+-rw-r--r--   0        0        0    25710 2024-04-05 16:07:52.856677 dspy_ai-2.5.0rc3/dspy/primitives/python_interpreter.py
+-rw-r--r--   0        0        0       30 2024-01-27 20:16:47.216808 dspy_ai-2.5.0rc3/dspy/retrieve/__init__.py
+-rw-r--r--   0        0        0    17405 2024-05-27 13:53:59.393937 dspy_ai-2.5.0rc3/dspy/retrieve/azureaisearch_rm.py
+-rw-r--r--   0        0        0     5683 2024-05-29 20:05:59.698525 dspy_ai-2.5.0rc3/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0        0        0     3264 2024-05-29 20:05:59.698629 dspy_ai-2.5.0rc3/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0        0        0     6604 2024-05-27 13:53:59.394297 dspy_ai-2.5.0rc3/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0        0        0     3804 2024-05-29 20:05:59.698742 dspy_ai-2.5.0rc3/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0        0        0     6605 2024-05-27 13:53:59.394532 dspy_ai-2.5.0rc3/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0        0        0     2937 2024-05-27 13:53:59.394597 dspy_ai-2.5.0rc3/dspy/retrieve/llama_index_rm.py
+-rw-r--r--   0        0        0     3459 2024-04-05 16:07:52.857777 dspy_ai-2.5.0rc3/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0        0        0     3998 2024-05-27 13:53:59.394660 dspy_ai-2.5.0rc3/dspy/retrieve/milvus_rm.py
+-rw-r--r--   0        0        0     3774 2024-04-05 16:07:52.857887 dspy_ai-2.5.0rc3/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0        0        0     6213 2024-04-05 16:07:52.857964 dspy_ai-2.5.0rc3/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0        0        0     5904 2024-05-29 20:05:59.698885 dspy_ai-2.5.0rc3/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0        0        0    10476 2024-04-05 16:07:52.858267 dspy_ai-2.5.0rc3/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0        0        0     4951 2024-05-27 13:53:59.394882 dspy_ai-2.5.0rc3/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0        0        0     2425 2024-05-27 13:53:59.394959 dspy_ai-2.5.0rc3/dspy/retrieve/ragatouille_rm.py
+-rw-r--r--   0        0        0     1443 2024-05-29 20:05:59.698981 dspy_ai-2.5.0rc3/dspy/retrieve/retrieve.py
+-rw-r--r--   0        0        0     4575 2024-05-27 13:53:59.395131 dspy_ai-2.5.0rc3/dspy/retrieve/snowflake_rm.py
+-rw-r--r--   0        0        0     5923 2024-05-27 13:53:59.395244 dspy_ai-2.5.0rc3/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0        0        0     4373 2024-05-29 20:05:59.699111 dspy_ai-2.5.0rc3/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0        0        0      438 2024-02-10 21:45:26.556459 dspy_ai-2.5.0rc3/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0        0        0     1678 2024-04-05 16:07:52.859233 dspy_ai-2.5.0rc3/dspy/retrieve/you_rm.py
+-rw-r--r--   0        0        0       46 2024-01-27 20:16:47.217346 dspy_ai-2.5.0rc3/dspy/signatures/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-05 16:07:52.859642 dspy_ai-2.5.0rc3/dspy/signatures/field.py
+-rw-r--r--   0        0        0    14752 2024-05-29 20:05:59.699252 dspy_ai-2.5.0rc3/dspy/signatures/signature.py
+-rw-r--r--   0        0        0      390 2024-04-05 16:07:52.860050 dspy_ai-2.5.0rc3/dspy/teleprompt/__init__.py
+-rw-r--r--   0        0        0    11291 2024-05-29 20:05:59.699407 dspy_ai-2.5.0rc3/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0        0        0    17725 2024-05-29 20:05:59.699529 dspy_ai-2.5.0rc3/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0        0        0     1359 2024-04-05 16:07:52.860514 dspy_ai-2.5.0rc3/dspy/teleprompt/ensemble.py
+-rw-r--r--   0        0        0     6292 2024-04-05 16:07:52.860625 dspy_ai-2.5.0rc3/dspy/teleprompt/finetune.py
+-rw-r--r--   0        0        0     1002 2024-05-27 13:53:59.396186 dspy_ai-2.5.0rc3/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0        0        0    31024 2024-05-29 20:05:59.699712 dspy_ai-2.5.0rc3/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0        0        0     8130 2024-05-27 13:53:59.396477 dspy_ai-2.5.0rc3/dspy/teleprompt/random_search.py
+-rw-r--r--   0        0        0     2673 2024-05-27 13:53:59.396900 dspy_ai-2.5.0rc3/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0        0        0     3878 2024-04-05 16:07:52.861256 dspy_ai-2.5.0rc3/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0        0        0    11876 2024-04-05 16:07:52.861442 dspy_ai-2.5.0rc3/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0        0        0       57 2024-04-05 16:07:52.861522 dspy_ai-2.5.0rc3/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0        0        0     3206 2024-05-27 13:53:59.397045 dspy_ai-2.5.0rc3/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0        0        0      948 2024-04-05 16:07:52.861703 dspy_ai-2.5.0rc3/dspy/teleprompt/vanilla.py
+-rw-r--r--   0        0        0       46 2024-05-27 13:53:59.397185 dspy_ai-2.5.0rc3/dspy/utils/__init__.py
+-rw-r--r--   0        0        0     7299 2024-05-29 20:05:59.699849 dspy_ai-2.5.0rc3/dspy/utils/dummies.py
+-rw-r--r--   0        0        0     3193 2024-05-27 13:53:59.397403 dspy_ai-2.5.0rc3/dspy/utils/logging.py
+-rw-r--r--   0        0        0     7757 2024-06-01 20:41:37.926972 dspy_ai-2.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    38956 1970-01-01 00:00:00.000000 dspy_ai-2.5.0rc3/PKG-INFO
```

### Comparing `dspy_ai-2.5.0rc2/LICENSE` & `dspy_ai-2.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/README.md` & `dspy_ai-2.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/__init__.py` & `dspy_ai-2.5.0rc3/dspy/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/datasets/colors.py` & `dspy_ai-2.5.0rc3/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/datasets/dataloader.py` & `dspy_ai-2.5.0rc3/dspy/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/datasets/dataset.py` & `dspy_ai-2.5.0rc3/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/datasets/gsm8k.py` & `dspy_ai-2.5.0rc3/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/datasets/hotpotqa.py` & `dspy_ai-2.5.0rc3/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/evaluate/auto_evaluation.py` & `dspy_ai-2.5.0rc3/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/evaluate/evaluate.py` & `dspy_ai-2.5.0rc3/dspy/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/evaluate/metrics.py` & `dspy_ai-2.5.0rc3/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/config.py` & `dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/signatures.py` & `dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/synthesizer.py` & `dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/synthesizer.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/utils.py` & `dspy_ai-2.5.0rc3/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/experimental/synthetic_data.py` & `dspy_ai-2.5.0rc3/dspy/experimental/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/functional/functional.py` & `dspy_ai-2.5.0rc3/dspy/functional/functional.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/modeling/backends/base.py` & `dspy_ai-2.5.0rc3/dspy/modeling/backends/base.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/modeling/backends/json.py` & `dspy_ai-2.5.0rc3/dspy/modeling/backends/json.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/modeling/backends/text.py` & `dspy_ai-2.5.0rc3/dspy/modeling/backends/text.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/aggregation.py` & `dspy_ai-2.5.0rc3/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought.py` & `dspy_ai-2.5.0rc3/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought_with_hint.py` & `dspy_ai-2.5.0rc3/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/knn.py` & `dspy_ai-2.5.0rc3/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/langchain.py` & `dspy_ai-2.5.0rc3/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/multi_chain_comparison.py` & `dspy_ai-2.5.0rc3/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/predict.py` & `dspy_ai-2.5.0rc3/dspy/predict/predict.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/program_of_thought.py` & `dspy_ai-2.5.0rc3/dspy/predict/program_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/react.py` & `dspy_ai-2.5.0rc3/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/predict/retry.py` & `dspy_ai-2.5.0rc3/dspy/predict/retry.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/assertions.py` & `dspy_ai-2.5.0rc3/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/box.py` & `dspy_ai-2.5.0rc3/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/example.py` & `dspy_ai-2.5.0rc3/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/module.py` & `dspy_ai-2.5.0rc3/dspy/primitives/module.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/prediction.py` & `dspy_ai-2.5.0rc3/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/program.py` & `dspy_ai-2.5.0rc3/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/primitives/python_interpreter.py` & `dspy_ai-2.5.0rc3/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/azureaisearch_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/azureaisearch_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/chromadb_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/chromadb_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/clarifai_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/clarifai_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/databricks_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/deeplake_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/deeplake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/faiss_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/faiss_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/llama_index_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/llama_index_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/marqo_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/milvus_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/milvus_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/mongodb_atlas_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/neo4j_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/pgvector_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/pgvector_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/pinecone_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/qdrant_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/qdrant_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/ragatouille_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/ragatouille_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/retrieve.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/retrieve.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/snowflake_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/snowflake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/vectara_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/weaviate_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/weaviate_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/retrieve/you_rm.py` & `dspy_ai-2.5.0rc3/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/signatures/field.py` & `dspy_ai-2.5.0rc3/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/signatures/signature.py` & `dspy_ai-2.5.0rc3/dspy/signatures/signature.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/bootstrap.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/copro_optimizer.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/copro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/ensemble.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/finetune.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/knn_fewshot.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/knn_fewshot.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/mipro_optimizer.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/mipro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/random_search.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/random_search.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_bayesian.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_typed.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/teleprompt_optuna.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/teleprompt_optuna.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/teleprompt/vanilla.py` & `dspy_ai-2.5.0rc3/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/utils/dummies.py` & `dspy_ai-2.5.0rc3/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/dspy/utils/logging.py` & `dspy_ai-2.5.0rc3/dspy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc2/pyproject.toml` & `dspy_ai-2.5.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.5.0rc2"
+version = "2.5.0rc3"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.13"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -64,25 +64,25 @@
 fastembed = ["fastembed>=0.2.0"]
 
 [project.urls]
 homepage = "https://github.com/stanfordnlp/dspy"
 
 [tool.poetry]
 name = "dspy-ai"
-version = "2.5.0rc2"
+version = "2.5.0rc3"
 description = "DSPy: The framework for programming—not prompting—foundation models"
 authors = ["Omar Khattab <okhattab@stanford.edu>"]
 maintainers = ["Cyrus Nouroozi <cyrus@edendaolab.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stanfordnlp/dspy"
 repository = "https://github.com/stanfordnlp/dspy"
 # documentation = "https://dspy-ai.readthedocs.io"
 keywords = ["dspy", "ai", "language models", "llm", "openai"]
-packages = [{ include = "dspy" }]
+packages = [{ include = "dspy" }, { include = "dsp" }]
 
 # may be a bit much
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pydantic = "^2.0"
 backoff = "^2.2.1"
 joblib = "^1.3.2"
```

### Comparing `dspy_ai-2.5.0rc2/PKG-INFO` & `dspy_ai-2.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.5.0rc2
+Version: 2.5.0rc3
 Summary: DSPy: The framework for programming—not prompting—foundation models
 Home-page: https://github.com/stanfordnlp/dspy
 License: MIT
 Keywords: dspy,ai,language models,llm,openai
 Author: Omar Khattab
 Author-email: okhattab@stanford.edu
 Maintainer: Cyrus Nouroozi
```

