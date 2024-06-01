# Comparing `tmp/hezar-0.37.0.tar.gz` & `tmp/hezar-0.38.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.37.0.tar", max compression
+gzip compressed data, was "hezar-0.38.0.tar", max compression
```

## Comparing `hezar-0.37.0.tar` & `hezar-0.38.0.tar`

### file list

```diff
@@ -1,136 +1,137 @@
--rw-r--r--   0        0        0    11337 2024-05-15 19:20:22.371938 hezar-0.37.0/LICENSE
--rw-r--r--   0        0        0    14442 2024-05-15 19:20:22.371938 hezar-0.37.0/README.md
--rw-r--r--   0        0        0      623 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/__init__.py
--rw-r--r--   0        0        0     5651 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/builders.py
--rw-r--r--   0        0        0    18042 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/configs.py
--rw-r--r--   0        0        0     4712 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/constants.py
--rw-r--r--   0        0        0       54 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/data/__init__.py
--rw-r--r--   0        0        0    13756 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      634 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     3760 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3727 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/image_captioning_dataset.py
--rw-r--r--   0        0        0     7384 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/ocr_dataset.py
--rw-r--r--   0        0        0     5923 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3079 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/speech_recognition_dataset.py
--rw-r--r--   0        0        0     4498 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     4820 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0      202 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0    11544 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     7171 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     7668 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      444 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     2285 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/accuracy.py
--rw-r--r--   0        0        0     2484 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/bleu.py
--rw-r--r--   0        0        0     3711 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/cer.py
--rw-r--r--   0        0        0     3209 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0     1302 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     3566 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/precision.py
--rw-r--r--   0        0        0     3509 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     3155 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/rouge.py
--rw-r--r--   0        0        0     4029 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0     2950 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/wer.py
--rw-r--r--   0        0        0      333 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/__init__.py
--rw-r--r--   0        0        0       88 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/__init__.py
--rw-r--r--   0        0        0       35 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/bert/__init__.py
--rw-r--r--   0        0        0     2787 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/bert/bert.py
--rw-r--r--   0        0        0      743 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/bert/bert_config.py
--rw-r--r--   0        0        0       53 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/distilbert/__init__.py
--rw-r--r--   0        0        0     2288 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/distilbert/distilbert.py
--rw-r--r--   0        0        0      618 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/distilbert/distilbert_config.py
--rw-r--r--   0        0        0       44 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/roberta/__init__.py
--rw-r--r--   0        0        0     2788 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/roberta/roberta.py
--rw-r--r--   0        0        0      812 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/roberta/roberta_config.py
--rw-r--r--   0        0        0       55 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/vit/__init__.py
--rw-r--r--   0        0        0     2172 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/vit/vit.py
--rw-r--r--   0        0        0      572 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/vit/vit_config.py
--rw-r--r--   0        0        0      120 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0      131 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/beit_roberta/__init__.py
--rw-r--r--   0        0        0     3493 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
--rw-r--r--   0        0        0     2376 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
--rw-r--r--   0        0        0      101 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0     1106 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/crnn_decode_utils.py
--rw-r--r--   0        0        0     4649 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/crnn_image2text.py
--rw-r--r--   0        0        0      478 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/crnn_image2text_config.py
--rw-r--r--   0        0        0      105 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0     3430 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text.py
--rw-r--r--   0        0        0     1899 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text_config.py
--rw-r--r--   0        0        0      115 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_gpt2/__init__.py
--rw-r--r--   0        0        0     3463 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
--rw-r--r--   0        0        0     1872 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
--rw-r--r--   0        0        0      127 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_roberta/__init__.py
--rw-r--r--   0        0        0     3864 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
--rw-r--r--   0        0        0     1952 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
--rw-r--r--   0        0        0       69 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/__init__.py
--rw-r--r--   0        0        0      107 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/bert/__init__.py
--rw-r--r--   0        0        0     4320 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling.py
--rw-r--r--   0        0        0      771 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py
--rw-r--r--   0        0        0      131 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/distilbert/__init__.py
--rw-r--r--   0        0        0     3921 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
--rw-r--r--   0        0        0      637 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
--rw-r--r--   0        0        0      119 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/roberta/__init__.py
--rw-r--r--   0        0        0     4384 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py
--rw-r--r--   0        0        0      831 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
--rw-r--r--   0        0        0    20158 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/model.py
--rw-r--r--   0        0        0     2141 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/model_outputs.py
--rw-r--r--   0        0        0       69 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     5118 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      931 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     5172 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      872 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0      139 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/roberta/__init__.py
--rw-r--r--   0        0        0     5821 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
--rw-r--r--   0        0        0     1025 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
--rw-r--r--   0        0        0       23 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0      306 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/speech_recognition/whisper/__init__.py
--rw-r--r--   0        0        0     7713 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
--rw-r--r--   0        0        0     7059 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
--rw-r--r--   0        0        0     2777 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
--rw-r--r--   0        0        0    27594 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
--rw-r--r--   0        0        0       69 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     4796 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      845 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     4357 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      748 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     4963 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      942 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_embedding/__init__.py
--rw-r--r--   0        0        0       38 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/__init__.py
--rw-r--r--   0        0        0      119 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/gpt2/__init__.py
--rw-r--r--   0        0        0     3324 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py
--rw-r--r--   0        0        0     1148 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
--rw-r--r--   0        0        0      111 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/t5/__init__.py
--rw-r--r--   0        0        0     4053 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation.py
--rw-r--r--   0        0        0      837 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation_config.py
--rw-r--r--   0        0        0      390 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0    13303 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/audio_feature_extractor.py
--rw-r--r--   0        0        0     8292 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/image_processor.py
--rw-r--r--   0        0        0     5043 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     4635 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      337 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     3973 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     4181 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4102 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    27637 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3537 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     6584 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/registry.py
--rw-r--r--   0        0        0      113 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/__init__.py
--rw-r--r--   0        0        0     7345 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/metrics_handlers.py
--rw-r--r--   0        0        0    31550 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/trainer.py
--rw-r--r--   0        0        0     5624 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/trainer_utils.py
--rw-r--r--   0        0        0      245 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0    23979 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/audio_utils.py
--rw-r--r--   0        0        0     3955 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0     7676 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/data_utils.py
--rw-r--r--   0        0        0      976 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     4145 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0     7352 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/image_utils.py
--rw-r--r--   0        0        0     1376 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/integration_utils.py
--rw-r--r--   0        0        0      622 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/logging.py
--rw-r--r--   0        0        0     4498 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     2600 2024-05-15 19:20:22.379938 hezar-0.37.0/pyproject.toml
--rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.37.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-06-01 08:04:44.624830 hezar-0.38.0/LICENSE
+-rw-r--r--   0        0        0    14442 2024-06-01 08:04:44.624830 hezar-0.38.0/README.md
+-rw-r--r--   0        0        0      623 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5651 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/builders.py
+-rw-r--r--   0        0        0    18631 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/configs.py
+-rw-r--r--   0        0        0     4752 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/constants.py
+-rw-r--r--   0        0        0       83 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0    13756 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0     1031 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/data_samplers.py
+-rw-r--r--   0        0        0      634 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     3727 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/image_captioning_dataset.py
+-rw-r--r--   0        0        0     7384 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/ocr_dataset.py
+-rw-r--r--   0        0        0     5923 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3079 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/speech_recognition_dataset.py
+-rw-r--r--   0        0        0     4498 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     4820 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0      202 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0    11544 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     7171 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     7668 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      444 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     2285 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/accuracy.py
+-rw-r--r--   0        0        0     2484 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/bleu.py
+-rw-r--r--   0        0        0     3711 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/cer.py
+-rw-r--r--   0        0        0     3209 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0     1302 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     3566 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/precision.py
+-rw-r--r--   0        0        0     3509 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     3155 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/rouge.py
+-rw-r--r--   0        0        0     4029 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0     2950 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/wer.py
+-rw-r--r--   0        0        0      362 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/__init__.py
+-rw-r--r--   0        0        0       35 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/bert/__init__.py
+-rw-r--r--   0        0        0     2787 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/bert/bert.py
+-rw-r--r--   0        0        0      743 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/bert/bert_config.py
+-rw-r--r--   0        0        0       53 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/distilbert/__init__.py
+-rw-r--r--   0        0        0     2288 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/distilbert/distilbert.py
+-rw-r--r--   0        0        0      618 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/distilbert/distilbert_config.py
+-rw-r--r--   0        0        0       44 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/roberta/__init__.py
+-rw-r--r--   0        0        0     2788 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/roberta/roberta.py
+-rw-r--r--   0        0        0      812 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/roberta/roberta_config.py
+-rw-r--r--   0        0        0       55 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/vit/__init__.py
+-rw-r--r--   0        0        0     2172 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/vit/vit.py
+-rw-r--r--   0        0        0      572 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/vit/vit_config.py
+-rw-r--r--   0        0        0      120 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0      131 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/beit_roberta/__init__.py
+-rw-r--r--   0        0        0     3493 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
+-rw-r--r--   0        0        0     2376 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
+-rw-r--r--   0        0        0      101 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0     1106 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/crnn_decode_utils.py
+-rw-r--r--   0        0        0     4649 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/crnn_image2text.py
+-rw-r--r--   0        0        0      478 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/crnn_image2text_config.py
+-rw-r--r--   0        0        0      105 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0     3430 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text.py
+-rw-r--r--   0        0        0     1899 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text_config.py
+-rw-r--r--   0        0        0      115 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_gpt2/__init__.py
+-rw-r--r--   0        0        0     3463 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
+-rw-r--r--   0        0        0     1872 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
+-rw-r--r--   0        0        0      127 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_roberta/__init__.py
+-rw-r--r--   0        0        0     3864 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
+-rw-r--r--   0        0        0     1952 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
+-rw-r--r--   0        0        0       69 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/__init__.py
+-rw-r--r--   0        0        0      107 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/bert/__init__.py
+-rw-r--r--   0        0        0     4320 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling.py
+-rw-r--r--   0        0        0      771 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py
+-rw-r--r--   0        0        0      131 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/distilbert/__init__.py
+-rw-r--r--   0        0        0     3921 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
+-rw-r--r--   0        0        0      637 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
+-rw-r--r--   0        0        0      119 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/roberta/__init__.py
+-rw-r--r--   0        0        0     4384 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py
+-rw-r--r--   0        0        0      831 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
+-rw-r--r--   0        0        0    20471 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/model.py
+-rw-r--r--   0        0        0     2346 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0       69 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     5118 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      931 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     5172 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      872 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      139 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/roberta/__init__.py
+-rw-r--r--   0        0        0     5821 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
+-rw-r--r--   0        0        0     1025 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
+-rw-r--r--   0        0        0       23 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      306 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/__init__.py
+-rw-r--r--   0        0        0     7713 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
+-rw-r--r--   0        0        0     7067 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
+-rw-r--r--   0        0        0     2821 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
+-rw-r--r--   0        0        0    27594 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
+-rw-r--r--   0        0        0       69 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     4796 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      845 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     4357 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      748 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     4963 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      942 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_embedding/__init__.py
+-rw-r--r--   0        0        0       38 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/__init__.py
+-rw-r--r--   0        0        0      119 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/gpt2/__init__.py
+-rw-r--r--   0        0        0     3324 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py
+-rw-r--r--   0        0        0     1148 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
+-rw-r--r--   0        0        0      111 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/t5/__init__.py
+-rw-r--r--   0        0        0     4053 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation.py
+-rw-r--r--   0        0        0      837 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation_config.py
+-rw-r--r--   0        0        0      390 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0    13303 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/audio_feature_extractor.py
+-rw-r--r--   0        0        0     8292 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/image_processor.py
+-rw-r--r--   0        0        0     5043 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     4635 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      337 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     3973 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     4181 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4102 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    27637 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3537 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     6584 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/registry.py
+-rw-r--r--   0        0        0      113 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/__init__.py
+-rw-r--r--   0        0        0     7345 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/metrics_handlers.py
+-rw-r--r--   0        0        0    32462 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/trainer.py
+-rw-r--r--   0        0        0     5624 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/trainer_utils.py
+-rw-r--r--   0        0        0      245 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0    23979 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/audio_utils.py
+-rw-r--r--   0        0        0     3955 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0     7678 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/data_utils.py
+-rw-r--r--   0        0        0      976 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     4145 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0     7352 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/image_utils.py
+-rw-r--r--   0        0        0     1376 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/integration_utils.py
+-rw-r--r--   0        0        0      622 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0     4498 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     2602 2024-06-01 08:04:44.632830 hezar-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.38.0/PKG-INFO
```

### Comparing `hezar-0.37.0/LICENSE` & `hezar-0.38.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/README.md` & `hezar-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/__init__.py` & `hezar-0.38.0/hezar/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.37.0"
+__version__ = "0.38.0"
```

### Comparing `hezar-0.37.0/hezar/builders.py` & `hezar-0.38.0/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/configs.py` & `hezar-0.38.0/hezar/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,15 +370,21 @@
         output_dir (str):
             Path to the directory to save trainer properties.
         device (str):
             Hardware device e.g, `cuda:0`, `cpu`, etc.
         num_epochs (int):
             Number of total epochs to train the model.
         init_weights_from (str):
