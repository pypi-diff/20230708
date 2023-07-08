# Comparing `tmp/hezar-0.14.0.tar.gz` & `tmp/hezar-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.14.0.tar", max compression
+gzip compressed data, was "hezar-0.14.1.tar", max compression
```

## Comparing `hezar-0.14.0.tar` & `hezar-0.14.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1065 2023-07-03 15:56:20.320494 hezar-0.14.0/LICENSE
--rw-r--r--   0        0        0     4406 2023-07-03 15:56:20.320494 hezar-0.14.0/README.md
--rw-r--r--   0        0        0      238 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/__init__.py
--rw-r--r--   0        0        0     6481 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/builders.py
--rw-r--r--   0        0        0    10446 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/configs.py
--rw-r--r--   0        0        0     1110 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1608 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4576 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3701 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      282 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     2679 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2813 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     2943 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      104 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/nfkc.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/nfkd.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/normalizer.py
--rw-r--r--   0        0        0     2218 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      298 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4623 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5181 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    18892 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4215 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8244 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/registry.py
--rw-r--r--   0        0        0       29 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0    13853 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1773 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      135 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0     3468 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/config_utils.py
--rw-r--r--   0        0        0      482 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     2773 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1579 2023-07-03 15:56:20.324494 hezar-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     6783 1970-01-01 00:00:00.000000 hezar-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 07:53:38.051829 hezar-0.14.1/LICENSE
+-rw-r--r--   0        0        0     4427 2023-07-08 07:53:38.051829 hezar-0.14.1/README.md
+-rw-r--r--   0        0        0      238 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/__init__.py
+-rw-r--r--   0        0        0     4471 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/builders.py
+-rw-r--r--   0        0        0    10536 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/configs.py
+-rw-r--r--   0        0        0     1216 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4576 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3701 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      282 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0     9544 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     2679 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2813 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     2943 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/nfkc.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/nfkd.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/normalizer.py
+-rw-r--r--   0        0        0     2218 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      298 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4623 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5181 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    18892 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4215 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     7771 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/registry.py
+-rw-r--r--   0        0        0       29 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0    14619 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1773 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      135 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/__init__.py
+-rw-r--r--   0        0        0     3468 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/config_utils.py
+-rw-r--r--   0        0        0      482 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     2773 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1579 2023-07-08 07:53:38.055829 hezar-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 hezar-0.14.1/PKG-INFO
```

### Comparing `hezar-0.14.0/LICENSE` & `hezar-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/README.md` & `hezar-0.14.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 
 # this is our Hub repo
 model_path = "hezarai/bert-fa-sentiment-digikala-snappfood"
 # load model and tokenizer
 model = Model.load(model_path)
 tokenizer = Tokenizer.load(model_path)
 # tokenize inputs
-example = ["کتابخانه هزار، بهترین کتابخانه هوش مصنوعیه"]
+example = ["هزار، کتابخانه‌ای کامل برای به کارگیری آسان هوش مصنوعی"]
 inputs = tokenizer(example, return_tensors="pt")
 # inference
 outputs = model.predict(inputs)
 # print outputs
 print(outputs)
 ```
 ```commandline
