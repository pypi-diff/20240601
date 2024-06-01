# Comparing `tmp/athina-1.4.1.tar.gz` & `tmp/athina-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina-1.4.1.tar", max compression
+gzip compressed data, was "athina-1.4.2.tar", max compression
```

## Comparing `athina-1.4.1.tar` & `athina-1.4.2.tar`

### file list

```diff
@@ -1,155 +1,155 @@
--rw-r--r--   0        0        0     8595 2024-04-07 19:50:25.988814 athina-1.4.1/README.md
--rw-r--r--   0        0        0      169 2024-04-07 19:50:25.988910 athina-1.4.1/athina/__init__.py
--rw-r--r--   0        0        0        0 2023-11-23 04:12:26.907515 athina-1.4.1/athina/cli/__init__.py
--rw-r--r--   0        0        0     5390 2024-04-07 19:50:25.989095 athina-1.4.1/athina/cli/cli.py
--rw-r--r--   0        0        0        0 2023-12-15 12:51:50.234650 athina-1.4.1/athina/constants/__init__.py
--rw-r--r--   0        0        0      517 2024-01-13 20:48:45.788836 athina-1.4.1/athina/constants/messages.py
--rw-r--r--   0        0        0       72 2024-05-16 22:07:31.607654 athina-1.4.1/athina/datasets/__init__.py
--rw-r--r--   0        0        0   218970 2024-04-07 19:50:25.989477 athina-1.4.1/athina/datasets/conversations.json
--rw-r--r--   0        0        0     3315 2024-05-29 20:39:08.688644 athina-1.4.1/athina/datasets/dataset.py
--rw-r--r--   0        0        0     3355 2023-12-21 07:47:22.703846 athina-1.4.1/athina/datasets/summarization_sample.py
--rw-r--r--   0        0        0     2675 2024-04-07 19:50:25.989613 athina-1.4.1/athina/datasets/yc_query_mini.py
--rw-r--r--   0        0        0        0 2023-11-27 22:10:49.443729 athina-1.4.1/athina/errors/__init__.py
--rw-r--r--   0        0        0      801 2024-04-07 19:50:25.989725 athina-1.4.1/athina/errors/exceptions.py
--rw-r--r--   0        0        0     5016 2024-05-29 18:43:09.546765 athina-1.4.1/athina/evals/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-16 22:07:33.542477 athina-1.4.1/athina/evals/base_evaluator.py
--rw-r--r--   0        0        0     4259 2024-05-16 22:07:33.542877 athina-1.4.1/athina/evals/conversation/conversation_coherence/evaluator.py
--rw-r--r--   0        0        0     1198 2024-04-07 19:50:25.990313 athina-1.4.1/athina/evals/conversation/conversation_coherence/prompt.py
--rw-r--r--   0        0        0     4414 2024-05-16 22:07:33.543237 athina-1.4.1/athina/evals/conversation/conversation_resolution/evaluator.py
--rw-r--r--   0        0        0     1104 2024-04-07 19:50:25.990577 athina-1.4.1/athina/evals/conversation/conversation_resolution/prompt.py
--rw-r--r--   0        0        0     2984 2024-05-29 18:43:09.547175 athina-1.4.1/athina/evals/eval_type.py
--rw-r--r--   0        0        0        0 2024-01-14 09:48:35.090076 athina-1.4.1/athina/evals/function/__init__.py
--rw-r--r--   0        0        0     3780 2024-05-16 22:07:33.544581 athina-1.4.1/athina/evals/function/function_evaluator.py
--rw-r--r--   0        0        0    20171 2024-05-29 18:43:09.547541 athina-1.4.1/athina/evals/function/functions.py
--rw-r--r--   0        0        0    11066 2024-05-29 18:43:09.547874 athina-1.4.1/athina/evals/function/wrapper.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.991128 athina-1.4.1/athina/evals/grounded/__init__.py
--rw-r--r--   0        0        0     4298 2024-05-16 22:07:33.544879 athina-1.4.1/athina/evals/grounded/grounded_evaluator.py
--rw-r--r--   0        0        0     4178 2024-04-07 19:50:25.991409 athina-1.4.1/athina/evals/grounded/similarity.py
--rw-r--r--   0        0        0     1708 2024-04-07 19:50:25.991495 athina-1.4.1/athina/evals/grounded/wrapper.py
--rw-r--r--   0        0        0     3362 2024-05-29 18:43:09.548081 athina-1.4.1/athina/evals/guardrails/correct_language/evaluator.py
--rw-r--r--   0        0        0     2813 2024-05-29 18:43:09.548263 athina-1.4.1/athina/evals/guardrails/detect_pii/evaluator.py
--rw-r--r--   0        0        0     3041 2024-05-16 22:07:33.545188 athina-1.4.1/athina/evals/guardrails/gibberish_text/evaluator.py
--rw-r--r--   0        0        0     2694 2024-05-29 18:43:09.548434 athina-1.4.1/athina/evals/guardrails/no_secrets_present/evaluator.py
--rw-r--r--   0        0        0     3134 2024-05-29 18:43:09.548628 athina-1.4.1/athina/evals/guardrails/politeness_check/evaluator.py
--rw-r--r--   0        0        0     2649 2024-05-29 18:43:09.548802 athina-1.4.1/athina/evals/guardrails/profanity_free/evaluator.py
--rw-r--r--   0        0        0     2826 2024-05-29 18:43:09.548978 athina-1.4.1/athina/evals/guardrails/reading_time/evaluator.py
--rw-r--r--   0        0        0     3772 2024-05-29 18:43:09.549157 athina-1.4.1/athina/evals/guardrails/restrict_to_topic/evaluator.py
--rw-r--r--   0        0        0     3797 2024-05-16 22:07:33.545707 athina-1.4.1/athina/evals/guardrails/sensitive_topics/evaluator.py
--rw-r--r--   0        0        0     2965 2024-05-16 22:07:33.545880 athina-1.4.1/athina/evals/guardrails/sfw/evaluator.py
--rw-r--r--   0        0        0     2850 2024-05-29 18:43:09.549328 athina-1.4.1/athina/evals/guardrails/toxic_language/evaluator.py
--rw-r--r--   0        0        0     3173 2024-05-29 18:43:09.549507 athina-1.4.1/athina/evals/guardrails/unusual_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2023-11-22 10:22:53.580396 athina-1.4.1/athina/evals/llm/__init__.py
--rw-r--r--   0        0        0        0 2023-11-22 14:42:09.270085 athina-1.4.1/athina/evals/llm/context_contains_enough_information/__init__.py
--rw-r--r--   0        0        0     3004 2024-05-16 22:07:33.546103 athina-1.4.1/athina/evals/llm/context_contains_enough_information/evaluator.py
--rw-r--r--   0        0        0     1867 2023-11-25 19:30:39.481282 athina-1.4.1/athina/evals/llm/context_contains_enough_information/examples.py
--rw-r--r--   0        0        0        0 2024-01-11 20:19:05.567209 athina-1.4.1/athina/evals/llm/custom_prompt/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-28 23:41:09.150533 athina-1.4.1/athina/evals/llm/custom_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2023-11-22 10:23:25.867325 athina-1.4.1/athina/evals/llm/does_response_answer_query/__init__.py
--rw-r--r--   0        0        0     2632 2024-04-07 19:50:25.992212 athina-1.4.1/athina/evals/llm/does_response_answer_query/evaluator.py
--rw-r--r--   0        0        0     1186 2023-11-25 19:30:56.907120 athina-1.4.1/athina/evals/llm/does_response_answer_query/examples.py
--rw-r--r--   0        0        0     1238 2023-11-24 19:58:55.424197 athina-1.4.1/athina/evals/llm/example.py
--rw-r--r--   0        0        0        0 2023-11-22 14:42:13.917099 athina-1.4.1/athina/evals/llm/faithfulness/__init__.py
--rw-r--r--   0        0        0     2599 2024-04-07 19:50:25.992315 athina-1.4.1/athina/evals/llm/faithfulness/evaluator.py
--rw-r--r--   0        0        0     1335 2023-11-24 19:56:49.591982 athina-1.4.1/athina/evals/llm/faithfulness/examples.py
--rw-r--r--   0        0        0        0 2024-01-11 20:19:05.567792 athina-1.4.1/athina/evals/llm/grading_criteria/__init__.py
--rw-r--r--   0        0        0     2209 2024-05-16 22:07:33.546656 athina-1.4.1/athina/evals/llm/grading_criteria/evaluator.py
--rw-r--r--   0        0        0     5821 2024-04-07 19:50:25.992563 athina-1.4.1/athina/evals/llm/groundedness/evaluator.py
--rw-r--r--   0        0        0     1601 2024-04-07 19:50:25.992633 athina-1.4.1/athina/evals/llm/groundedness/prompt.py
--rw-r--r--   0        0        0     4982 2024-05-16 22:07:31.609011 athina-1.4.1/athina/evals/llm/llm_evaluator.py
--rw-r--r--   0        0        0    10915 2024-04-07 19:50:25.992910 athina-1.4.1/athina/evals/llm/summary_accuracy/evaluator.py
--rw-r--r--   0        0        0        0 2024-01-14 09:48:35.092826 athina-1.4.1/athina/evals/ragas/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.992937 athina-1.4.1/athina/evals/ragas/answer_correctness/__init__.py
--rw-r--r--   0        0        0     2383 2024-04-07 19:50:25.993020 athina-1.4.1/athina/evals/ragas/answer_correctness/evaluator.py
--rw-r--r--   0        0        0        0 2024-01-14 09:48:35.092904 athina-1.4.1/athina/evals/ragas/answer_relevancy/__init__.py
--rw-r--r--   0        0        0     2441 2024-04-07 19:50:25.993135 athina-1.4.1/athina/evals/ragas/answer_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993157 athina-1.4.1/athina/evals/ragas/answer_semantic_similarity/__init__.py
--rw-r--r--   0        0        0     2440 2024-04-07 19:50:25.993233 athina-1.4.1/athina/evals/ragas/answer_semantic_similarity/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993256 athina-1.4.1/athina/evals/ragas/coherence/__init__.py
--rw-r--r--   0        0        0     2187 2024-05-16 22:07:31.609542 athina-1.4.1/athina/evals/ragas/coherence/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993368 athina-1.4.1/athina/evals/ragas/conciseness/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-16 22:07:31.610375 athina-1.4.1/athina/evals/ragas/conciseness/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993480 athina-1.4.1/athina/evals/ragas/context_precision/__init__.py
--rw-r--r--   0        0        0     2521 2024-05-16 22:07:31.610901 athina-1.4.1/athina/evals/ragas/context_precision/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993603 athina-1.4.1/athina/evals/ragas/context_recall/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-07 19:50:25.993697 athina-1.4.1/athina/evals/ragas/context_recall/evaluator.py
--rw-r--r--   0        0        0        0 2024-01-14 09:48:35.093237 athina-1.4.1/athina/evals/ragas/context_relevancy/__init__.py
--rw-r--r--   0        0        0     2159 2024-04-07 19:50:25.993803 athina-1.4.1/athina/evals/ragas/context_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993825 athina-1.4.1/athina/evals/ragas/faithfulness/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-07 19:50:25.993921 athina-1.4.1/athina/evals/ragas/faithfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.993945 athina-1.4.1/athina/evals/ragas/harmfulness/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-16 22:07:31.611355 athina-1.4.1/athina/evals/ragas/harmfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-04-07 19:50:25.994064 athina-1.4.1/athina/evals/ragas/maliciousness/__init__.py
--rw-r--r--   0        0        0     2127 2024-05-16 22:07:31.611816 athina-1.4.1/athina/evals/ragas/maliciousness/evaluator.py
--rw-r--r--   0        0        0     3298 2024-04-07 19:50:25.994247 athina-1.4.1/athina/evals/ragas/ragas_evaluator.py
--rw-r--r--   0        0        0     5154 2024-04-07 19:50:25.994437 athina-1.4.1/athina/evals/safety/content_moderation/evaluator.py
--rw-r--r--   0        0        0     3387 2024-05-16 22:07:33.547112 athina-1.4.1/athina/evals/safety/pii_detection/evaluator.py
--rw-r--r--   0        0        0     4370 2024-04-07 19:50:25.994697 athina-1.4.1/athina/evals/safety/prompt_injection/evaluator.py
--rw-r--r--   0        0        0      106 2024-04-07 19:50:25.994786 athina-1.4.1/athina/guard/exception.py
--rw-r--r--   0        0        0     1404 2024-04-07 19:50:25.994864 athina-1.4.1/athina/guard/guard.py
--rw-r--r--   0        0        0        0 2023-12-21 07:47:22.705649 athina-1.4.1/athina/helpers/__init__.py
--rw-r--r--   0        0        0     5739 2024-05-16 22:07:33.547311 athina-1.4.1/athina/helpers/athina_logging_helper.py
--rw-r--r--   0        0        0     1351 2024-04-07 19:50:25.995144 athina-1.4.1/athina/helpers/config.py
--rw-r--r--   0        0        0      122 2024-04-07 19:50:25.995236 athina-1.4.1/athina/helpers/constants.py
--rw-r--r--   0        0        0      790 2024-05-16 22:07:33.547486 athina-1.4.1/athina/helpers/dataset_helper.py
--rw-r--r--   0        0        0      172 2023-11-27 19:55:02.984766 athina-1.4.1/athina/helpers/eval_helper.py
--rw-r--r--   0        0        0      642 2024-01-14 09:48:35.094199 athina-1.4.1/athina/helpers/function_eval_util.py
--rw-r--r--   0        0        0     5152 2024-05-29 18:43:09.549922 athina-1.4.1/athina/helpers/get_evaluator.py
--rw-r--r--   0        0        0      135 2024-05-28 23:41:09.150851 athina-1.4.1/athina/helpers/jinja_helper.py
--rw-r--r--   0        0        0     2469 2024-05-24 10:38:54.005106 athina-1.4.1/athina/helpers/json.py
--rw-r--r--   0        0        0      403 2023-11-23 04:40:00.458953 athina-1.4.1/athina/helpers/kwparser.py
--rw-r--r--   0        0        0      894 2024-04-07 19:50:25.995488 athina-1.4.1/athina/helpers/loader_helper.py
--rw-r--r--   0        0        0     3051 2023-11-22 10:19:41.524239 athina-1.4.1/athina/helpers/logger.py
--rw-r--r--   0        0        0      265 2023-11-27 21:45:05.573359 athina-1.4.1/athina/helpers/package_helper.py
--rw-r--r--   0        0        0     5296 2024-04-07 19:50:25.995652 athina-1.4.1/athina/helpers/run_helper.py
--rw-r--r--   0        0        0        0 2023-11-25 20:04:00.083831 athina-1.4.1/athina/interfaces/__init__.py
--rw-r--r--   0        0        0     3905 2024-04-07 19:50:25.995763 athina-1.4.1/athina/interfaces/athina.py
--rw-r--r--   0        0        0      132 2024-04-07 19:50:25.995857 athina-1.4.1/athina/interfaces/data.py
--rw-r--r--   0        0        0     2065 2024-05-16 22:07:33.548003 athina-1.4.1/athina/interfaces/model.py
--rw-r--r--   0        0        0      100 2023-12-15 12:51:50.239840 athina-1.4.1/athina/interfaces/openai.py
--rw-r--r--   0        0        0     2944 2024-04-07 19:50:25.996104 athina-1.4.1/athina/interfaces/result.py
--rw-r--r--   0        0        0      126 2023-11-22 13:56:11.774041 athina-1.4.1/athina/keys/__init__.py
--rw-r--r--   0        0        0      322 2023-11-25 22:10:24.729172 athina-1.4.1/athina/keys/athina_api_key.py
--rw-r--r--   0        0        0      236 2023-11-22 13:57:34.533378 athina-1.4.1/athina/keys/openai_api_key.py
--rw-r--r--   0        0        0        0 2024-05-16 22:07:31.612271 athina-1.4.1/athina/llms/__init__.py
--rw-r--r--   0        0        0     1368 2024-05-24 10:38:54.005289 athina-1.4.1/athina/llms/abstract_llm_service.py
--rw-r--r--   0        0        0     1524 2024-05-24 10:38:54.005385 athina-1.4.1/athina/llms/litellm_service.py
--rw-r--r--   0        0        0     3461 2024-05-24 10:38:54.005505 athina-1.4.1/athina/llms/openai_service.py
--rw-r--r--   0        0        0      337 2023-12-21 07:47:22.706564 athina-1.4.1/athina/llms/question_answerer.py
--rw-r--r--   0        0        0     2874 2024-04-07 19:50:25.996425 athina-1.4.1/athina/llms/question_answerer_bulk.py
--rw-r--r--   0        0        0     3675 2024-04-07 19:50:25.996529 athina-1.4.1/athina/llms/question_answerer_cot.py
--rw-r--r--   0        0        0     6674 2024-04-07 19:50:25.996722 athina-1.4.1/athina/llms/question_answerer_with_retrieval.py
--rw-r--r--   0        0        0     2402 2024-04-07 19:50:25.996889 athina-1.4.1/athina/llms/question_generator.py
--rw-r--r--   0        0        0      323 2024-04-07 19:50:25.997032 athina-1.4.1/athina/loaders/__init__.py
--rw-r--r--   0        0        0     2326 2024-05-16 22:07:33.548158 athina-1.4.1/athina/loaders/base_loader.py
--rw-r--r--   0        0        0     2179 2024-05-16 22:07:33.548423 athina-1.4.1/athina/loaders/conversation_loader.py
--rw-r--r--   0        0        0     6507 2024-05-16 22:07:33.548593 athina-1.4.1/athina/loaders/loader.py
--rw-r--r--   0        0        0     3597 2024-05-16 22:07:33.548845 athina-1.4.1/athina/loaders/response_loader.py
--rw-r--r--   0        0        0     2970 2024-04-07 19:50:25.997588 athina-1.4.1/athina/loaders/summary_loader.py
--rw-r--r--   0        0        0     2380 2024-04-07 19:50:25.997668 athina-1.4.1/athina/loaders/text_loader.py
--rw-r--r--   0        0        0     1854 2023-12-21 07:47:22.709347 athina-1.4.1/athina/metrics/agreement_score.py
--rw-r--r--   0        0        0     2448 2023-12-21 07:47:22.709571 athina-1.4.1/athina/metrics/contradiction_score.py
--rw-r--r--   0        0        0     1342 2024-04-07 19:50:25.997754 athina-1.4.1/athina/metrics/groundedness.py
--rw-r--r--   0        0        0     2209 2023-12-23 23:51:10.658340 athina-1.4.1/athina/metrics/hallucination_score.py
--rw-r--r--   0        0        0      246 2024-01-14 09:48:35.094671 athina-1.4.1/athina/metrics/metric.py
--rw-r--r--   0        0        0     3000 2024-04-07 19:50:25.997868 athina-1.4.1/athina/metrics/metric_type.py
--rw-r--r--   0        0        0      393 2024-01-05 10:26:13.883309 athina-1.4.1/athina/metrics/passed.py
--rw-r--r--   0        0        0      275 2024-04-07 19:50:25.997955 athina-1.4.1/athina/metrics/ragas_metric.py
--rw-r--r--   0        0        0      509 2024-04-07 19:50:25.998030 athina-1.4.1/athina/metrics/similarity_score.py
--rw-r--r--   0        0        0        0 2023-11-21 23:55:43.624615 athina-1.4.1/athina/runner/__init__.py
--rw-r--r--   0        0        0     7034 2024-05-30 00:18:42.432531 athina-1.4.1/athina/runner/run.py
--rw-r--r--   0        0        0      418 2024-05-30 00:15:45.290012 athina-1.4.1/athina/runner/run_wrapper.py
--rw-r--r--   0        0        0     5729 2024-05-29 18:43:09.550327 athina-1.4.1/athina/scripts/guardrails.py
--rw-r--r--   0        0        0    13810 2024-05-26 21:36:09.961943 athina-1.4.1/athina/services/athina_api_service.py
--rw-r--r--   0        0        0      472 2024-05-24 10:38:54.005625 athina-1.4.1/athina/steps/__init__.py
--rw-r--r--   0        0        0     2107 2024-05-28 23:41:09.151184 athina-1.4.1/athina/steps/api.py
--rw-r--r--   0        0        0     4456 2024-05-24 10:38:54.006179 athina-1.4.1/athina/steps/base.py
--rw-r--r--   0        0        0     1729 2024-05-24 10:38:54.006387 athina-1.4.1/athina/steps/chain.py
--rw-r--r--   0        0        0     1346 2024-05-28 23:41:09.151429 athina-1.4.1/athina/steps/classify_text.py
--rw-r--r--   0        0        0     1501 2024-05-24 10:38:54.006892 athina-1.4.1/athina/steps/conditional.py
--rw-r--r--   0        0        0        0 2024-05-24 10:38:54.006919 athina-1.4.1/athina/steps/debug.py
--rw-r--r--   0        0        0     1440 2024-05-28 23:41:09.151588 athina-1.4.1/athina/steps/extract_entities.py
--rw-r--r--   0        0        0      646 2024-05-24 10:38:54.007404 athina-1.4.1/athina/steps/iterator.py
--rw-r--r--   0        0        0     3696 2024-05-28 23:41:09.151929 athina-1.4.1/athina/steps/llm.py
--rw-r--r--   0        0        0      787 2024-05-24 10:38:54.007611 athina-1.4.1/athina/steps/transform.py
--rw-r--r--   0        0        0     1090 2024-05-30 00:16:54.258793 athina-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 athina-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     8595 2024-05-03 15:41:49.406642 athina-1.4.2/README.md
+-rw-r--r--   0        0        0      169 2024-05-03 15:41:49.406999 athina-1.4.2/athina/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.4.2/athina/cli/__init__.py
+-rw-r--r--   0        0        0     5390 2024-05-05 12:00:16.321612 athina-1.4.2/athina/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.4.2/athina/constants/__init__.py
+-rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.4.2/athina/constants/messages.py
+-rw-r--r--   0        0        0       72 2024-05-03 15:41:49.407935 athina-1.4.2/athina/datasets/__init__.py
+-rw-r--r--   0        0        0   218970 2024-05-03 15:41:49.408467 athina-1.4.2/athina/datasets/conversations.json
+-rw-r--r--   0        0        0     3315 2024-05-29 20:37:43.202700 athina-1.4.2/athina/datasets/dataset.py
+-rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.4.2/athina/datasets/summarization_sample.py
+-rw-r--r--   0        0        0     2675 2024-05-03 15:41:49.409340 athina-1.4.2/athina/datasets/yc_query_mini.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.4.2/athina/errors/__init__.py
+-rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.4.2/athina/errors/exceptions.py
+-rw-r--r--   0        0        0     5016 2024-05-29 18:23:51.695514 athina-1.4.2/athina/evals/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-16 19:27:48.886844 athina-1.4.2/athina/evals/base_evaluator.py
+-rw-r--r--   0        0        0     4259 2024-05-16 19:27:48.887245 athina-1.4.2/athina/evals/conversation/conversation_coherence/evaluator.py
+-rw-r--r--   0        0        0     1198 2024-05-03 15:41:49.410542 athina-1.4.2/athina/evals/conversation/conversation_coherence/prompt.py
+-rw-r--r--   0        0        0     4414 2024-05-16 19:27:48.887449 athina-1.4.2/athina/evals/conversation/conversation_resolution/evaluator.py
+-rw-r--r--   0        0        0     1104 2024-05-03 15:41:49.410767 athina-1.4.2/athina/evals/conversation/conversation_resolution/prompt.py
+-rw-r--r--   0        0        0     2984 2024-05-29 18:23:51.695664 athina-1.4.2/athina/evals/eval_type.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.4.2/athina/evals/function/__init__.py
+-rw-r--r--   0        0        0     3780 2024-05-16 19:27:48.888106 athina-1.4.2/athina/evals/function/function_evaluator.py
+-rw-r--r--   0        0        0    20171 2024-05-29 18:23:51.696561 athina-1.4.2/athina/evals/function/functions.py
+-rw-r--r--   0        0        0    11066 2024-05-29 18:23:51.697020 athina-1.4.2/athina/evals/function/wrapper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.4.2/athina/evals/grounded/__init__.py
+-rw-r--r--   0        0        0     4298 2024-05-16 19:27:48.888364 athina-1.4.2/athina/evals/grounded/grounded_evaluator.py
+-rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.4.2/athina/evals/grounded/similarity.py
+-rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.4.2/athina/evals/grounded/wrapper.py
+-rw-r--r--   0        0        0     3369 2024-06-01 05:59:02.026656 athina-1.4.2/athina/evals/guardrails/correct_language/evaluator.py
+-rw-r--r--   0        0        0     2820 2024-06-01 05:59:02.026917 athina-1.4.2/athina/evals/guardrails/detect_pii/evaluator.py
+-rw-r--r--   0        0        0     3048 2024-06-01 05:59:02.027436 athina-1.4.2/athina/evals/guardrails/gibberish_text/evaluator.py
+-rw-r--r--   0        0        0     2701 2024-06-01 05:59:02.027606 athina-1.4.2/athina/evals/guardrails/no_secrets_present/evaluator.py
+-rw-r--r--   0        0        0     3141 2024-06-01 05:59:02.027839 athina-1.4.2/athina/evals/guardrails/politeness_check/evaluator.py
+-rw-r--r--   0        0        0     2656 2024-06-01 05:59:02.028223 athina-1.4.2/athina/evals/guardrails/profanity_free/evaluator.py
+-rw-r--r--   0        0        0     2833 2024-06-01 05:59:02.028659 athina-1.4.2/athina/evals/guardrails/reading_time/evaluator.py
+-rw-r--r--   0        0        0     3779 2024-06-01 05:59:02.029061 athina-1.4.2/athina/evals/guardrails/restrict_to_topic/evaluator.py
+-rw-r--r--   0        0        0     3804 2024-06-01 05:59:02.029255 athina-1.4.2/athina/evals/guardrails/sensitive_topics/evaluator.py
+-rw-r--r--   0        0        0     2972 2024-06-01 05:59:02.029401 athina-1.4.2/athina/evals/guardrails/sfw/evaluator.py
+-rw-r--r--   0        0        0     2857 2024-06-01 05:59:02.029797 athina-1.4.2/athina/evals/guardrails/toxic_language/evaluator.py
+-rw-r--r--   0        0        0     3180 2024-06-01 05:59:02.030159 athina-1.4.2/athina/evals/guardrails/unusual_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.4.2/athina/evals/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.4.2/athina/evals/llm/context_contains_enough_information/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-16 19:27:48.889580 athina-1.4.2/athina/evals/llm/context_contains_enough_information/evaluator.py
+-rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.4.2/athina/evals/llm/context_contains_enough_information/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.4.2/athina/evals/llm/custom_prompt/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-29 18:23:47.847799 athina-1.4.2/athina/evals/llm/custom_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.4.2/athina/evals/llm/does_response_answer_query/__init__.py
+-rw-r--r--   0        0        0     2632 2024-05-03 15:41:49.417364 athina-1.4.2/athina/evals/llm/does_response_answer_query/evaluator.py
+-rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.4.2/athina/evals/llm/does_response_answer_query/examples.py
+-rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.4.2/athina/evals/llm/example.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.4.2/athina/evals/llm/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2599 2024-05-03 15:41:49.417490 athina-1.4.2/athina/evals/llm/faithfulness/evaluator.py
+-rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.4.2/athina/evals/llm/faithfulness/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.4.2/athina/evals/llm/grading_criteria/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-16 19:27:48.889913 athina-1.4.2/athina/evals/llm/grading_criteria/evaluator.py
+-rw-r--r--   0        0        0     5821 2024-05-03 15:41:49.418273 athina-1.4.2/athina/evals/llm/groundedness/evaluator.py
+-rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.4.2/athina/evals/llm/groundedness/prompt.py
+-rw-r--r--   0        0        0     4982 2024-05-05 09:24:29.466550 athina-1.4.2/athina/evals/llm/llm_evaluator.py
+-rw-r--r--   0        0        0    10915 2024-05-03 15:41:49.418745 athina-1.4.2/athina/evals/llm/summary_accuracy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.4.2/athina/evals/ragas/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.4.2/athina/evals/ragas/answer_correctness/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-03 15:41:49.419035 athina-1.4.2/athina/evals/ragas/answer_correctness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.4.2/athina/evals/ragas/answer_relevancy/__init__.py
+-rw-r--r--   0        0        0     2441 2024-05-03 15:41:49.419202 athina-1.4.2/athina/evals/ragas/answer_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.4.2/athina/evals/ragas/answer_semantic_similarity/__init__.py
+-rw-r--r--   0        0        0     2440 2024-05-03 15:41:49.419340 athina-1.4.2/athina/evals/ragas/answer_semantic_similarity/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.4.2/athina/evals/ragas/coherence/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-03 15:41:49.419789 athina-1.4.2/athina/evals/ragas/coherence/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.4.2/athina/evals/ragas/conciseness/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-03 15:41:49.420084 athina-1.4.2/athina/evals/ragas/conciseness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.4.2/athina/evals/ragas/context_precision/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-03 15:41:49.420494 athina-1.4.2/athina/evals/ragas/context_precision/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.4.2/athina/evals/ragas/context_recall/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-03 15:41:49.420634 athina-1.4.2/athina/evals/ragas/context_recall/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.4.2/athina/evals/ragas/context_relevancy/__init__.py
+-rw-r--r--   0        0        0     2159 2024-05-03 15:41:49.420776 athina-1.4.2/athina/evals/ragas/context_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.4.2/athina/evals/ragas/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2370 2024-05-03 15:41:49.420918 athina-1.4.2/athina/evals/ragas/faithfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.4.2/athina/evals/ragas/harmfulness/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-03 15:41:49.421222 athina-1.4.2/athina/evals/ragas/harmfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.4.2/athina/evals/ragas/maliciousness/__init__.py
+-rw-r--r--   0        0        0     2127 2024-05-03 15:41:49.421640 athina-1.4.2/athina/evals/ragas/maliciousness/evaluator.py
+-rw-r--r--   0        0        0     3298 2024-05-03 15:41:49.421803 athina-1.4.2/athina/evals/ragas/ragas_evaluator.py
+-rw-r--r--   0        0        0     5154 2024-05-03 15:41:49.422152 athina-1.4.2/athina/evals/safety/content_moderation/evaluator.py
+-rw-r--r--   0        0        0     3387 2024-05-03 15:41:49.422800 athina-1.4.2/athina/evals/safety/pii_detection/evaluator.py
+-rw-r--r--   0        0        0     4370 2024-05-03 15:41:49.424028 athina-1.4.2/athina/evals/safety/prompt_injection/evaluator.py
+-rw-r--r--   0        0        0      106 2024-05-03 15:41:49.424321 athina-1.4.2/athina/guard/exception.py
+-rw-r--r--   0        0        0     1404 2024-05-03 15:41:49.424686 athina-1.4.2/athina/guard/guard.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.4.2/athina/helpers/__init__.py
+-rw-r--r--   0        0        0     5739 2024-05-16 19:27:48.890218 athina-1.4.2/athina/helpers/athina_logging_helper.py
+-rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.4.2/athina/helpers/config.py
+-rw-r--r--   0        0        0      122 2024-05-29 19:56:29.342493 athina-1.4.2/athina/helpers/constants.py
+-rw-r--r--   0        0        0      790 2024-05-16 19:27:48.890420 athina-1.4.2/athina/helpers/dataset_helper.py
+-rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.4.2/athina/helpers/eval_helper.py
+-rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.4.2/athina/helpers/function_eval_util.py
+-rw-r--r--   0        0        0     5152 2024-05-29 18:23:51.699858 athina-1.4.2/athina/helpers/get_evaluator.py
+-rw-r--r--   0        0        0      135 2024-05-25 05:42:57.983530 athina-1.4.2/athina/helpers/jinja_helper.py
+-rw-r--r--   0        0        0     2469 2024-05-22 07:52:50.227484 athina-1.4.2/athina/helpers/json.py
+-rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.4.2/athina/helpers/kwparser.py
+-rw-r--r--   0        0        0      894 2024-05-03 15:41:49.425348 athina-1.4.2/athina/helpers/loader_helper.py
+-rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.4.2/athina/helpers/logger.py
+-rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.4.2/athina/helpers/package_helper.py
+-rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.4.2/athina/helpers/run_helper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.4.2/athina/interfaces/__init__.py
+-rw-r--r--   0        0        0     3905 2024-05-03 15:41:49.425463 athina-1.4.2/athina/interfaces/athina.py
+-rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.4.2/athina/interfaces/data.py
+-rw-r--r--   0        0        0     2065 2024-05-14 15:59:10.451321 athina-1.4.2/athina/interfaces/model.py
+-rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.4.2/athina/interfaces/openai.py
+-rw-r--r--   0        0        0     2944 2024-05-05 12:12:32.954417 athina-1.4.2/athina/interfaces/result.py
+-rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.4.2/athina/keys/__init__.py
+-rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.4.2/athina/keys/athina_api_key.py
+-rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.4.2/athina/keys/openai_api_key.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.4.2/athina/llms/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-22 07:52:50.227988 athina-1.4.2/athina/llms/abstract_llm_service.py
+-rw-r--r--   0        0        0     1524 2024-05-22 07:52:50.228405 athina-1.4.2/athina/llms/litellm_service.py
+-rw-r--r--   0        0        0     3461 2024-05-29 18:23:47.848584 athina-1.4.2/athina/llms/openai_service.py
+-rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.4.2/athina/llms/question_answerer.py
+-rw-r--r--   0        0        0     2874 2024-05-21 13:33:12.522927 athina-1.4.2/athina/llms/question_answerer_bulk.py
+-rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.4.2/athina/llms/question_answerer_cot.py
+-rw-r--r--   0        0        0     6674 2024-05-03 15:41:49.426272 athina-1.4.2/athina/llms/question_answerer_with_retrieval.py
+-rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.4.2/athina/llms/question_generator.py
+-rw-r--r--   0        0        0      323 2024-05-03 15:41:49.426530 athina-1.4.2/athina/loaders/__init__.py
+-rw-r--r--   0        0        0     2326 2024-05-16 23:56:49.987467 athina-1.4.2/athina/loaders/base_loader.py
+-rw-r--r--   0        0        0     2179 2024-05-16 19:27:48.890989 athina-1.4.2/athina/loaders/conversation_loader.py
+-rw-r--r--   0        0        0     6507 2024-05-17 01:08:19.006440 athina-1.4.2/athina/loaders/loader.py
+-rw-r--r--   0        0        0     3597 2024-05-16 19:27:48.892946 athina-1.4.2/athina/loaders/response_loader.py
+-rw-r--r--   0        0        0     2970 2024-05-03 17:07:59.624449 athina-1.4.2/athina/loaders/summary_loader.py
+-rw-r--r--   0        0        0     2380 2024-05-03 15:41:49.427400 athina-1.4.2/athina/loaders/text_loader.py
+-rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.4.2/athina/metrics/agreement_score.py
+-rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.4.2/athina/metrics/contradiction_score.py
+-rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.4.2/athina/metrics/groundedness.py
+-rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.4.2/athina/metrics/hallucination_score.py
+-rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.4.2/athina/metrics/metric.py
+-rw-r--r--   0        0        0     3000 2024-05-03 15:41:49.427514 athina-1.4.2/athina/metrics/metric_type.py
+-rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.4.2/athina/metrics/passed.py
+-rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.4.2/athina/metrics/ragas_metric.py
+-rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.4.2/athina/metrics/similarity_score.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.4.2/athina/runner/__init__.py
+-rw-r--r--   0        0        0     7034 2024-05-30 05:39:04.348672 athina-1.4.2/athina/runner/run.py
+-rw-r--r--   0        0        0      418 2024-05-30 05:39:04.349357 athina-1.4.2/athina/runner/run_wrapper.py
+-rw-r--r--   0        0        0     5729 2024-05-29 18:23:51.700266 athina-1.4.2/athina/scripts/guardrails.py
+-rw-r--r--   0        0        0    13810 2024-05-29 20:37:14.247205 athina-1.4.2/athina/services/athina_api_service.py
+-rw-r--r--   0        0        0      472 2024-05-29 18:23:47.849253 athina-1.4.2/athina/steps/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-28 05:27:42.582035 athina-1.4.2/athina/steps/api.py
+-rw-r--r--   0        0        0     4456 2024-05-22 07:52:50.229580 athina-1.4.2/athina/steps/base.py
+-rw-r--r--   0        0        0     1729 2024-05-22 07:52:50.229864 athina-1.4.2/athina/steps/chain.py
+-rw-r--r--   0        0        0     1346 2024-05-27 14:49:53.587855 athina-1.4.2/athina/steps/classify_text.py
+-rw-r--r--   0        0        0     1501 2024-05-22 07:52:50.230002 athina-1.4.2/athina/steps/conditional.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:52:50.230033 athina-1.4.2/athina/steps/debug.py
+-rw-r--r--   0        0        0     1440 2024-05-27 14:49:53.588354 athina-1.4.2/athina/steps/extract_entities.py
+-rw-r--r--   0        0        0      646 2024-05-22 07:52:50.230202 athina-1.4.2/athina/steps/iterator.py
+-rw-r--r--   0        0        0     3696 2024-06-01 05:58:57.571371 athina-1.4.2/athina/steps/llm.py
+-rw-r--r--   0        0        0      787 2024-05-22 07:52:50.230543 athina-1.4.2/athina/steps/transform.py
+-rw-r--r--   0        0        0     1090 2024-06-01 05:59:02.030753 athina-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9904 1970-01-01 00:00:00.000000 athina-1.4.2/PKG-INFO
```

### Comparing `athina-1.4.1/README.md` & `athina-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/cli/cli.py` & `athina-1.4.2/athina/cli/cli.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/constants/messages.py` & `athina-1.4.2/athina/constants/messages.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/datasets/conversations.json` & `athina-1.4.2/athina/datasets/conversations.json`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/datasets/dataset.py` & `athina-1.4.2/athina/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/datasets/summarization_sample.py` & `athina-1.4.2/athina/datasets/summarization_sample.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/datasets/yc_query_mini.py` & `athina-1.4.2/athina/datasets/yc_query_mini.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/errors/exceptions.py` & `athina-1.4.2/athina/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/__init__.py` & `athina-1.4.2/athina/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/base_evaluator.py` & `athina-1.4.2/athina/evals/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/conversation/conversation_coherence/evaluator.py` & `athina-1.4.2/athina/evals/conversation/conversation_coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/conversation/conversation_coherence/prompt.py` & `athina-1.4.2/athina/evals/conversation/conversation_coherence/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/conversation/conversation_resolution/evaluator.py` & `athina-1.4.2/athina/evals/conversation/conversation_resolution/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/conversation/conversation_resolution/prompt.py` & `athina-1.4.2/athina/evals/conversation/conversation_resolution/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/eval_type.py` & `athina-1.4.2/athina/evals/eval_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/function/function_evaluator.py` & `athina-1.4.2/athina/evals/function/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/function/functions.py` & `athina-1.4.2/athina/evals/function/functions.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/function/wrapper.py` & `athina-1.4.2/athina/evals/function/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/grounded/grounded_evaluator.py` & `athina-1.4.2/athina/evals/grounded/grounded_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/grounded/similarity.py` & `athina-1.4.2/athina/evals/grounded/similarity.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/grounded/wrapper.py` & `athina-1.4.2/athina/evals/grounded/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/guardrails/correct_language/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/correct_language/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 validation_passed = False
                 grade_reason = str(e).replace('Validation failed for field with errors:', '')
 
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=validation_passed,
+                    value=float(validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/detect_pii/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/detect_pii/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             # Pass LLM output through guard
             guard_result = guard.parse(text)
             grade_reason = "Text is free of PII" if guard_result.validation_passed else "Text contains PII"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/gibberish_text/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/gibberish_text/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             # Pass LLM output through guard
             guard_result = guard.parse(text)
             grade_reason = "Text is sensible" if guard_result.validation_passed else "Text is gibberish"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/no_secrets_present/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/no_secrets_present/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             # Pass LLM output through guard
             guard_result = guard.parse(text)
             grade_reason = "Text contains secrets" if guard_result.validation_passed else "Text has no secrets"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/politeness_check/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/politeness_check/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             guard = Guard.from_string(validators=[self.validator])
             guard_result = guard.parse(text)
             grade_reason = "Text is polite" if guard_result.validation_passed else "Text is not polite"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/profanity_free/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/profanity_free/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             # Pass LLM output through guard
             guard_result = guard.parse(text)
             grade_reason = "Text is profanity-free" if guard_result.validation_passed else "Text contains profanity"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/reading_time/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/reading_time/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             # Pass LLM output through guard
             guard_result = guard.parse(text)
             grade_reason = "Text is readable within provided time." if guard_result.validation_passed else "Text is not readable within provided time."
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/restrict_to_topic/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/restrict_to_topic/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 validation_passed = False
                 grade_reason = str(e).replace('Validation failed for field with errors:', '')
 
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=validation_passed,
+                    value=float(validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/sensitive_topics/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/sensitive_topics/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 validation_passed = False
                 grade_reason = str(e).replace('Validation failed for field with errors:', '')
 
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=validation_passed,
+                    value=float(validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/sfw/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/sfw/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             # Pass LLM output through guard
             guard_result = guard.parse(text)
             grade_reason = "Text is safe for work" if guard_result.validation_passed else "Text is NSFW"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/toxic_language/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/toxic_language/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             # Setup Guard
             guard_result = self._guard.validate(text)
             grade_reason = "Text is toxicity-free" if guard_result.validation_passed else "Text is toxic"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/guardrails/unusual_prompt/evaluator.py` & `athina-1.4.2/athina/evals/guardrails/unusual_prompt/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             guard = Guard.from_string(validators=[self.validator])
             guard_result = guard.parse(text)
             grade_reason = "Text is not an unusual prompt" if guard_result.validation_passed else "Text is a unusual prompt"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
-                    value=guard_result.validation_passed,
+                    value=float(guard_result.validation_passed),
                 )
             )
         except Exception as e:
             logger.error(f"Error occurred during eval: {e}")
             raise e
 
         end_time = time.time()
```