-            Path to a model from disk or Hub to load the initial weights from.
+            Path to a model from disk or Hub to load the initial weights from. Note that this only loads the model
+            weights and ignores other checkpoint-related states if the path is a checkpoint. To resume training from
+            a checkpoint use the `resume` parameter.
+        resume_from_checkpoint (bool, str, os.PathLike):
+            Resume training from a checkpoint. If set to True, the trainer will load the latest checkpoint, otherwise if
+            a path to a checkpoint is given, it will load that checkpoint and all the other states corresponding to that
+            checkpoint.
         num_dataloader_workers (int):
             Number of dataloader workers, defaults to 4 .
         seed (int):
             Control determinism of the run by setting a seed value. defaults to 42.
         optimizer (OptimizerType):
             Name of the optimizer, available values include properties in `OptimizerType` enum.
         learning_rate (float):
@@ -420,14 +426,15 @@
     name: str = field(init=False, default="trainer")
     config_type: str = field(init=False, default=ConfigType.TRAINER)
     output_dir: str
     task: str | TaskType
     device: str = "cuda"
     num_epochs: int = None
     init_weights_from: str = None
+    resume_from_checkpoint: bool | str | os.PathLike = None
     num_dataloader_workers: int = 0
     dataloader_drop_last: bool = False
     dataloader_shuffle: bool = True
     seed: int = 42
     optimizer: str | OptimizerType = None
     learning_rate: float = 2e-5
     weight_decay: float = 0.0