-{'labels': ['positive'], 'probs': [0.9960528612136841]}
+{'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
 ### Build models from scratch
 Wanna use models without any pretrained weights? Easy!
 
 Build a raw BERT-based model for text classification with a single line of code!
 ```python
 from hezar import build_model
```

### Comparing `hezar-0.14.0/hezar/configs.py` & `hezar-0.14.1/hezar/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,16 @@
     Base dataclass for all trainer configs
     """
     name: str = field(default=None, metadata={"help": "The trainer's key in the trainers_registry"})
     config_type: str = "train"
     task: TaskType = None
     device: str = "cuda"
     init_weights_from: str = None
+    dataset_config: Union[DatasetConfig, Dict] = None
+    num_dataloader_workers: int = 0
     seed: int = 42
     optimizer: Union[Dict[str, Any], OptimizerConfig] = None
     batch_size: int = None
     use_amp: bool = False
     metrics: Dict[str, Dict] = field(default_factory=dict)
     num_epochs: int = None
     save_freq: int = 1
```

### Comparing `hezar-0.14.0/hezar/constants.py` & `hezar-0.14.1/hezar/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,7 +29,14 @@
     IMAGE2TEXT = "image2text"
     LANGUAGE_MODELING = "language_modeling"
     SEQUENCE_LABELING = "sequence_labeling"
     SPEECH_RECOGNITION = "speech_recognition"
     TEXT_CLASSIFICATION = "text_classification"
     TEXT_DETECTION = "text_detection"
     SEQ2SEQ = "seq2seq"
+
+
+class SplitType(Enum):
+    TRAIN = "train"
+    EVAL = "eval"
+    VALID = "validation"
+    TEST = "test"
```

### Comparing `hezar-0.14.0/hezar/data/data_collators.py` & `hezar-0.14.1/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/data/datasets/dataset.py` & `hezar-0.14.1/hezar/data/datasets/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Optional, Union
 
 from torch.utils.data import Dataset as TorchDataset
 
 from ...configs import DatasetConfig
-from ...constants import DEFAULT_DATASET_CONFIG_FILE
+from ...constants import DEFAULT_DATASET_CONFIG_FILE, SplitType
 from ...utils import get_module_class
 
 
 class Dataset(TorchDataset):
     """
     Base class for all datasets in Hezar.
 
@@ -17,27 +17,28 @@
         **kwargs:
     """
     config_filename = DEFAULT_DATASET_CONFIG_FILE
 
     def __init__(self, config: DatasetConfig, **kwargs):
         self.config = config.update(kwargs)
         self.preprocessor = None
+        self.data_collator = None
 
     def __len__(self):
         raise NotImplementedError
 
     def __getitem__(self, index):
         raise NotImplementedError
 
     @classmethod
     def load(
         cls,
         hub_path: Union[str, os.PathLike],
         config_filename: Optional[str] = None,
-        split: Optional[str] = None,
+        split: Optional[Union[str, SplitType]] = None,
         **kwargs,
     ):
         """
         Load the dataset from hub.
 
         Args:
             hub_path: Path to dataset from hub or locally
```

### Comparing `hezar-0.14.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.14.1/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.14.1/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/data/utils/data_utils.py` & `hezar-0.14.1/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/embeddings/embedding.py` & `hezar-0.14.1/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/embeddings/fasttext.py` & `hezar-0.14.1/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/embeddings/word2vec.py` & `hezar-0.14.1/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/model.py` & `hezar-0.14.1/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/preprocessors/preprocessor.py` & `hezar-0.14.1/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.14.1/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.14.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.14.1/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.14.1/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/registry.py` & `hezar-0.14.1/hezar/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 
 Note: In case of adding a new registry container, make sure to add to `__all__` below!
 """
 
 from dataclasses import dataclass
 from typing import Dict, Type
 
-from torch import nn, optim
-
 from .configs import DatasetConfig, EmbeddingConfig, ModelConfig, PreprocessorConfig, TrainConfig
 from .utils import get_logger
 
 
 __all__ = [
     "register_model",
     "register_preprocessor",
@@ -43,41 +41,23 @@
 logger = get_logger(__name__)
 
 
 @dataclass
 class Registry:
     module_class: type
     config_class: type
-    doc: str
+    doc: str = None
 
 
 models_registry: Dict[str, Registry] = {}
 preprocessors_registry: Dict[str, Registry] = {}
 datasets_registry: Dict[str, Registry] = {}
 embeddings_registry: Dict[str, Registry] = {}
 trainers_registry: Dict[str, Registry] = {}
 
-criterions_registry = {
-    "bce": nn.BCELoss,
-    "bce_with_logits": nn.BCEWithLogitsLoss,
-    "nll": nn.NLLLoss,
-    "cross_entropy": nn.CrossEntropyLoss,
-    "mse": nn.MSELoss,
-    "ctc": nn.CTCLoss,
-}
-optimizers_registry = {
-    "adam": optim.Adam,
-    "adamw": optim.AdamW,
-    "sgd": optim.SGD,
-}
-lr_schedulers_registry = {
-    "reduce_on_plateau": optim.lr_scheduler.ReduceLROnPlateau,
-    "cosine_lr": optim.lr_scheduler.CosineAnnealingLR,
-}
-
 
 def register_model(model_name: str, config_class: Type[ModelConfig]):
     """
     A class decorator that adds the model class and the config class to the `models_registry`
 
     Args:
         model_name: Model's registry name e.g, `bert_sequence_labeling`
```

### Comparing `hezar-0.14.0/hezar/trainers/trainer.py` & `hezar-0.14.1/hezar/trainers/trainer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 import random
 import tempfile
-from typing import Dict
+from typing import Dict, Optional, Union
 
 import numpy as np
-import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_folder
+import torch
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
 from torchmetrics import Accuracy, F1Score, Precision
 from tqdm import tqdm
 
-from ..builders import build_optimizer, build_scheduler
 from ..configs import LRSchedulerConfig, OptimizerConfig, TrainConfig
 from ..constants import (
     DEFAULT_DATASET_CONFIG_FILE,
     DEFAULT_TRAINER_CONFIG_FILE,
     DEFAULT_TRAINER_SUBFOLDER,
     HEZAR_CACHE_DIR,
     TQDM_BAR_FORMAT,
@@ -30,14 +29,24 @@
 
 METRICS_MAP = {
     "accuracy": Accuracy,
     "f1": F1Score,
     "precision": Precision,
 }
 
+optimizers = {
+    "adam": torch.optim.Adam,
+    "adamw": torch.optim.AdamW,
+    "sgd": torch.optim.SGD,
+}
+lr_schedulers = {
+    "reduce_on_plateau": torch.optim.lr_scheduler.ReduceLROnPlateau,
+    "cosine_lr": torch.optim.lr_scheduler.CosineAnnealingLR,
+}
+
 
 class Trainer:
     """
     A general but fully featured model trainer/evaluator for Hezar models.
 
     Args:
         model ([`Model`] or `torch.nn.Module`): The main model to train and evaluate
@@ -62,74 +71,86 @@
         eval_dataset: Dataset = None,
         data_collator=None,
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
     ):
         self.config = config
 
-        self.device, self.device_type = self._set_device_and_type()
+        self.device, self.device_type = self._prepare_device_and_type()
         self.autocast_dtype = torch.bfloat16 if self.device_type == "cpu" else torch.float16
         self.scaler = torch.cuda.amp.GradScaler(enabled=self.config.use_amp and self.device_type == "cuda")
 
-        self.set_seed(self.config.seed)
+        self._set_seed(self.config.seed)
 
-        self.model = self._init_model_weights(model).to(self.device)
+        self.model = self._prepare_model(model)
 
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
-        self.data_collator = data_collator
-        self.num_labels = self.train_dataset.num_labels  # noqa
+        self.data_collator = data_collator or self.train_dataset.data_collator
+        self.train_dataloader, self.eval_dataloader = self._prepare_dataloaders()
 
-        self.train_dataloader, self.eval_dataloader = self._setup_dataloaders()
-
-        self.optimizer, self.lr_scheduler = self._setup_optimizers(optimizer, lr_scheduler)
+        self.optimizer, self.lr_scheduler = self._prepare_optimizers(optimizer, lr_scheduler)
 
         self.metrics_manager = self._setup_metrics_manager(self.config.metrics)
 
         self.tensorboard = SummaryWriter(log_dir=self.config.log_dir)
 
+    def _prepare_device_and_type(self):
+        device = self.config.device if "cuda" in self.config.device and torch.cuda.is_available() else "cpu"
+        device_type = "cuda" if "cuda" in device else "cpu"
+        return device, device_type
+
     @staticmethod
-    def set_seed(seed):
+    def _set_seed(seed):
         torch.manual_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
 
-    def _init_model_weights(self, model):
+    def _prepare_model(self, model: Model):
+        if model is None:
+            raise ValueError("`model` must be given to the Trainer!")
         hub_path = self.config.init_weights_from
-        local_path = hf_hub_download(hub_path, filename=model.model_filename, cache_dir=HEZAR_CACHE_DIR)
-        model.load_state_dict(torch.load(local_path, map_location="cpu"))
+        if hub_path is not None:
+            local_path = hf_hub_download(hub_path, filename=model.model_filename, cache_dir=HEZAR_CACHE_DIR)
+            model.load_state_dict(torch.load(local_path, map_location="cpu"))
+        model.to(self.device)
         return model
 
-    def _set_device_and_type(self):
-        device = self.config.device if "cuda" in self.config.device and torch.cuda.is_available() else "cpu"
-        device_type = "cuda" if "cuda" in device else "cpu"
-        return device, device_type
-
-    def _setup_dataloaders(self):
+    def _prepare_dataloaders(self):
         """
         Set up data loaders (train/eval) and return them.
 
         Returns:
              A tuple of train and eval dataloaders
         """
-        train_dataloader = DataLoader(
-            dataset=self.train_dataset,
-            batch_size=self.config.batch_size,
-            collate_fn=self.data_collator,
-            shuffle=True,
-        )
-        eval_dataloader = DataLoader(
-            dataset=self.eval_dataset,
-            batch_size=self.config.batch_size,
-            collate_fn=self.data_collator,
-            shuffle=True,
-        )
+        if self.train_dataset is not None:
+            train_dataloader = DataLoader(
+                dataset=self.train_dataset,
+                batch_size=self.config.batch_size,
+                collate_fn=self.data_collator,
+                num_workers=self.config.num_dataloader_workers,
+                shuffle=True,
+            )
+        else:
+            raise ValueError("Cannot create train dataloader because `train_dataset` is not given!")
+        if self.eval_dataset is not None:
+            eval_dataloader = DataLoader(
+                dataset=self.eval_dataset,
+                batch_size=self.config.batch_size,
+                collate_fn=self.data_collator,
+                num_workers=self.config.num_dataloader_workers,
+                shuffle=True,
+            )
+        else:
+            logger.warning("Cannot create eval dataloader because `eval_dataset` is not given to the Trainer!")
+            eval_dataloader = None
+
         return train_dataloader, eval_dataloader
 
-    def _setup_optimizers(self, optimizer: torch.optim.Optimizer = None, lr_scheduler=None):
+    def _prepare_optimizers(self, optimizer: torch.optim.Optimizer = None, lr_scheduler=None):
         """
         Set up the optimizer and lr scheduler if they're not already given
 
         Args:
             optimizer: If None do nothing and return it, otherwise build it using the train config
             lr_scheduler: If None do nothing and return it, otherwise build it using the train config
 
@@ -143,45 +164,37 @@
             if isinstance(optimizer_config, OptimizerConfig):
                 optimizer_config = optimizer_config.dict()
 
             optimizer_name = optimizer_config.pop("name")
             scheduler_config = optimizer_config.pop("scheduler")
 
             optimizer_config.pop("config_type", None)
-            optimizer = build_optimizer(
-                optimizer_name,
-                self.model.parameters(),
-                **optimizer_config,
-            )
+            optimizer = optimizers[optimizer_name](self.model.parameters(), **optimizer_config)
 
             if lr_scheduler is None and scheduler_config is not None:
                 if isinstance(scheduler_config, LRSchedulerConfig):
                     scheduler_config = scheduler_config.dict()
                 scheduler_name = scheduler_config.pop("name")
                 scheduler_config.pop("config_type", None)
-                lr_scheduler = build_scheduler(
-                    scheduler_name,
-                    optimizer,
-                    **scheduler_config,
-                )
+                lr_scheduler = lr_schedulers[scheduler_name](optimizer, **scheduler_config)
         return optimizer, lr_scheduler
 
     def _setup_metrics_manager(self, metrics: Dict[str, Dict]) -> MetricsManager:
         """
         Set up metrics manager to track and update metrics like loss, accuracy, f1, etc.
 
         Args:
             metrics: A dict of metrics names and their kwargs {metric_name: **kwargs}
 
         Returns:
              A MetricsManager instance
         """
         metrics_dict = {"loss": None}
         for name, kwargs in metrics.items():
-            metrics_dict[name] = METRICS_MAP[name](num_classes=self.num_labels, **kwargs)
+            metrics_dict[name] = METRICS_MAP[name](num_classes=self.train_dataset.config.num_labels, **kwargs)
         metrics_manager = MetricsManager(metrics_dict)
         return metrics_manager
 
     def training_step(self, input_batch: Dict[str, torch.Tensor]):
         """
         Train one batch of data and return metrics outputs
```

### Comparing `hezar-0.14.0/hezar/trainers/trainer_utils.py` & `hezar-0.14.1/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/utils/config_utils.py` & `hezar-0.14.1/hezar/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/hezar/utils/hub_utils.py` & `hezar-0.14.1/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.0/pyproject.toml` & `hezar-0.14.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.14.0"
+version = "0.14.1"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.14.0/PKG-INFO` & `hezar-0.14.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.14.0
+Version: 0.14.1
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -72,23 +72,23 @@
 
 # this is our Hub repo
 model_path = "hezarai/bert-fa-sentiment-digikala-snappfood"
 # load model and tokenizer
 model = Model.load(model_path)
 tokenizer = Tokenizer.load(model_path)
 # tokenize inputs
-example = ["کتابخانه هزار، بهترین کتابخانه هوش مصنوعیه"]
+example = ["هزار، کتابخانه‌ای کامل برای به کارگیری آسان هوش مصنوعی"]
 inputs = tokenizer(example, return_tensors="pt")
 # inference
 outputs = model.predict(inputs)
 # print outputs
 print(outputs)
 ```
 ```commandline
-{'labels': ['positive'], 'probs': [0.9960528612136841]}
+{'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
 ### Build models from scratch
 Wanna use models without any pretrained weights? Easy!
 
 Build a raw BERT-based model for text classification with a single line of code!
 ```python
 from hezar import build_model
```