### Comparing `athina-1.4.1/athina/evals/llm/context_contains_enough_information/evaluator.py` & `athina-1.4.2/athina/evals/llm/context_contains_enough_information/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/context_contains_enough_information/examples.py` & `athina-1.4.2/athina/evals/llm/context_contains_enough_information/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/custom_prompt/evaluator.py` & `athina-1.4.2/athina/evals/llm/custom_prompt/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/does_response_answer_query/evaluator.py` & `athina-1.4.2/athina/evals/llm/does_response_answer_query/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/does_response_answer_query/examples.py` & `athina-1.4.2/athina/evals/llm/does_response_answer_query/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/example.py` & `athina-1.4.2/athina/evals/llm/example.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/faithfulness/evaluator.py` & `athina-1.4.2/athina/evals/llm/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/faithfulness/examples.py` & `athina-1.4.2/athina/evals/llm/faithfulness/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/grading_criteria/evaluator.py` & `athina-1.4.2/athina/evals/llm/grading_criteria/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/groundedness/evaluator.py` & `athina-1.4.2/athina/evals/llm/groundedness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/groundedness/prompt.py` & `athina-1.4.2/athina/evals/llm/groundedness/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/llm_evaluator.py` & `athina-1.4.2/athina/evals/llm/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/llm/summary_accuracy/evaluator.py` & `athina-1.4.2/athina/evals/llm/summary_accuracy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/answer_correctness/evaluator.py` & `athina-1.4.2/athina/evals/ragas/answer_correctness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/answer_relevancy/evaluator.py` & `athina-1.4.2/athina/evals/ragas/answer_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/answer_semantic_similarity/evaluator.py` & `athina-1.4.2/athina/evals/ragas/answer_semantic_similarity/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/coherence/evaluator.py` & `athina-1.4.2/athina/evals/ragas/coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/conciseness/evaluator.py` & `athina-1.4.2/athina/evals/ragas/conciseness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/context_precision/evaluator.py` & `athina-1.4.2/athina/evals/ragas/context_precision/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/context_recall/evaluator.py` & `athina-1.4.2/athina/evals/ragas/context_recall/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/context_relevancy/evaluator.py` & `athina-1.4.2/athina/evals/ragas/context_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/faithfulness/evaluator.py` & `athina-1.4.2/athina/evals/ragas/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/harmfulness/evaluator.py` & `athina-1.4.2/athina/evals/ragas/harmfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/maliciousness/evaluator.py` & `athina-1.4.2/athina/evals/ragas/maliciousness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/ragas/ragas_evaluator.py` & `athina-1.4.2/athina/evals/ragas/ragas_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/safety/content_moderation/evaluator.py` & `athina-1.4.2/athina/evals/safety/content_moderation/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/safety/pii_detection/evaluator.py` & `athina-1.4.2/athina/evals/safety/pii_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/evals/safety/prompt_injection/evaluator.py` & `athina-1.4.2/athina/evals/safety/prompt_injection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/guard/guard.py` & `athina-1.4.2/athina/guard/guard.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/athina_logging_helper.py` & `athina-1.4.2/athina/helpers/athina_logging_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/config.py` & `athina-1.4.2/athina/helpers/config.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/dataset_helper.py` & `athina-1.4.2/athina/helpers/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/function_eval_util.py` & `athina-1.4.2/athina/helpers/function_eval_util.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/get_evaluator.py` & `athina-1.4.2/athina/helpers/get_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/json.py` & `athina-1.4.2/athina/helpers/json.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/loader_helper.py` & `athina-1.4.2/athina/helpers/loader_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/logger.py` & `athina-1.4.2/athina/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/helpers/run_helper.py` & `athina-1.4.2/athina/helpers/run_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/interfaces/athina.py` & `athina-1.4.2/athina/interfaces/athina.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/interfaces/model.py` & `athina-1.4.2/athina/interfaces/model.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/interfaces/result.py` & `athina-1.4.2/athina/interfaces/result.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/abstract_llm_service.py` & `athina-1.4.2/athina/llms/abstract_llm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/litellm_service.py` & `athina-1.4.2/athina/llms/litellm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/openai_service.py` & `athina-1.4.2/athina/llms/openai_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/question_answerer_bulk.py` & `athina-1.4.2/athina/llms/question_answerer_bulk.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/question_answerer_cot.py` & `athina-1.4.2/athina/llms/question_answerer_cot.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/question_answerer_with_retrieval.py` & `athina-1.4.2/athina/llms/question_answerer_with_retrieval.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/llms/question_generator.py` & `athina-1.4.2/athina/llms/question_generator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/loaders/base_loader.py` & `athina-1.4.2/athina/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/loaders/conversation_loader.py` & `athina-1.4.2/athina/loaders/conversation_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/loaders/loader.py` & `athina-1.4.2/athina/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/loaders/response_loader.py` & `athina-1.4.2/athina/loaders/response_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/loaders/summary_loader.py` & `athina-1.4.2/athina/loaders/summary_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/loaders/text_loader.py` & `athina-1.4.2/athina/loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/metrics/agreement_score.py` & `athina-1.4.2/athina/metrics/agreement_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/metrics/contradiction_score.py` & `athina-1.4.2/athina/metrics/contradiction_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/metrics/groundedness.py` & `athina-1.4.2/athina/metrics/groundedness.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/metrics/hallucination_score.py` & `athina-1.4.2/athina/metrics/hallucination_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/metrics/metric_type.py` & `athina-1.4.2/athina/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/runner/run.py` & `athina-1.4.2/athina/runner/run.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/scripts/guardrails.py` & `athina-1.4.2/athina/scripts/guardrails.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/services/athina_api_service.py` & `athina-1.4.2/athina/services/athina_api_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/api.py` & `athina-1.4.2/athina/steps/api.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/base.py` & `athina-1.4.2/athina/steps/base.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/chain.py` & `athina-1.4.2/athina/steps/chain.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/classify_text.py` & `athina-1.4.2/athina/steps/classify_text.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/conditional.py` & `athina-1.4.2/athina/steps/conditional.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/extract_entities.py` & `athina-1.4.2/athina/steps/extract_entities.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/iterator.py` & `athina-1.4.2/athina/steps/iterator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/llm.py` & `athina-1.4.2/athina/steps/llm.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/athina/steps/transform.py` & `athina-1.4.2/athina/steps/transform.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.1/pyproject.toml` & `athina-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athina"
-version = "1.4.1"
+version = "1.4.2"
 description = "Python SDK to configure and run evaluations for your LLM-based application"
 authors = ["Shiv Sakhuja <shiv@athina.ai>", "Akshat Gupta <akshat@athina.ai>", "Vivek Aditya <vivek@athina.ai>", "Akhil Bisht <akhil@athina.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 retrying = "^1.3.4"
```

### Comparing `athina-1.4.1/PKG-INFO` & `athina-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: athina
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python SDK to configure and run evaluations for your LLM-based application
 Author: Shiv Sakhuja
 Author-email: shiv@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: datasets (>=2.16.0,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: langchain (>=0.0.350)
 Requires-Dist: langchain-openai (>=0.0.3,<0.0.4)
 Requires-Dist: litellm (==1.35.6)
 Requires-Dist: llama-index (>=0.9.40,<0.10.0)
```