```

### Comparing `hezar-0.37.0/hezar/constants.py` & `hezar-0.38.0/hezar/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 DEFAULT_MODEL_FILE = "model.pt"
 DEFAULT_MODEL_CONFIG_FILE = "model_config.yaml"
 DEFAULT_TRAINER_SUBFOLDER = "train"
 DEFAULT_TRAINER_CONFIG_FILE = "train_config.yaml"
 DEFAULT_TRAINER_CSV_LOG_FILE = "training_logs.csv"
 DEFAULT_TRAINER_STATE_FILE = "trainer_state.yaml"
+DEFAULT_OPTIMIZER_FILE = "optimizer.pt"
 DEFAULT_PREPROCESSOR_SUBFOLDER = "preprocessor"
 DEFAULT_NORMALIZER_CONFIG_FILE = "normalizer_config.yaml"
 DEFAULT_IMAGE_PROCESSOR_CONFIG_FILE = "image_processor_config.yaml"
 DEFAULT_FEATURE_EXTRACTOR_CONFIG_FILE = "feature_extractor_config.yaml"
 DEFAULT_TOKENIZER_FILE = "tokenizer.json"
 DEFAULT_TOKENIZER_CONFIG_FILE = "tokenizer_config.yaml"
 DEFAULT_DATASET_CONFIG_FILE = "dataset_config.yaml"
```

### Comparing `hezar-0.37.0/hezar/data/data_collators.py` & `hezar-0.38.0/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/__init__.py` & `hezar-0.38.0/hezar/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/dataset.py` & `hezar-0.38.0/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/image_captioning_dataset.py` & `hezar-0.38.0/hezar/data/datasets/image_captioning_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/ocr_dataset.py` & `hezar-0.38.0/hezar/data/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.38.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/speech_recognition_dataset.py` & `hezar-0.38.0/hezar/data/datasets/speech_recognition_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.38.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.38.0/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/embeddings/embedding.py` & `hezar-0.38.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/embeddings/fasttext.py` & `hezar-0.38.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/embeddings/word2vec.py` & `hezar-0.38.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/accuracy.py` & `hezar-0.38.0/hezar/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/bleu.py` & `hezar-0.38.0/hezar/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/cer.py` & `hezar-0.38.0/hezar/metrics/cer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/f1.py` & `hezar-0.38.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/metric.py` & `hezar-0.38.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/precision.py` & `hezar-0.38.0/hezar/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/recall.py` & `hezar-0.38.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/rouge.py` & `hezar-0.38.0/hezar/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/seqeval.py` & `hezar-0.38.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/metrics/wer.py` & `hezar-0.38.0/hezar/metrics/wer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/bert/bert.py` & `hezar-0.38.0/hezar/models/backbone/bert/bert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/bert/bert_config.py` & `hezar-0.38.0/hezar/models/backbone/bert/bert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/distilbert/distilbert.py` & `hezar-0.38.0/hezar/models/backbone/distilbert/distilbert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/distilbert/distilbert_config.py` & `hezar-0.38.0/hezar/models/backbone/distilbert/distilbert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/roberta/roberta.py` & `hezar-0.38.0/hezar/models/backbone/roberta/roberta.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/roberta/roberta_config.py` & `hezar-0.38.0/hezar/models/backbone/roberta/roberta_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/vit/vit.py` & `hezar-0.38.0/hezar/models/backbone/vit/vit.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/backbone/vit/vit_config.py` & `hezar-0.38.0/hezar/models/backbone/vit/vit_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py` & `hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py` & `hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/crnn/crnn_decode_utils.py` & `hezar-0.38.0/hezar/models/image2text/crnn/crnn_decode_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/crnn/crnn_image2text.py` & `hezar-0.38.0/hezar/models/image2text/crnn/crnn_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text.py` & `hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text_config.py` & `hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py` & `hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py` & `hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py` & `hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py` & `hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling.py` & `hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py` & `hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py` & `hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py` & `hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py` & `hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py` & `hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/model.py` & `hezar-0.38.0/hezar/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,29 +366,33 @@
         return model_outputs
 
     @torch.inference_mode()
     def predict(
         self,
         inputs: Any | List[Any],
         device: str | torch.device = None,
+        preprocess: bool = True,
         unpack_forward_inputs: bool = True,
+        post_process: bool = True,
         **kwargs,
     ) -> List[Any] | torch.Tensor:
         """
         Perform an end-to-end prediction on raw inputs.
 
         If the model is a generative model, it has to implement the `generate()` method too which will be called
         instead of `forward()`. (`forward()` method is called internally within the `generate()` method)
 
         Args:
             inputs: Raw inputs e.g, a list of texts, path to images, etc.
             device: What device to perform inference on
+            preprocess: Whether to call :method:`preprocess()` before :method:`forward()`
             unpack_forward_inputs: Whether to unpack forward inputs. Set to False if you want to send preprocess outputs
                 directly to the `forward/generate` method without unpacking it. Note that this only applies to the cases
                 that the preprocess method's output is a dict-like/mapping object.
+            post_process: Whether to call :method:`post_process()` after :method:`forward()`
             **kwargs: Other arguments for `preprocess`, `forward`, `generate` and `post_process`. each will be passed to
                 the correct method automatically.
 
         Returns:
             Prediction results, each model or task can have its own type and structure
         """
         # Unpack kwargs for each step
