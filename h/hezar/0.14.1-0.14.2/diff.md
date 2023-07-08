# Comparing `tmp/hezar-0.14.1.tar.gz` & `tmp/hezar-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.14.1.tar", max compression
+gzip compressed data, was "hezar-0.14.2.tar", max compression
```

## Comparing `hezar-0.14.1.tar` & `hezar-0.14.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1065 2023-07-08 07:53:38.051829 hezar-0.14.1/LICENSE
--rw-r--r--   0        0        0     4427 2023-07-08 07:53:38.051829 hezar-0.14.1/README.md
--rw-r--r--   0        0        0      238 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/__init__.py
--rw-r--r--   0        0        0     4471 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/builders.py
--rw-r--r--   0        0        0    10536 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/configs.py
--rw-r--r--   0        0        0     1216 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4576 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3701 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      282 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     2679 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2813 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     2943 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      104 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/nfkc.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/nfkd.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/normalizers/normalizer.py
--rw-r--r--   0        0        0     2218 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      298 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4623 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5181 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    18892 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4215 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     7771 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/registry.py
--rw-r--r--   0        0        0       29 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/trainers/__init__.py
--rw-r--r--   0        0        0    14619 2023-07-08 07:53:38.051829 hezar-0.14.1/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1773 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      135 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/__init__.py
--rw-r--r--   0        0        0     3468 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/config_utils.py
--rw-r--r--   0        0        0      482 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     2773 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-08 07:53:38.055829 hezar-0.14.1/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1579 2023-07-08 07:53:38.055829 hezar-0.14.1/pyproject.toml
--rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 hezar-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 09:09:38.277521 hezar-0.14.2/LICENSE
+-rw-r--r--   0        0        0     4427 2023-07-08 09:09:38.277521 hezar-0.14.2/README.md
+-rw-r--r--   0        0        0      238 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/__init__.py
+-rw-r--r--   0        0        0     4471 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/builders.py
+-rw-r--r--   0        0        0    10536 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/configs.py
+-rw-r--r--   0        0        0     1216 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-08 09:09:38.277521 hezar-0.14.2/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4576 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3701 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      282 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0     9544 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     2679 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2813 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     2943 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/normalizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/normalizers/nfkc.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/normalizers/nfkd.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/normalizers/normalizer.py
+-rw-r--r--   0        0        0     2218 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      298 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4644 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5202 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    18892 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4236 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     7771 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/registry.py
+-rw-r--r--   0        0        0       29 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0    14619 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1773 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      135 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/utils/__init__.py
+-rw-r--r--   0        0        0     3468 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/utils/config_utils.py
+-rw-r--r--   0        0        0      482 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     2773 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-08 09:09:38.281521 hezar-0.14.2/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1579 2023-07-08 09:09:38.281521 hezar-0.14.2/pyproject.toml
+-rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 hezar-0.14.2/PKG-INFO
```

### Comparing `hezar-0.14.1/LICENSE` & `hezar-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/README.md` & `hezar-0.14.2/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/builders.py` & `hezar-0.14.2/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/configs.py` & `hezar-0.14.2/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/constants.py` & `hezar-0.14.2/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/data/data_collators.py` & `hezar-0.14.2/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/data/datasets/dataset.py` & `hezar-0.14.2/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.14.2/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.14.2/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/data/utils/data_utils.py` & `hezar-0.14.2/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/embeddings/embedding.py` & `hezar-0.14.2/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/embeddings/fasttext.py` & `hezar-0.14.2/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/embeddings/word2vec.py` & `hezar-0.14.2/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.14.2/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.14.2/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.14.2/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.14.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.14.2/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.14.2/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/model.py` & `hezar-0.14.2/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.14.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.14.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.14.2/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.14.2/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.14.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.14.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.14.2/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.14.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/preprocessors/preprocessor.py` & `hezar-0.14.2/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.14.2/hezar/preprocessors/tokenizers/bpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     pad_token_type_id: int = 0
     pad_token: str = "<pad>"
     pad_to_multiple_of: int = 0
     dropout: float = None
     continuing_subword_prefix: str = ""
     end_of_word_suffix: str = ""
     fuse_unk: bool = False
-    train_config: BPETrainConfig = BPETrainConfig()
+    train_config: BPETrainConfig = field(default_factory=BPETrainConfig)
 
 
 @register_preprocessor("bpe_tokenizer", config_class=BPEConfig)
 class BPETokenizer(Tokenizer):
     """
     A standard Byte-level BPE tokenizer using 🤗HuggingFace Tokenizers
```

### Comparing `hezar-0.14.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.14.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     pad_to_multiple_of: int = 0
     dropout: float = None
     continuing_subword_prefix: str = ""
     replacement: str = "_"
     add_prefix_space: bool = True
     end_of_word_suffix: str = ""
     fuse_unk: bool = False
-    train_config: SentencePieceBPETrainConfig = SentencePieceBPETrainConfig()
+    train_config: SentencePieceBPETrainConfig = field(default_factory=SentencePieceBPETrainConfig)
 
 
 @register_preprocessor("sentencepiece_bpe_tokenizer", config_class=SentencePieceBPEConfig)
 class SentencePieceBPETokenizer(Tokenizer):
     """
     A standard SentencePiece BPE tokenizer using 🤗HuggingFace Tokenizers
```

### Comparing `hezar-0.14.1/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.14.2/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.14.2/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     pad_to_multiple_of: int = 0
     pad_token_id: int = 0
     pad_token: str = "[PAD]"
     pad_token_type_id: int = 0
     special_tokens: List[str] = field(default_factory=lambda: ["[UNK]", "[SEP]", "[CLS]", "[PAD]", "[MASK]"])
     unk_token: str = "[UNK]"
     wordpieces_prefix: str = "##"
-    train_config: WordPieceTrainConfig = WordPieceTrainConfig()
+    train_config: WordPieceTrainConfig = field(default_factory=WordPieceTrainConfig)
 
 
 @register_preprocessor("wordpiece_tokenizer", config_class=WordPieceConfig)
 class WordPieceTokenizer(Tokenizer):
     """
     A standard WordPiece tokenizer using 🤗HuggingFace Tokenizers
```

### Comparing `hezar-0.14.1/hezar/registry.py` & `hezar-0.14.2/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/trainers/trainer.py` & `hezar-0.14.2/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/trainers/trainer_utils.py` & `hezar-0.14.2/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/utils/config_utils.py` & `hezar-0.14.2/hezar/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/hezar/utils/hub_utils.py` & `hezar-0.14.2/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.1/pyproject.toml` & `hezar-0.14.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.14.1"
+version = "0.14.2"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.14.1/PKG-INFO` & `hezar-0.14.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.14.1
+Version: 0.14.2
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