@@ -401,32 +405,33 @@
                 f"Unrecognized arguments {list(invalid_kwargs.keys())} passed to `{self.__class__.__name__}.predict()`"
             )
 
         # Put model in eval mode
         self.eval()
 
         # Preprocessing step
-        model_inputs = self.preprocess(inputs, **preprocess_kwargs)
+        model_inputs = self.preprocess(inputs, **preprocess_kwargs) if preprocess else inputs
 
         # Map inputs and model to device
         device = device or self.device
         model_inputs = self._move_inputs_to_device(model_inputs, device)
         self.to(device)
 
         # Specify model inference function
         inference_fn = self.generate if self.is_generative else self.__call__
 
         # Model inference step (forward for regular models and generate for generative models)
-        if isinstance(model_inputs, Dict) and unpack_forward_inputs:
+        if isinstance(model_inputs, dict) and unpack_forward_inputs:
             model_outputs = inference_fn(**model_inputs, **forward_kwargs)
         else:
             model_outputs = inference_fn(model_inputs, **forward_kwargs)
 
         # Post-processing step
-        processed_outputs = self.post_process(model_outputs, **post_process_kwargs)
+        processed_outputs = self.post_process(model_outputs, **post_process_kwargs) if post_process else model_outputs
+
         return processed_outputs
 
     @staticmethod
     def _move_inputs_to_device(inputs, device):
         """
         Move all input tensors in the inputs to the device
```

### Comparing `hezar-0.37.0/hezar/models/model_outputs.py` & `hezar-0.38.0/hezar/models/model_outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 """
 Define all model outputs here
 """
 from dataclasses import asdict, dataclass
 from typing import Dict, List, Optional
 
 
+__all__ = [
+    "ModelOutput",
+    "MaskFillingOutput",
+    "TextClassificationOutput",
+    "SequenceLabelingOutput",
+    "TextGenerationOutput",
+    "SpeechRecognitionOutput",
+    "Image2TextOutput",
+]
+
+
 @dataclass
 class ModelOutput:
     """
     Base class for all models' prediction outputs (`model.predict()`/`model.post_process()` outputs).
 
     Note that prediction outputs must all be a list of `ModelOutput` objects since we consider only batch inferences.
```

### Comparing `hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py` & `hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py` & `hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py` & `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py` & `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from ....constants import Backends
 from ....registry import register_model
 from ....utils import is_backend_available, load_audio_files, shift_tokens_right
 from ...model import Model
 from ...model_outputs import SpeechRecognitionOutput
 from .whisper_speech_recognition_config import WhisperSpeechRecognitionConfig
 
+
 if is_backend_available(Backends.TRANSFORMERS):
-    from transformers import WhisperConfig, WhisperForConditionalGeneration, GenerationConfig
+    from transformers import GenerationConfig, WhisperConfig, WhisperForConditionalGeneration
 
 _required_backends = [
     Backends.TRANSFORMERS,
     Backends.TOKENIZERS,
     Backends.LIBROSA,
 ]
 
@@ -102,15 +103,15 @@
         is_multilingual=None,
         prompt_ids=None,
         **kwargs,
     ):
         if generation_config is not None:
             self.config.generation_config.update(**generation_config)
 
-        generation_config = GenerationConfig(**self.config.generation_config)
+        generation_config = GenerationConfig(**self.config.generation_config.dict())
 
         generation_outputs = self.whisper.generate(
             input_features=input_features,
             generation_config=generation_config,
             logits_processor=logits_processor,
             stopping_criteria=stopping_criteria,
             prefix_allowed_tokens_fn=prefix_allowed_tokens_fn,
```

### Comparing `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py` & `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 from typing import List
 
 from ....configs import ModelConfig
 
 
 @dataclass
-class WhisperSpeechRecognitionGenerationConfig(ModelConfig):
+class WhisperSpeechRecognitionGenerationConfig:
     alignment_heads: List[List[int]] = None
     begin_suppress_tokens: List[int] = field(default_factory=lambda: [220, 50256])
     bos_token_id: int = 50257
     decoder_start_token_id: int = 50258
     eos_token_id: int = 50257
     forced_decoder_ids: List[List[int]] = field(default_factory=lambda: [[1, None], [2, 50359]])
     is_multilingual: bool = True
@@ -18,14 +18,17 @@
     no_timestamps_token_id: int = 50363
     pad_token_id: int = 50257
     prev_sot_token_id: int = 50361
     return_timestamps: int = False
     suppress_tokens: List[int] = None
     task_to_id: dict[str, int] = field(default_factory=lambda: {"transcribe": 50359, "translate": 50358})
 
+    def dict(self):
+        return asdict(self)
+
 
 @dataclass
 class WhisperSpeechRecognitionConfig(ModelConfig):
     name = "whisper_speech_recognition"
     vocab_size: int = 51865
     num_mel_bins: int = 80
     encoder_layers: int = 6
```

### Comparing `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py` & `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py` & `hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py` & `hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation.py` & `hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation_config.py` & `hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/audio_feature_extractor.py` & `hezar-0.38.0/hezar/preprocessors/audio_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/image_processor.py` & `hezar-0.38.0/hezar/preprocessors/image_processor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/preprocessor.py` & `hezar-0.38.0/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/text_normalizer.py` & `hezar-0.38.0/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.38.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.38.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.38.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/registry.py` & `hezar-0.38.0/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/trainer/metrics_handlers.py` & `hezar-0.38.0/hezar/trainer/metrics_handlers.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/trainer/trainer.py` & `hezar-0.38.0/hezar/trainer/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from __future__ import annotations
 
 import math
 import os
-import random
+import tempfile
 from typing import Any, Callable, Dict, Tuple
 
-import numpy as np
 import pandas as pd
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
 from tqdm.auto import tqdm
 
 from ..configs import TrainerConfig
 from ..constants import (
     DEFAULT_DATASET_CONFIG_FILE,
+    DEFAULT_OPTIMIZER_FILE,
     DEFAULT_TRAINER_CONFIG_FILE,
     DEFAULT_TRAINER_CSV_LOG_FILE,
     DEFAULT_TRAINER_STATE_FILE,
     DEFAULT_TRAINER_SUBFOLDER,
     HEZAR_CACHE_DIR,
     TQDM_BAR_FORMAT,
     Backends,
     LRSchedulerType,
     OptimizerType,
     TaskType,
 )
-from ..data.datasets import Dataset
+from ..data import Dataset, SlicedSampler
 from ..models import Model
 from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import (
     Logger,
     colorize_text,
     is_backend_available,
     sanitize_function_parameters,
-    verify_dependencies,
     set_seed,
+    verify_dependencies,
 )
 from .metrics_handlers import (
     Image2TextMetricHandler,
     MetricsHandler,
     SequenceLabelingMetricsHandler,
     SpeechRecognitionMetricsHandler,
     TextClassificationMetricsHandler,
@@ -102,14 +102,15 @@
     """
 
     trainer_subfolder = DEFAULT_TRAINER_SUBFOLDER
     trainer_config_file = DEFAULT_TRAINER_CONFIG_FILE
     trainer_csv_log_file = DEFAULT_TRAINER_CSV_LOG_FILE
     dataset_config_file = DEFAULT_DATASET_CONFIG_FILE
     trainer_state_file = DEFAULT_TRAINER_STATE_FILE
+    optimizer_file = DEFAULT_OPTIMIZER_FILE
     default_optimizer = OptimizerType.ADAM
     default_lr_scheduler = None
     _required_backends = [Backends.ACCELERATE]
 
     def __init__(
         self,
         model: Model = None,
@@ -122,143 +123,190 @@
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
         accelerator: "Accelerator" = None,
     ):
         # Check if all required dependencies are installed
         verify_dependencies(self._required_backends)
 
-        # Setup logger
-        self.logger = get_distributed_logger(__name__)
-
         # Configuration
         self.config = config
         self.device = "cuda" if torch.cuda.is_available() and not self.config.use_cpu else "cpu"
 
+        # Setup accelerated objects if possible
+        self.accelerator = accelerator
+        if self.accelerator is None:
+            self.accelerator = Accelerator(
+                mixed_precision=self.config.mixed_precision,
+                cpu=True if self.device == "cpu" else False,
+                step_scheduler_with_optimizer=False,
+                gradient_accumulation_steps=self.config.gradient_accumulation_steps,
+            )
+
+        # Setup logger
+        self.logger = get_distributed_logger(__name__)
+
+        # Configure datasets and data loaders
+        self.train_dataset = train_dataset
+        self.eval_dataset = eval_dataset
+        self.data_collator = data_collator or self.train_dataset.data_collator
+        self.steps_in_epoch = math.ceil(len(self.train_dataset) / self.config.batch_size)
+        self.total_steps = self.steps_in_epoch * self.config.num_epochs
+        self.config.save_steps = self.steps_in_epoch if not self.config.save_steps else self.config.save_steps
+        self.saves_in_epoch = math.floor(self.steps_in_epoch / self.config.save_steps)
+
+        # Setup checkpoint and state handler
+        self.checkpoints_dir = os.path.join(self.config.output_dir, self.config.checkpoints_dir)
+        self.state = self._create_trainer_state(self.config.resume_from_checkpoint)
+        self.logs_dir = self.state.logs_dir
+
         # Set determinism
         set_seed(self.config.seed)
 
         # Setup model and preprocessor(s)
         self.model = self._setup_model(model)
-        if self.model.preprocessor is None:
+        if model.preprocessor is None:
             if preprocessor is not None:
-                self.model.preprocessor = preprocessor
+                model.preprocessor = preprocessor
             else:
                 raise ValueError(
                     "You must set a preprocessor for the model or pass the preprocessor parameter to the Trainer!"
                 )
 
-        # Configure datasets and data loaders
-        self.train_dataset = train_dataset
-        self.eval_dataset = eval_dataset
-        self.data_collator = data_collator or self.train_dataset.data_collator
-        self.train_dataloader, self.eval_dataloader = self._setup_dataloaders()
-        self.total_steps = len(self.train_dataloader) * self.config.num_epochs
-        self.config.save_steps = len(self.train_dataloader) if not self.config.save_steps else self.config.save_steps
-        self.save_steps_per_epoch = math.ceil(len(self.train_dataloader) / self.config.save_steps)
-
         # Setup optimizer and (optionally) lr scheduler
-        self.optimizer, self.lr_scheduler = self._setup_optimizers(optimizer, lr_scheduler)
-
-        # Setup accelerated objects if possible
-        self.accelerator = accelerator
-        if self.accelerator is None:
-            self.accelerator = Accelerator(
-                mixed_precision=self.config.mixed_precision,
-                cpu=True if self.device == "cpu" else False,
-                step_scheduler_with_optimizer=True if self.lr_scheduler is not None else False,
-                gradient_accumulation_steps=self.config.gradient_accumulation_steps,
-            )
+        self.optimizer, self.lr_scheduler = self._create_optimizers(optimizer, lr_scheduler)
 
-        self.model, self.optimizer, self.lr_scheduler, self.train_dataloader, self.eval_dataloader = (
-            self.accelerator.prepare(
-                self.model,
-                self.optimizer,
-                self.lr_scheduler,
-                self.train_dataloader,
-                self.eval_dataloader,
-            )
+        self.model, self.optimizer, self.lr_scheduler = self.accelerator.prepare(
+            self.model, self.optimizer, self.lr_scheduler
         )
 
         # Setup metrics handler and inner trackers for the trainer
-        self.metrics_handler = metrics_handler or self._setup_metrics_handler()
-
-        # Configure checkpoints and logging directories
-        self.logs_dir = resolve_logdir(os.path.join(self.config.output_dir, self.config.logs_dir))
-        self.checkpoints_dir = os.path.join(self.config.output_dir, self.config.checkpoints_dir)
+        self.metrics_handler = metrics_handler or self._create_metrics_handler()
 
         # Setup logging properties
         self.tensorboard = SummaryWriter(log_dir=self.logs_dir)
         self.csv_logger = CSVLogger(logs_dir=self.logs_dir, csv_filename=self.trainer_csv_log_file)
 
-        # Configure trainer state
-        self.state = TrainerState(
-            epoch=1,
-            total_epochs=self.config.num_epochs,
-            metric_for_best_checkpoint=self.config.metric_for_best_model,
-            logs_dir=self.logs_dir,
-        )
+    def _create_trainer_state(self, checkpoint: str = None):
+        """
+        Create Trainer's state attribute.
+
+        Args:
+            checkpoint: Optional checkpoint path or bool value to load the state from there
+
+        Returns:
+            A TrainerState object
+        """
+        trainer_state_path = os.path.join(self.checkpoints_dir, self.trainer_state_file)
+        if checkpoint is not None and os.path.isfile(trainer_state_path):
+            state = TrainerState.load(trainer_state_path)
+            # Overwrite some fields if checkpoint is a path
+            if os.path.isdir(checkpoint):
+                step = os.path.basename(checkpoint)
+                state.global_step = int(step) if step.isdigit() else self.state.global_step
+                state.epoch = math.ceil(state.global_step / self.steps_in_epoch)
+                state.epoch_step = state.global_step % self.steps_in_epoch
+                if state.epoch_step == 0:
+                    state.epoch += 1
+        else:
+            state = TrainerState(
+                epoch=1,
+                total_epochs=self.config.num_epochs,
+                metric_for_best_checkpoint=self.config.metric_for_best_model,
+                logs_dir=resolve_logdir(os.path.join(self.config.output_dir, self.config.logs_dir)),
+            )
+        return state
+
+    def _resolve_checkpoint_path(self, checkpoint: str | bool):
+        if isinstance(checkpoint, bool) and checkpoint:
+            checkpoint_path = os.path.join(self.checkpoints_dir, str(self.state.global_step))
+        elif os.path.isdir(checkpoint):
+            checkpoint_path = checkpoint
+        else:
+            raise ValueError(f"Checkpoint `{checkpoint}` is either invalid or does not exist!")
+
+        return checkpoint_path
 
     def _setup_model(self, model: Model) -> Model:
         """
-        Download the model from HuggingFace Hub if `init_weights_from` is given in the config. Load the model to the
-        device and return it.
+        Create and load the weights for the model. The weights will be loaded to the model depending
+        on `config.resume_from_checkpoint` or `config.init_weights_from`.
         """
         if model is None:
             raise ValueError("`model` must be given to the Trainer!")
-        hub_path = self.config.init_weights_from
-        if hub_path is not None:
-            if os.path.isdir(hub_path):
-                model_path = os.path.join(hub_path, model.model_filename)
-            else:
-                model_path = hf_hub_download(
-                    hub_path,
-                    filename=model.model_filename,
-                    cache_dir=HEZAR_CACHE_DIR,
-                    resume_download=True,
-                )
-            model.load_state_dict(torch.load(model_path))
+
+        # Maybe load from checkpoint
+        if self.config.resume_from_checkpoint is not None:
+            checkpoint_path = self._resolve_checkpoint_path(self.config.resume_from_checkpoint)
+            model_path = os.path.join(checkpoint_path, model.model_filename)
+            if os.path.isdir(checkpoint_path) and os.path.isfile(model_path):
+                model.load_state_dict(torch.load(model_path))
+                self.logger.info(f"Resuming training from checkpoint at `{checkpoint_path}`")
+        # Maybe load from pretrained weights locally or from a hub repo
+        elif self.config.init_weights_from is not None and self.state.global_step == 0 and self.state.epoch == 1:
+            if self.config.init_weights_from is not None:
+                if os.path.isdir(self.config.init_weights_from):
+                    model_path = os.path.join(self.config.init_weights_from, model.model_filename)
+                else:
+                    model_path = hf_hub_download(
+                        self.config.init_weights_from,
+                        filename=model.model_filename,
+                        cache_dir=HEZAR_CACHE_DIR,
+                        resume_download=True,
+                    )
+                model.load_state_dict(torch.load(model_path))
+
         return model
 
-    def _setup_dataloaders(self) -> Tuple[DataLoader, DataLoader | None]:
+    def create_dataloaders(self) -> Tuple[DataLoader, DataLoader | None]:
         """
         Set up data loaders (train/eval) and return them.
 
         Returns:
              A tuple of train and eval dataloaders
         """
         if self.train_dataset is not None:
+            # Handle resuming
+            if self.state.epoch_step != 0:
+                start_index = self.state.epoch_step * self.config.batch_size
+                sampler = SlicedSampler(self.train_dataset, start_index=start_index)
+                shuffle = False
+            else:
+                sampler = None
+                shuffle = self.config.dataloader_shuffle
+
             train_dataloader = DataLoader(
                 dataset=self.train_dataset,
                 batch_size=self.config.batch_size,
                 collate_fn=self.data_collator,
+                sampler=sampler,
                 num_workers=self.config.num_dataloader_workers,
                 drop_last=self.config.dataloader_drop_last,
-                shuffle=self.config.dataloader_shuffle,
+                shuffle=shuffle,
             )
         else:
             raise ValueError("Cannot create train dataloader because `train_dataset` is not given!")
+
         if self.eval_dataset is not None:
             eval_dataloader = DataLoader(
                 dataset=self.eval_dataset,
                 batch_size=self.config.eval_batch_size or self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
                 drop_last=self.config.dataloader_drop_last,
                 shuffle=self.config.dataloader_shuffle,
             )
         else:
-            self.logger.warning(
-                "Cannot create eval dataloader because `eval_dataset` is not given to the Trainer! "
-                "Setting eval_dataloader to None..."
-            )
-            eval_dataloader = None
+            raise ValueError("Cannot create evaluation dataloader because `eval_dataset` is not given!")
+
+        if self.accelerator is not None:
+            train_dataloader, eval_dataloader = self.accelerator.prepare(train_dataloader, eval_dataloader)
 
         return train_dataloader, eval_dataloader
 
-    def _setup_optimizers(self, optimizer: torch.optim.Optimizer = None, lr_scheduler=None):
+    def _create_optimizers(self, optimizer: torch.optim.Optimizer = None, lr_scheduler=None):
         """
         Set up the optimizer and lr lr_scheduler if they're not already given
 
         Args:
             optimizer: If None do nothing and return it, otherwise build it using the train config
             lr_scheduler: If None do nothing and return it, otherwise build it using the train config
 
@@ -268,89 +316,40 @@
         if optimizer is None:
             optimizer_type = self.config.optimizer or self.default_optimizer
             optimizer = optimizers[optimizer_type](
                 self.model.parameters(),
                 lr=self.config.learning_rate,
                 weight_decay=self.config.weight_decay,
             )
+            if self.config.resume_from_checkpoint is not None:
+                checkpoint_path = self._resolve_checkpoint_path(self.config.resume_from_checkpoint)
+                optimizer_path = os.path.join(checkpoint_path, self.optimizer_file)
+                if os.path.isdir(checkpoint_path) and os.path.isfile(optimizer_path):
+                    optimizer.load_state_dict(torch.load(optimizer_path))
 
             if lr_scheduler is None:
                 scheduler_name = self.config.lr_scheduler or self.default_lr_scheduler
                 scheduler_kwargs = self.config.lr_scheduler_kwargs or {}
                 if scheduler_name is None:
                     lr_scheduler = None
                 else:
                     lr_scheduler = lr_schedulers[scheduler_name](optimizer, **scheduler_kwargs, verbose=True)
         return optimizer, lr_scheduler
 
-    def _setup_metrics_handler(self):
+    def _create_metrics_handler(self):
         """
         Setup MetricsHandler instance for the trainer
 
         Returns:
             A MetricsHandler subclass instance based on self.config.task
         """
         metrics_handler_cls = task_to_metrics_handlers_mapping[self.config.task]
         metrics_handler = metrics_handler_cls(metrics=self.config.metrics, trainer=self)  # noqa
         return metrics_handler
 
-    def load_from_checkpoint(self, checkpoint: str | bool = True, load_best: bool = False):
-        """
-        Load trainer states like model weights, optimizer, etc. from a checkpoint
-
-        Args:
-            checkpoint: Path to checkpoint directory
-            load_best: Whether to load the best checkpoint or not, if False, loads the latest checkpoint
-        """
-        if os.path.isdir(checkpoint) and load_best:
-            self.logger.warning("The `load_best` parameter has no effect when `checkpoint` is a path!")
-
-        # Load trainer state file if available
-        state_path = os.path.join(self.checkpoints_dir, self.trainer_state_file)
-        if os.path.isfile(state_path):
-            self.state = TrainerState.load(state_path)
-
-        # If checkpoint is True instead of a path to the checkpoint, load the latest of the best checkpoint
-        if isinstance(checkpoint, bool):
-            if load_best:
-                checkpoint = os.path.join(self.checkpoints_dir, str(self.state.best_checkpoint))
-            else:
-                # Get the most recent checkpoint based on global step
-                checkpoint = os.path.join(
-                    self.checkpoints_dir,
-                    str(self.state.global_step).zfill(len(str(self.total_steps))),
-                )
-
-        # Load checkpoint file and update trainer state based on the checkpoint file
-        if os.path.isdir(checkpoint):
-            # Figure out the step and epoch number
-            step = os.path.basename(checkpoint)
-            self.state.global_step = int(step) if step.isdigit() else self.state.global_step
-            self.state.epoch = math.ceil(self.state.global_step / len(self.train_dataloader)) - 1
-            self.state.epoch_step = self.state.global_step % len(self.train_dataloader)
-            if self.state.epoch_step == 0:
-                self.state.epoch += 1
-            # Load model's state dict
-            model_path = os.path.join(checkpoint, self.model.model_filename)
-            if os.path.isfile(model_path):
-                self.model.load_state_dict(torch.load(model_path))
-                self.model = self.accelerator.prepare(self.model)
-                self.logger.info(f"Successfully loaded checkpoint from `{checkpoint}` ")
-            else:
-                raise FileNotFoundError(
-                    f"Could not find `{self.model.model_filename}` at `{os.path.dirname(model_path)}`!\n"
-                )
-        else:
-            self.logger.warning(
-                f"{checkpoint} does not seem to be a valid checkpoint!"
-            )
-
-        if self.state.global_step >= self.total_steps:
-            self.logger.warning(f"The checkpoint at `{checkpoint}` belongs to the last training step!")
-
     def load_csv_logs(self, logs_dir=None):
         """
         Load the CSV log file
         Args:
             logs_dir: Path to logs directory, defaults to self.config.logs_dir
 
         Returns:
@@ -498,29 +497,23 @@
         Returns:
             Metrics averages through the full iteration
         """
         losses_sum = 0
         self.model.train()
         with tqdm(
             self.train_dataloader,
+            initial=self.state.epoch_step,
             unit="batch",
             desc=f"Epoch: {epoch_num}/{self.config.num_epochs} ",
             bar_format=TQDM_BAR_FORMAT,
             ascii=" #",
             disable=not self.accelerator.is_local_main_process,
         ) as iterator:
-            for step, input_batch in enumerate(iterator):
-                # TODO make this more efficient in a way that the data loader skips batches without iterating them
-                # Skip the first batches to reach `epoch_step`
-                if step < self.state.epoch_step:
-                    iterator.set_description(desc="Skipping already trained batches...")
-                    continue
-                elif step == self.state.epoch_step:
-                    iterator.set_description(desc=f"Epoch: {epoch_num}/{self.config.num_epochs} ")
-
+            for input_batch in iterator:
+                step = self.state.global_step
                 # Prepare inputs
                 input_batch = self.prepare_input_batch(input_batch)
 
                 # Training on one batch
                 with self.accelerator.accumulate(self.model):
                     outputs = self.training_step(input_batch)
                     # Optimization step
@@ -626,26 +619,28 @@
         [_print_info_line(k, v) for k, v in info.items()]
         # Footer
         self.accelerator.print(f"\n{colorize_text(footer, 'bold')}\n")
 
     def train(self, resume_from_checkpoint: str | bool = None):
         """
         The full training process like training, evaluation, logging and saving model checkpoints.
-
-        Args:
-            resume_from_checkpoint: Resume from checkpoint path (if value is a path) or automatically load from the
-            latest checkpoint (if value is True)
         """
-        if resume_from_checkpoint:
-            self.load_from_checkpoint(resume_from_checkpoint)
+        if resume_from_checkpoint is not None:
+            raise ValueError(
+                "Setting `resume_from_checkpoint` in `Trainer.train(resume_from_checkpoint=...)` is deprecated. "
+                "You have to set it in the trainer's config!"
+            )
 
         self.print_info()
 
         for epoch in range(self.state.epoch, self.config.num_epochs + 1):
             self.accelerator.print()
+            self.state.epoch = epoch
+
+            self.train_dataloader, self.eval_dataloader = self.create_dataloaders()
 
             # Train on the whole training set
             training_results = self.inner_training_loop(epoch)
 
             # Save checkpoint
             if self.accelerator.is_local_main_process:
                 if self.config.save_enabled:
@@ -665,15 +660,15 @@
 
             # Update trainer state
             self.state.epoch = epoch
             self.state.epoch_step = 0
             self.state.update_best_results(
                 metric_value=all_logs[self.config.metric_for_best_model],
                 objective=self.metrics_handler.objective,
-                step=epoch,
+                step=self.state.global_step,
             )
 
             # Log everything
             self.log(all_logs, epoch)
 
         self.logger.info("Training done!")
 
@@ -694,78 +689,87 @@
                 self.trainer_state_file,
             )
         )
 
     def save(
         self,
         path: str,
-        config_filename=None,
-        model_filename=None,
-        model_config_filename=None,
-        subfolder=None,
-        dataset_config_file=None,
+        config_filename: str = None,
+        model_filename: str = None,
+        model_config_filename: str = None,
+        subfolder: str = None,
+        dataset_config_file: str = None,
+        optimizer_file: str = None,
     ):
         """
         Save the trainer and relevant files to a path.
 
         Files to save are train config, model weights, model config, preprocessor files and preprocessor config.
 
         Args:
             path: A directory to save everything
-            config_filename: Config filename
+            config_filename: Config file name
             model_filename: Model file name
             model_config_filename: Model config file name
             subfolder: Optional sub-folder
-            dataset_config_file: Dataset config filename
+            dataset_config_file: Dataset config file name
+            optimizer_file: Optimizer state file name
         """
         config_filename = config_filename or self.trainer_config_file
         subfolder = subfolder or self.trainer_subfolder
         dataset_config_file = dataset_config_file or self.dataset_config_file
+        optimizer_file = optimizer_file or self.optimizer_file
 
         self.config.save(path, filename=config_filename, subfolder=subfolder)
         self.model.save(path, filename=model_filename, config_filename=model_config_filename)
+        torch.save(self.optimizer, os.path.join(path, subfolder, optimizer_file))
         if isinstance(self.train_dataset, Dataset):
             self.train_dataset.config.save(path, filename=dataset_config_file, subfolder=subfolder)
         else:
             self.logger.warning(
                 "The dataset passed to the Trainer is not a `hezar.data.Dataset` instance so that no dataset config"
                 " will be saved!"
             )
 
     def push_to_hub(
         self,
         repo_id: str,
         config_filename: str = None,
         push_model: bool = True,
+        push_optimizer: bool = True,
         push_logs: bool = True,
         model_filename: str = None,
         model_config_filename: str = None,
+        optimizer_filename: str = None,
         subfolder: str = None,
         dataset_config_filename: str = None,
         commit_message: str = None,
         private: bool = False,
     ):
         """
         Push everything to the Hub
 
         Args:
             repo_id: Path to hub
             config_filename: Trainer config file name
-            push_model: Whether to push the model or not
-            push_logs: Whether to push training logs or not
+            push_model: Whether to push the model
+            push_optimizer: Whether to push the optimizer
+            push_logs: Whether to push training logs
             model_filename: Model file name
+            optimizer_filename: Optimizer file name
             model_config_filename: Model config file name
             subfolder: Path to Trainer files
             dataset_config_filename: Dataset config file name
             commit_message: Commit message for the push
             private: Whether to create a private repo if it doesn't exist already
         """
         config_filename = config_filename or self.trainer_config_file
         subfolder = subfolder or self.trainer_subfolder
         dataset_config_file = dataset_config_filename or self.dataset_config_file
+        optimizer_filename = optimizer_filename or self.optimizer_file
 
         # create remote repo
         create_repo(repo_id, repo_type="model", exist_ok=True, private=private)
 
         if not commit_message:
             commit_message = "Hezar: Upload training files"
 
@@ -781,24 +785,35 @@
             repo_id,
             filename=dataset_config_file,
             subfolder=subfolder,
             private=private,
             commit_message=commit_message
         )
 
-        # upload model
+        # Upload model
         if push_model:
             self.model.push_to_hub(
                 repo_id,
                 filename=model_filename,
                 config_filename=model_config_filename,
                 commit_message=commit_message,
                 private=private,
             )
 
+        # Upload optimizer state
+        if push_optimizer:
+            optimizer_path = os.path.join(tempfile.mkdtemp(), optimizer_filename)
+            torch.save(self.optimizer.state_dict(), optimizer_path)
+            upload_file(
+                path_or_fileobj=optimizer_path,
+                path_in_repo=os.path.join(self.trainer_subfolder, optimizer_filename),
+                repo_id=repo_id,
+                commit_message=commit_message,
+            )
+        # Upload logs
         if push_logs:
             upload_file(
                 path_or_fileobj=self.csv_logger.save_path,
                 path_in_repo=os.path.join(self.trainer_subfolder, self.trainer_csv_log_file),
                 repo_id=repo_id,
                 commit_message=commit_message,
             )
```

### Comparing `hezar-0.37.0/hezar/trainer/trainer_utils.py` & `hezar-0.38.0/hezar/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/audio_utils.py` & `hezar-0.38.0/hezar/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/common_utils.py` & `hezar-0.38.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/data_utils.py` & `hezar-0.38.0/hezar/utils/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
 
 from omegaconf import DictConfig
 
 from ..constants import PaddingType
 from .logging import Logger
 
+
 if TYPE_CHECKING:
     import torch
 
 __all__ = [
     "convert_batch_dict_dtype",
     "resolve_inputs_length_for_padding",
     "pad_batch_items",
@@ -233,14 +234,15 @@
         else:
             config[k] = v
 
     return config
 
 
 def set_seed(seed):
-    import torch
-    import numpy as np
     import random
 
+    import numpy as np
+    import torch
+
     torch.manual_seed(seed)
     np.random.seed(seed)
     random.seed(seed)
```

### Comparing `hezar-0.37.0/hezar/utils/file_utils.py` & `hezar-0.38.0/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/hub_utils.py` & `hezar-0.38.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/image_utils.py` & `hezar-0.38.0/hezar/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/integration_utils.py` & `hezar-0.38.0/hezar/utils/integration_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/logging.py` & `hezar-0.38.0/hezar/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/hezar/utils/registry_utils.py` & `hezar-0.38.0/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.37.0/pyproject.toml` & `hezar-0.38.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.37.0"
+version = "0.38.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!"
 license = "Apache-2.0"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
 readme = ["README.md"]
 keywords = ["packaging", "poetry"]
 documentation = "https://hezarai.github.io/hezar/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 exclude = [
     "docs",
     "examples",
@@ -59,15 +59,15 @@
 vision = ["pillow"]
 embeddings = ["gensim", "numpy", "scipy"]
 dev = ["pytest", "ruff", "sphinx", "myst-parser", "furo", "sphinx-copybutton"]
 all = ["numpy", "gensim", "seqeval", "jiwer", "soundfile", "librosa", "pillow", "nltk", "rouge_score", "scipy"]
 
 [tool.black]
 line-length = 120
-target-version = ['py39', 'py310', 'py311']
+target-version = ['py310', 'py311', 'py312']
 
 [tool.ruff]
 ignore = ["C901", "E501", "E741", "W605", "F403", "F405"]
 select = ["C", "E", "F", "I", "W"]
 line-length = 120
 
 [tool.ruff.per-file-ignores]
```

### Comparing `hezar-0.37.0/PKG-INFO` & `hezar-0.38.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.37.0
+Version: 0.38.0
 Summary: Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!
 Home-page: https://github.com/hezarai
 License: Apache-2.0
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

