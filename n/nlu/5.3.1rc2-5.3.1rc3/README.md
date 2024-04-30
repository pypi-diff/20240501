# Comparing `tmp/nlu-5.3.1rc2.tar.gz` & `tmp/nlu-5.3.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlu-5.3.1rc2.tar", last modified: Tue Mar 19 04:35:44 2024, max compression
+gzip compressed data, was "nlu-5.3.1rc3.tar", last modified: Tue Mar 19 22:21:36 2024, max compression
```

## Comparing `nlu-5.3.1rc2.tar` & `nlu-5.3.1rc3.tar`

### file list

```diff
@@ -1,620 +1,620 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.962079 nlu-5.3.1rc2/
--rw-rw-r--   0 root         (0) root         (0)    11357 2022-07-04 18:06:45.000000 nlu-5.3.1rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)   108800 2024-03-19 04:35:44.962079 nlu-5.3.1rc2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)   107703 2024-01-18 20:27:20.000000 nlu-5.3.1rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/
--rw-rw-r--   0 root         (0) root         (0)    21597 2024-03-19 04:35:37.000000 nlu-5.3.1rc2/nlu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/assertions/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/assertions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/assertions/assertion_dl/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/assertions/assertion_dl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      963 2022-03-24 18:05:28.000000 nlu-5.3.1rc2/nlu/components/assertions/assertion_dl/assertion_dl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/assertions/assertion_log_reg/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/assertions/assertion_log_reg/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      978 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/assertions/assertion_log_reg/assertion_log_reg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/chunkers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/chunkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/chunkers/chunk_mapper/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/chunkers/chunk_mapper/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      534 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/chunkers/chunk_mapper/chunk_mapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/chunkers/contextual_parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/chunkers/contextual_parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      529 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/chunkers/contextual_parser/contextual_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/chunkers/default_chunker/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/chunkers/default_chunker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      266 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/chunkers/default_chunker/default_chunker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/chunkers/ngram/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/chunkers/ngram/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      269 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/chunkers/ngram/ngram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/asr/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/asr/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      449 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/asr/wav2Vec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/asr_hubert/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/asr_hubert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      444 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/asr_hubert/hubert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/asr_whisper/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/asr_whisper/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      446 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/asr_whisper/whisper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/bart_zero_shot_classification/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 03:58:53.000000 nlu-5.3.1rc2/nlu/components/classifiers/bart_zero_shot_classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-03-05 03:58:53.000000 nlu-5.3.1rc2/nlu/components/classifiers/bart_zero_shot_classification/bart_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/bert_zero_shot_classification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/bert_zero_shot_classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      586 2023-09-10 22:53:52.000000 nlu-5.3.1rc2/nlu/components/classifiers/bert_zero_shot_classification/bert_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/classifier_dl/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/classifier_dl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1024 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/classifier_dl/classifier_dl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/deberta_zero_shot/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 13:41:34.000000 nlu-5.3.1rc2/nlu/components/classifiers/deberta_zero_shot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      625 2024-03-05 13:41:34.000000 nlu-5.3.1rc2/nlu/components/classifiers/deberta_zero_shot/deberta_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/distil_bert_zero_shot_classification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/distil_bert_zero_shot_classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      604 2023-09-10 22:53:52.000000 nlu-5.3.1rc2/nlu/components/classifiers/distil_bert_zero_shot_classification/distil_bert_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/generic_classifier/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/generic_classifier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      952 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/generic_classifier/generic_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_swin/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_swin/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      552 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_swin/swin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_vit/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_vit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      564 2023-09-10 22:53:52.000000 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_vit/convnext_image_classification.py
--rw-rw-r--   0 root         (0) root         (0)      549 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/image_classification_vit/vit_image_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu/components/classifiers/language_detector/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/language_detector/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      448 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/language_detector/language_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/multi_classifier/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/multi_classifier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      804 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/multi_classifier/multi_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/named_entity_recognizer_crf/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/named_entity_recognizer_crf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1026 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/named_entity_recognizer_crf/ner_crf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/ner/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/ner/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      928 2023-05-08 14:21:54.000000 nlu-5.3.1rc2/nlu/components/classifiers/ner/ner_dl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/ner_healthcare/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/ner_healthcare/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1097 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/ner_healthcare/ner_dl_healthcare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/ner_zero_shot/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/ner_zero_shot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      613 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/ner_zero_shot/ner_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/pos/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/pos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      709 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/pos/part_of_speech_jsl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/roberta_zero_shot_classification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-09-10 22:53:52.000000 nlu-5.3.1rc2/nlu/components/classifiers/roberta_zero_shot_classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      633 2023-09-10 22:53:52.000000 nlu-5.3.1rc2/nlu/components/classifiers/roberta_zero_shot_classification/roberta_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/sentiment_detector/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/sentiment_detector/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      482 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/sentiment_detector/sentiment_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/sentiment_dl/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/sentiment_dl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      768 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/classifiers/sentiment_dl/sentiment_dl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_albert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_albert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      541 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_albert/seq_albert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_bert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_bert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      584 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_bert/seq_bert_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_bert_medical/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_bert_medical/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      474 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_bert_medical/seq_bert_medical_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_camembert/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_camembert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      553 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_camembert/seq_camembert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_deberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_deberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      624 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_deberta/seq_deberta_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      637 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert/seq_distilbert_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert_medical/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert_medical/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      504 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert_medical/seq_distilbert_medical_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_longformer/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_longformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      557 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_longformer/seq_longformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      545 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_roberta/seq_roberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_xlm_roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_xlm_roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      557 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_xlm_roberta/seq_xlm_roberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/seq_xlnet/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_xlnet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      537 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/seq_xlnet/seq_xlnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_albert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_albert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      545 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_albert/span_albert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_bert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_bert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      537 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_bert/span_bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_camembert/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_camembert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      547 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_camembert/span_camembert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_deberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_deberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      549 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_deberta/span_deberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_distilbert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_distilbert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      561 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_distilbert/span_distilbert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_longformer/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_longformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      561 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_longformer/span_longformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_medical/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_medical/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      612 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_medical/span_medical.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      549 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_roberta/span_roberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/span_xlm_roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_xlm_roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      561 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/classifiers/span_xlm_roberta/span_xlm_roberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_albert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_albert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      511 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_albert/token_albert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_bert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_bert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      495 2023-01-23 17:32:13.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_bert/token_bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_bert_healthcare/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_bert_healthcare/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      604 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_bert_healthcare/token_bert_healthcare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_camembert/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_camembert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      515 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_camembert/token_camembert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_deberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-20 15:03:43.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_deberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      507 2022-05-20 15:03:43.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_deberta/token_deberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_distilbert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_distilbert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      519 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_distilbert/token_distilbert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_longformer/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_longformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      519 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_longformer/token_longformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.942079 nlu-5.3.1rc2/nlu/components/classifiers/token_roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      507 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_roberta/token_roberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/classifiers/token_xlm_roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_xlm_roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      519 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_xlm_roberta/token_xlmroberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/classifiers/token_xlnet/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_xlnet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      499 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/token_xlnet/token_xlnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/classifiers/vivekn_sentiment/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/vivekn_sentiment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      724 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/vivekn_sentiment/vivekn_sentiment_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/classifiers/xlm_roberta_zero_shot_classification/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:01:09.000000 nlu-5.3.1rc2/nlu/components/classifiers/xlm_roberta_zero_shot_classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      604 2024-03-05 04:01:09.000000 nlu-5.3.1rc2/nlu/components/classifiers/xlm_roberta_zero_shot_classification/xlm_roberta_zero_shot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/classifiers/yake/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/classifiers/yake/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      460 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/classifiers/yake/yake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/coref/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/coref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/coref/coref_bert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/coref/coref_bert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      487 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/coref/coref_bert/coref_bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/deidentifiers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/deidentifiers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/deidentifiers/deidentifier/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/deidentifiers/deidentifier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      914 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/deidentifiers/deidentifier/deidentifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/dependency_typeds/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/dependency_typeds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/dependency_typeds/labeled_dependency_parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/dependency_typeds/labeled_dependency_parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      872 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/dependency_typeds/labeled_dependency_parser/labeled_dependency_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/dependency_untypeds/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/dependency_untypeds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/dependency_untypeds/unlabeled_dependency_parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/dependency_untypeds/unlabeled_dependency_parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      859 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/dependency_untypeds/unlabeled_dependency_parser/unlabeled_dependency_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/albert/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/albert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      454 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/albert/spark_nlp_albert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/bert/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/bert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      451 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/embeddings/bert/spark_nlp_bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/bert_sentence_chunk/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/embeddings/bert_sentence_chunk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      630 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/embeddings/bert_sentence_chunk/bert_sentence_chunk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/camenbert/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-20 15:03:43.000000 nlu-5.3.1rc2/nlu/components/embeddings/camenbert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      476 2022-06-13 17:50:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/camenbert/camenbert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/deberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-24 18:05:28.000000 nlu-5.3.1rc2/nlu/components/embeddings/deberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      474 2022-03-24 18:05:28.000000 nlu-5.3.1rc2/nlu/components/embeddings/deberta/deberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/distil_bert/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/embeddings/distil_bert/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      485 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/distil_bert/distilbert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/doc2vec/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/doc2vec/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      616 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/doc2vec/doc2vec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/elmo/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/elmo/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      485 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/elmo/spark_nlp_elmo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/glove/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/glove/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      496 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/embeddings/glove/glove.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/instructor_sentence/
--rw-rw-r--   0 root         (0) root         (0)      592 2024-01-10 22:49:05.000000 nlu-5.3.1rc2/nlu/components/embeddings/instructor_sentence/InstructorEmbeddings.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-10 22:49:05.000000 nlu-5.3.1rc2/nlu/components/embeddings/instructor_sentence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/longformer/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/longformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      485 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/longformer/longformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/openai_embeddings/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:11:12.000000 nlu-5.3.1rc2/nlu/components/embeddings/openai_embeddings/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      437 2024-03-05 04:11:12.000000 nlu-5.3.1rc2/nlu/components/embeddings/openai_embeddings/openai_embeddings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/roberta/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/embeddings/roberta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      451 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/roberta/roberta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/sentence_bert/
--rw-rw-r--   0 root         (0) root         (0)      500 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_bert/BertSentenceEmbedding.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_bert/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/sentence_bge/
--rw-rw-r--   0 root         (0) root         (0)      479 2024-03-05 15:40:40.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_bge/BGESentenceEmbedding.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:08:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_bge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/sentence_e5/
--rw-rw-r--   0 root         (0) root         (0)      457 2024-01-10 22:49:05.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_e5/E5SentenceEmbedding.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-10 22:49:05.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_e5/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/sentence_mpnet/
--rw-rw-r--   0 root         (0) root         (0)      488 2024-03-05 03:50:14.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_mpnet/MPNetSentenceEmbedding.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-10 22:49:05.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_mpnet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/sentence_roberta/
--rw-rw-r--   0 root         (0) root         (0)      520 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_roberta/RobertaSentenceEmbedding.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_roberta/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/sentence_xlm/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_xlm/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      531 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/sentence_xlm/sentence_xlm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/use/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/use/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      494 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/use/spark_nlp_use.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/word2vec/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/word2vec/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      638 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/word2vec/word2vec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/xlm/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/embeddings/xlm/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      480 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/xlm/xlm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings/xlnet/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings/xlnet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      474 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/embeddings/xlnet/spark_nlp_xlnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings_chunks/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings_chunks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/embeddings_chunks/chunk_embedder/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/embeddings_chunks/chunk_embedder/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      288 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/embeddings_chunks/chunk_embedder/chunk_embedder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/lemmatizers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/lemmatizers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/lemmatizers/lemmatizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/lemmatizers/lemmatizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      597 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/lemmatizers/lemmatizer/spark_nlp_lemmatizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.946079 nlu-5.3.1rc2/nlu/components/matchers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/matchers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/matchers/context_parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/matchers/context_parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      785 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/matchers/context_parser/context_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/matchers/date_matcher/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/matchers/date_matcher/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      256 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/matchers/date_matcher/date_matcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/matchers/regex_matcher/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/matchers/regex_matcher/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      522 2022-07-16 00:45:53.000000 nlu-5.3.1rc2/nlu/components/matchers/regex_matcher/regex_matcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/matchers/text_matcher/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/matchers/text_matcher/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      533 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/matchers/text_matcher/text_matcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/normalizers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/normalizers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/normalizers/document_normalizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/normalizers/document_normalizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      278 2022-06-13 17:50:32.000000 nlu-5.3.1rc2/nlu/components/normalizers/document_normalizer/spark_nlp_document_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/normalizers/drug_normalizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/normalizers/drug_normalizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      246 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/normalizers/drug_normalizer/drug_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/normalizers/normalizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/normalizers/normalizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      449 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/normalizers/normalizer/spark_nlp_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/relation_extractors/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1066 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor/relation_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor_dl/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor_dl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      939 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor_dl/relation_extractor_dl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/relation_extractors/zero_shot_relation_extractor/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/zero_shot_relation_extractor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      710 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/relation_extractors/zero_shot_relation_extractor/zero_shot_relation_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/resolutions/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/resolutions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/resolutions/chunk_entity_resolver/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/resolutions/chunk_entity_resolver/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1247 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/resolutions/chunk_entity_resolver/chunk_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/resolutions/sentence_entity_resolver/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/resolutions/sentence_entity_resolver/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1154 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/resolutions/sentence_entity_resolver/sentence_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/sentence_detectors/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/sentence_detectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/sentence_detectors/deep_sentence_detector/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/sentence_detectors/deep_sentence_detector/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      700 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/sentence_detectors/deep_sentence_detector/deep_sentence_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/sentence_detectors/pragmatic_sentence_detector/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/sentence_detectors/pragmatic_sentence_detector/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      233 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/sentence_detectors/pragmatic_sentence_detector/sentence_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/bart_transformer/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-09-10 22:53:52.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/bart_transformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      299 2023-09-10 22:53:54.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/bart_transformer/bart_transformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/gpt2/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/gpt2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      442 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/gpt2/gpt2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/marian/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/marian/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      455 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/marian/marian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/med_summarizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 18:22:55.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/med_summarizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      382 2023-07-29 18:22:55.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/med_summarizer/med_summarizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/med_text_generator/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-09-10 22:53:54.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/med_text_generator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      397 2023-09-10 22:53:55.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/med_text_generator/med_text_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/openai_completion/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:11:12.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/openai_completion/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      437 2024-03-05 04:11:12.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/openai_completion/openai_completion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/t5/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/t5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      419 2023-06-14 00:49:59.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/t5/t5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/seq2seqs/tapas_qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/tapas_qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      479 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/seq2seqs/tapas_qa/tapas_qa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/spell_checkers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/spell_checkers/context_spell/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/context_spell/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      644 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/context_spell/context_spell_checker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/spell_checkers/norvig_spell/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/norvig_spell/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      705 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/norvig_spell/norvig_spell_checker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/spell_checkers/symmetric_spell/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/symmetric_spell/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      627 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/spell_checkers/symmetric_spell/symmetric_spell_checker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/stemmers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/stemmers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/stemmers/stemmer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/stemmers/stemmer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      206 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/stemmers/stemmer/spark_nlp_stemmer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/stopwordscleaners/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/stopwordscleaners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/stopwordscleaners/stopwordcleaner/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/stopwordscleaners/stopwordcleaner/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      459 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/stopwordscleaners/stopwordcleaner/nlustopwordcleaner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/tokenizers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/tokenizers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/tokenizers/default_tokenizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/tokenizers/default_tokenizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      212 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/tokenizers/default_tokenizer/default_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/tokenizers/regex_tokenizer/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/tokenizers/regex_tokenizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      210 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/tokenizers/regex_tokenizer/regex_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/tokenizers/word_segmenter/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/tokenizers/word_segmenter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      942 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/tokenizers/word_segmenter/word_segmenter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/utils/audio_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/utils/audio_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      231 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/utils/audio_assembler/audio_assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/utils/chunk_2_doc/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/chunk_2_doc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      219 2023-07-29 18:22:55.000000 nlu-5.3.1rc2/nlu/components/utils/chunk_2_doc/doc_2_chunk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.950079 nlu-5.3.1rc2/nlu/components/utils/chunk_merger/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/utils/chunk_merger/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      248 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/utils/chunk_merger/chunk_merger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/deep_sentence_detector/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/deep_sentence_detector/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      254 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/deep_sentence_detector/sentence_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/doc2chunk/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/utils/doc2chunk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      206 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/utils/doc2chunk/doc_2_chunk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/document_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/document_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      261 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/document_assembler/spark_nlp_document_assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/feature_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/feature_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      743 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/utils/feature_assembler/feature_assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/image_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/utils/image_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      222 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/utils/image_assembler/spark_nlp_image_assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/multi_document_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/utils/multi_document_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      300 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/components/utils/multi_document_assembler/spark_nlp_multi_document_assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/ner_to_chunk_converter/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/ner_to_chunk_converter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      236 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/ner_to_chunk_converter/ner_to_chunk_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/ner_to_chunk_converter_licensed/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/ner_to_chunk_converter_licensed/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      284 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/components/utils/ner_to_chunk_converter_licensed/ner_to_chunk_converter_licensed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/sdf_finisher/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/utils/sdf_finisher/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      206 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/components/utils/sdf_finisher/sdf_finisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/sentence_detector/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/sentence_detector/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      232 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/sentence_detector/sentence_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/sentence_embeddings/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/sentence_embeddings/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      308 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/components/utils/sentence_embeddings/spark_nlp_sentence_embedding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/table_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/utils/table_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      239 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/components/utils/table_assembler/spark_nlp_multi_document_assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/components/utils/token_assembler/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/components/utils/token_assembler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7815 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/discovery.py
--rw-rw-r--   0 root         (0) root         (0)     5620 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/finance.py
--rw-rw-r--   0 root         (0) root         (0)     7379 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/ocr_components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/pdf_builders/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/ocr_components/pdf_builders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/pdf_builders/text2pdf/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/ocr_components/pdf_builders/text2pdf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-24 18:05:28.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/doc_table_extractor/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/doc_table_extractor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      232 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/doc_table_extractor/doc2table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image2table/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image2table/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      317 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image2table/image2table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image2table_cell/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image2table_cell/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      311 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image2table_cell/image2table_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image_table_cell2text/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image_table_cell2text/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      313 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/image_table_cell2text/image_table_cell2text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/pdf_table_extractor/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-24 18:05:28.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/pdf_table_extractor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      232 2022-03-24 18:05:28.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/pdf_table_extractor/pdf2table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/ppt_table_extractor/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/ppt_table_extractor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      232 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/ocr_components/table_extractors/ppt_table_extractor/ppt2table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/doc2text/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 03:48:20.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/doc2text/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      216 2022-03-20 03:48:20.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/doc2text/doc2text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/img2text/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 03:48:20.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/img2text/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      282 2022-03-20 03:48:20.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/img2text/img2text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/pdf2text/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 03:48:20.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/pdf2text/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      257 2022-03-20 03:48:20.000000 nlu-5.3.1rc2/nlu/ocr_components/text_recognizers/pdf2text/pdf2text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/utils/binary2image/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/binary2image/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      229 2022-05-04 18:56:01.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/binary2image/binary2image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/utils/image2hocr/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-20 15:03:43.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/image2hocr/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      220 2022-05-20 15:03:43.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/image2hocr/image2hocr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/utils/image_split_regions/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/image_split_regions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      348 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/ocr_components/utils/image_split_regions/image_split_regions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/visual_classifiers/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/ocr_components/visual_classifiers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/ocr_components/visual_classifiers/visual_document_classifier/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 13:49:14.000000 nlu-5.3.1rc2/nlu/ocr_components/visual_classifiers/visual_document_classifier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      413 2024-03-05 13:49:14.000000 nlu-5.3.1rc2/nlu/ocr_components/visual_classifiers/visual_document_classifier/visual_document_classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/pipe/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/pipe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/pipe/col_substitution/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13549 2024-03-06 20:46:50.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/col_name_substitution_utils.py
--rw-rw-r--   0 root         (0) root         (0)    19512 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/col_substitution_HC.py
--rw-rw-r--   0 root         (0) root         (0)     2302 2024-03-05 13:49:14.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/col_substitution_OCR.py
--rw-rw-r--   0 root         (0) root         (0)    58659 2024-01-26 01:30:49.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/col_substitution_OS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.954079 nlu-5.3.1rc2/nlu/pipe/col_substitution/name_deduction/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/name_deduction/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1365 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_HC.py
--rw-rw-r--   0 root         (0) root         (0)     3270 2024-03-05 04:12:31.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_OS.py
--rw-rw-r--   0 root         (0) root         (0)     2269 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/substitution_map_HC.py
--rw-rw-r--   0 root         (0) root         (0)     1028 2024-03-06 20:40:38.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/substitution_map_OCR.py
--rw-rw-r--   0 root         (0) root         (0)     7139 2024-03-05 04:11:12.000000 nlu-5.3.1rc2/nlu/pipe/col_substitution/substitution_map_OS.py
--rw-rw-r--   0 root         (0) root         (0)    16332 2024-01-11 02:26:48.000000 nlu-5.3.1rc2/nlu/pipe/component_resolution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/extractors/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/pipe/extractors/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4092 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extraction_resolver_HC.py
--rw-rw-r--   0 root         (0) root         (0)     9570 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extraction_resolver_OS.py
--rw-rw-r--   0 root         (0) root         (0)     8685 2024-03-05 03:50:14.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_base_data_classes.py
--rw-rw-r--   0 root         (0) root         (0)     7670 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_configs_HC.py
--rw-rw-r--   0 root         (0) root         (0)     1793 2024-03-05 03:50:14.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_configs_OCR.py
--rw-rw-r--   0 root         (0) root         (0)    16014 2024-01-26 01:30:49.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_configs_OS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17860 2024-03-05 13:49:14.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/base_extractor_methods.py
--rw-rw-r--   0 root         (0) root         (0)     9574 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/helper_extractor_methods.py
--rw-rw-r--   0 root         (0) root         (0)     2023 2024-03-05 13:49:14.000000 nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/ocr_extractors.py
--rw-rw-r--   0 root         (0) root         (0)    10975 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/pipe/nlu_component.py
--rw-rw-r--   0 root         (0) root         (0)    43285 2023-06-20 10:22:32.000000 nlu-5.3.1rc2/nlu/pipe/pipe_logic.py
--rw-rw-r--   0 root         (0) root         (0)    59785 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/pipe/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/pipe/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5545 2024-03-08 03:33:58.000000 nlu-5.3.1rc2/nlu/pipe/utils/audio_data_conversion_utils.py
--rw-rw-r--   0 root         (0) root         (0)    12486 2024-01-20 19:09:31.000000 nlu-5.3.1rc2/nlu/pipe/utils/component_utils.py
--rw-rw-r--   0 root         (0) root         (0)    22703 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/pipe/utils/data_conversion_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4587 2024-03-08 03:33:58.000000 nlu-5.3.1rc2/nlu/pipe/utils/ocr_data_conversion_utils.py
--rw-rw-r--   0 root         (0) root         (0)     7784 2024-01-26 01:30:49.000000 nlu-5.3.1rc2/nlu/pipe/utils/output_level_resolution_utils.py
--rw-rw-r--   0 root         (0) root         (0)    45177 2024-03-05 03:13:40.000000 nlu-5.3.1rc2/nlu/pipe/utils/pipe_utils.py
--rw-rw-r--   0 root         (0) root         (0)    19805 2024-03-17 10:45:01.000000 nlu-5.3.1rc2/nlu/pipe/utils/predict_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/utils/resolution/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/pipe/utils/resolution/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6139 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/pipe/utils/resolution/nlu_ref_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4913 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/pipe/utils/resolution/storage_ref_resolution_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3852 2022-07-16 00:46:01.000000 nlu-5.3.1rc2/nlu/pipe/utils/resolution/storage_ref_utils.py
--rw-rw-r--   0 root         (0) root         (0)      328 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/utils/resolution/uid_to_storage_ref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/viz/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc2/nlu/pipe/viz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-06-03 18:35:35.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1151 2021-06-03 18:35:35.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/gen_streamlit_code.py
--rw-rw-r--   0 root         (0) root         (0)   447301 2021-06-03 18:35:35.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/logo.py
--rw-rw-r--   0 root         (0) root         (0)    23290 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_dashboard_OS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      509 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_utils/viz_dependency_validation_OS.py
--rw-rw-r--   0 root         (0) root         (0)     7458 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_utils_OS.py
--rw-rw-r--   0 root         (0) root         (0)    52331 2022-04-25 18:48:19.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_viz_tracker.py
--rw-rw-r--   0 root         (0) root         (0)     1272 2021-06-03 18:35:35.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/styles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4917 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/entity_manifold_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4887 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/classifier.py
--rw-rw-r--   0 root         (0) root         (0)     1890 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/dep_tree.py
--rw-rw-r--   0 root         (0) root         (0)    10443 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/entity_embedding_manifold.py
--rw-rw-r--   0 root         (0) root         (0)     3760 2022-04-25 18:48:20.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/ner.py
--rw-rw-r--   0 root         (0) root         (0)    14451 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/sentence_embedding_manifold.py
--rw-rw-r--   0 root         (0) root         (0)     4381 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/token_features.py
--rw-rw-r--   0 root         (0) root         (0)    12575 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_embedding_manifold.py
--rw-rw-r--   0 root         (0) root         (0)    13387 2022-04-25 18:48:20.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_similarity.py
--rw-rw-r--   0 root         (0) root         (0)      817 2022-02-28 15:19:47.000000 nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_dependency_validation_OS.py
--rw-rw-r--   0 root         (0) root         (0)     3788 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/pipe/viz/vis_utils.py
--rw-rw-r--   0 root         (0) root         (0)    12510 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/pipe/viz/vis_utils_HC.py
--rw-rw-r--   0 root         (0) root         (0)     5305 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/pipe/viz/vis_utils_OS.py
--rw-rw-r--   0 root         (0) root         (0)  1776142 2024-03-05 13:47:55.000000 nlu-5.3.1rc2/nlu/spellbook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.958079 nlu-5.3.1rc2/nlu/universe/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:57.000000 nlu-5.3.1rc2/nlu/universe/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19866 2024-03-05 13:41:34.000000 nlu-5.3.1rc2/nlu/universe/annotator_class_universe.py
--rw-rw-r--   0 root         (0) root         (0)     1339 2022-07-16 00:42:45.000000 nlu-5.3.1rc2/nlu/universe/atoms.py
--rw-rw-r--   0 root         (0) root         (0)   365699 2024-03-15 06:36:57.000000 nlu-5.3.1rc2/nlu/universe/component_universes.py
--rw-rw-r--   0 root         (0) root         (0)    21541 2024-03-05 13:41:57.000000 nlu-5.3.1rc2/nlu/universe/feature_node_ids.py
--rw-rw-r--   0 root         (0) root         (0)    36685 2024-03-05 13:49:14.000000 nlu-5.3.1rc2/nlu/universe/feature_node_universes.py
--rw-rw-r--   0 root         (0) root         (0)     8081 2024-03-05 03:50:14.000000 nlu-5.3.1rc2/nlu/universe/feature_resolutions.py
--rw-rw-r--   0 root         (0) root         (0)     6343 2024-01-11 21:35:47.000000 nlu-5.3.1rc2/nlu/universe/feature_universes.py
--rw-rw-r--   0 root         (0) root         (0)     3504 2023-05-09 22:51:38.000000 nlu-5.3.1rc2/nlu/universe/logic_universes.py
--rw-rw-r--   0 root         (0) root         (0)     1443 2023-06-07 06:50:17.000000 nlu-5.3.1rc2/nlu/universe/universes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.962079 nlu-5.3.1rc2/nlu/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-06-03 18:35:35.000000 nlu-5.3.1rc2/nlu/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.962079 nlu-5.3.1rc2/nlu/utils/environment/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:57.000000 nlu-5.3.1rc2/nlu/utils/environment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13341 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/utils/environment/authentication.py
--rw-rw-r--   0 root         (0) root         (0)     4837 2022-07-17 17:01:42.000000 nlu-5.3.1rc2/nlu/utils/environment/env_utils.py
--rw-rw-r--   0 root         (0) root         (0)      693 2021-06-03 18:35:35.000000 nlu-5.3.1rc2/nlu/utils/environment/env_verification.py
--rw-rw-r--   0 root         (0) root         (0)     4414 2023-03-29 16:59:00.000000 nlu-5.3.1rc2/nlu/utils/environment/offline_load_utils.py
--rw-rw-r--   0 root         (0) root         (0)      549 2022-05-20 15:03:43.000000 nlu-5.3.1rc2/nlu/utils/environment/offline_load_utils_licensed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.962079 nlu-5.3.1rc2/nlu/utils/modelhub/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:57.000000 nlu-5.3.1rc2/nlu/utils/modelhub/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3551 2022-04-25 18:48:20.000000 nlu-5.3.1rc2/nlu/utils/modelhub/modelhub_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 04:35:44.938079 nlu-5.3.1rc2/nlu.egg-info/
--rw-r--r--   0 root         (0) root         (0)   108800 2024-03-19 04:35:44.000000 nlu-5.3.1rc2/nlu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22430 2024-03-19 04:35:44.000000 nlu-5.3.1rc2/nlu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 04:35:44.000000 nlu-5.3.1rc2/nlu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-19 04:35:44.000000 nlu-5.3.1rc2/nlu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-19 04:35:44.000000 nlu-5.3.1rc2/nlu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 04:35:44.962079 nlu-5.3.1rc2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1628 2024-03-05 14:54:38.000000 nlu-5.3.1rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.105540 nlu-5.3.1rc3/
+-rw-rw-r--   0 root         (0) root         (0)    11357 2022-07-04 18:06:45.000000 nlu-5.3.1rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)   108800 2024-03-19 22:21:36.105540 nlu-5.3.1rc3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)   107703 2024-01-18 20:27:20.000000 nlu-5.3.1rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/
+-rw-rw-r--   0 root         (0) root         (0)    21597 2024-03-19 22:21:32.000000 nlu-5.3.1rc3/nlu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/assertions/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/assertions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/assertions/assertion_dl/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/assertions/assertion_dl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      963 2022-03-24 18:05:28.000000 nlu-5.3.1rc3/nlu/components/assertions/assertion_dl/assertion_dl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/assertions/assertion_log_reg/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/assertions/assertion_log_reg/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      978 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/assertions/assertion_log_reg/assertion_log_reg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/chunkers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/chunkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/chunkers/chunk_mapper/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/chunkers/chunk_mapper/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      534 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/chunkers/chunk_mapper/chunk_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/chunkers/contextual_parser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/chunkers/contextual_parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      529 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/chunkers/contextual_parser/contextual_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/chunkers/default_chunker/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/chunkers/default_chunker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      266 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/chunkers/default_chunker/default_chunker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/chunkers/ngram/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/chunkers/ngram/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      269 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/chunkers/ngram/ngram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/asr/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/asr/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      449 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/asr/wav2Vec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/asr_hubert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/asr_hubert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      444 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/asr_hubert/hubert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/asr_whisper/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/asr_whisper/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      446 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/asr_whisper/whisper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/bart_zero_shot_classification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 03:58:53.000000 nlu-5.3.1rc3/nlu/components/classifiers/bart_zero_shot_classification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-03-05 03:58:53.000000 nlu-5.3.1rc3/nlu/components/classifiers/bart_zero_shot_classification/bart_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/bert_zero_shot_classification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/bert_zero_shot_classification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2023-09-10 22:53:52.000000 nlu-5.3.1rc3/nlu/components/classifiers/bert_zero_shot_classification/bert_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/classifier_dl/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/classifier_dl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1024 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/classifier_dl/classifier_dl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/deberta_zero_shot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 13:41:34.000000 nlu-5.3.1rc3/nlu/components/classifiers/deberta_zero_shot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      625 2024-03-05 13:41:34.000000 nlu-5.3.1rc3/nlu/components/classifiers/deberta_zero_shot/deberta_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/distil_bert_zero_shot_classification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/distil_bert_zero_shot_classification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      604 2023-09-10 22:53:52.000000 nlu-5.3.1rc3/nlu/components/classifiers/distil_bert_zero_shot_classification/distil_bert_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/generic_classifier/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/generic_classifier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      952 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/generic_classifier/generic_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_swin/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_swin/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      552 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_swin/swin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_vit/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_vit/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      564 2023-09-10 22:53:52.000000 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_vit/convnext_image_classification.py
+-rw-rw-r--   0 root         (0) root         (0)      549 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/image_classification_vit/vit_image_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/language_detector/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/language_detector/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      448 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/language_detector/language_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/multi_classifier/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/multi_classifier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      804 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/multi_classifier/multi_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/named_entity_recognizer_crf/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/named_entity_recognizer_crf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1026 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/named_entity_recognizer_crf/ner_crf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/ner/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/ner/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      928 2023-05-08 14:21:54.000000 nlu-5.3.1rc3/nlu/components/classifiers/ner/ner_dl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/ner_healthcare/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/ner_healthcare/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1097 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/ner_healthcare/ner_dl_healthcare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/ner_zero_shot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/ner_zero_shot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      613 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/ner_zero_shot/ner_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu/components/classifiers/pos/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/pos/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      709 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/pos/part_of_speech_jsl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/roberta_zero_shot_classification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-09-10 22:53:52.000000 nlu-5.3.1rc3/nlu/components/classifiers/roberta_zero_shot_classification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      633 2023-09-10 22:53:52.000000 nlu-5.3.1rc3/nlu/components/classifiers/roberta_zero_shot_classification/roberta_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/sentiment_detector/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/sentiment_detector/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      482 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/sentiment_detector/sentiment_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/sentiment_dl/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/sentiment_dl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      768 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/classifiers/sentiment_dl/sentiment_dl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_albert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_albert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      541 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_albert/seq_albert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_bert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_bert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      584 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_bert/seq_bert_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_bert_medical/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_bert_medical/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      474 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_bert_medical/seq_bert_medical_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_camembert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_camembert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      553 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_camembert/seq_camembert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_deberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_deberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      624 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_deberta/seq_deberta_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      637 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert/seq_distilbert_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert_medical/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert_medical/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      504 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert_medical/seq_distilbert_medical_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_longformer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_longformer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      557 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_longformer/seq_longformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      545 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_roberta/seq_roberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_xlm_roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_xlm_roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      557 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_xlm_roberta/seq_xlm_roberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/seq_xlnet/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_xlnet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      537 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/seq_xlnet/seq_xlnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_albert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_albert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      545 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_albert/span_albert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_bert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_bert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      537 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_bert/span_bert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_camembert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_camembert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      547 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_camembert/span_camembert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_deberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_deberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      549 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_deberta/span_deberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_distilbert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_distilbert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      561 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_distilbert/span_distilbert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_longformer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_longformer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      561 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_longformer/span_longformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_medical/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_medical/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      612 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_medical/span_medical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      549 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_roberta/span_roberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/span_xlm_roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_xlm_roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      561 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/classifiers/span_xlm_roberta/span_xlm_roberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_albert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_albert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      511 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_albert/token_albert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_bert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_bert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      495 2023-01-23 17:32:13.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_bert/token_bert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_bert_healthcare/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_bert_healthcare/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      604 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_bert_healthcare/token_bert_healthcare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_camembert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_camembert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      515 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_camembert/token_camembert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_deberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-20 15:03:43.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_deberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      507 2022-05-20 15:03:43.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_deberta/token_deberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_distilbert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_distilbert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      519 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_distilbert/token_distilbert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_longformer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_longformer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      519 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_longformer/token_longformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      507 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_roberta/token_roberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_xlm_roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_xlm_roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      519 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_xlm_roberta/token_xlmroberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/token_xlnet/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_xlnet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      499 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/token_xlnet/token_xlnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/vivekn_sentiment/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/vivekn_sentiment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      724 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/vivekn_sentiment/vivekn_sentiment_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/xlm_roberta_zero_shot_classification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:01:09.000000 nlu-5.3.1rc3/nlu/components/classifiers/xlm_roberta_zero_shot_classification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      604 2024-03-05 04:01:09.000000 nlu-5.3.1rc3/nlu/components/classifiers/xlm_roberta_zero_shot_classification/xlm_roberta_zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/classifiers/yake/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/classifiers/yake/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      460 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/classifiers/yake/yake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/coref/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/coref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/coref/coref_bert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/coref/coref_bert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      487 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/coref/coref_bert/coref_bert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/deidentifiers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/deidentifiers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/deidentifiers/deidentifier/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/deidentifiers/deidentifier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      914 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/deidentifiers/deidentifier/deidentifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/dependency_typeds/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/dependency_typeds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/dependency_typeds/labeled_dependency_parser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/dependency_typeds/labeled_dependency_parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      872 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/dependency_typeds/labeled_dependency_parser/labeled_dependency_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/dependency_untypeds/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/dependency_untypeds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/dependency_untypeds/unlabeled_dependency_parser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/dependency_untypeds/unlabeled_dependency_parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      859 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/dependency_untypeds/unlabeled_dependency_parser/unlabeled_dependency_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/albert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/albert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      454 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/albert/spark_nlp_albert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/bert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/bert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      451 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/embeddings/bert/spark_nlp_bert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/bert_sentence_chunk/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/embeddings/bert_sentence_chunk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      630 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/embeddings/bert_sentence_chunk/bert_sentence_chunk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/camenbert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-20 15:03:43.000000 nlu-5.3.1rc3/nlu/components/embeddings/camenbert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      476 2022-06-13 17:50:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/camenbert/camenbert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/deberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-24 18:05:28.000000 nlu-5.3.1rc3/nlu/components/embeddings/deberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      474 2022-03-24 18:05:28.000000 nlu-5.3.1rc3/nlu/components/embeddings/deberta/deberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.089540 nlu-5.3.1rc3/nlu/components/embeddings/distil_bert/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/embeddings/distil_bert/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      485 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/distil_bert/distilbert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/doc2vec/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/doc2vec/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      616 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/doc2vec/doc2vec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/elmo/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/elmo/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      485 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/elmo/spark_nlp_elmo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/glove/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/glove/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      496 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/embeddings/glove/glove.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/instructor_sentence/
+-rw-rw-r--   0 root         (0) root         (0)      592 2024-01-10 22:49:05.000000 nlu-5.3.1rc3/nlu/components/embeddings/instructor_sentence/InstructorEmbeddings.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-10 22:49:05.000000 nlu-5.3.1rc3/nlu/components/embeddings/instructor_sentence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/longformer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/longformer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      485 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/longformer/longformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/openai_embeddings/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:11:12.000000 nlu-5.3.1rc3/nlu/components/embeddings/openai_embeddings/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-03-05 04:11:12.000000 nlu-5.3.1rc3/nlu/components/embeddings/openai_embeddings/openai_embeddings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/roberta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/embeddings/roberta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      451 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/roberta/roberta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/sentence_bert/
+-rw-rw-r--   0 root         (0) root         (0)      500 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_bert/BertSentenceEmbedding.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_bert/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/sentence_bge/
+-rw-rw-r--   0 root         (0) root         (0)      479 2024-03-05 15:40:40.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_bge/BGESentenceEmbedding.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:08:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_bge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/sentence_e5/
+-rw-rw-r--   0 root         (0) root         (0)      457 2024-01-10 22:49:05.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_e5/E5SentenceEmbedding.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-10 22:49:05.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_e5/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/sentence_mpnet/
+-rw-rw-r--   0 root         (0) root         (0)      488 2024-03-05 03:50:14.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_mpnet/MPNetSentenceEmbedding.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-10 22:49:05.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_mpnet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/sentence_roberta/
+-rw-rw-r--   0 root         (0) root         (0)      520 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_roberta/RobertaSentenceEmbedding.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_roberta/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/sentence_xlm/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_xlm/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      531 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/sentence_xlm/sentence_xlm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/use/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/use/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      494 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/use/spark_nlp_use.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/word2vec/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/word2vec/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      638 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/word2vec/word2vec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/xlm/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/embeddings/xlm/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      480 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/xlm/xlm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings/xlnet/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings/xlnet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      474 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/embeddings/xlnet/spark_nlp_xlnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings_chunks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings_chunks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/embeddings_chunks/chunk_embedder/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/embeddings_chunks/chunk_embedder/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      288 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/embeddings_chunks/chunk_embedder/chunk_embedder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/lemmatizers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/lemmatizers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/lemmatizers/lemmatizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/lemmatizers/lemmatizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      597 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/lemmatizers/lemmatizer/spark_nlp_lemmatizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/matchers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/matchers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/matchers/context_parser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/matchers/context_parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      785 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/matchers/context_parser/context_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/matchers/date_matcher/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/matchers/date_matcher/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      256 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/matchers/date_matcher/date_matcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/matchers/regex_matcher/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/matchers/regex_matcher/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      522 2022-07-16 00:45:53.000000 nlu-5.3.1rc3/nlu/components/matchers/regex_matcher/regex_matcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/matchers/text_matcher/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/matchers/text_matcher/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      533 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/matchers/text_matcher/text_matcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/normalizers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/normalizers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/normalizers/document_normalizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/normalizers/document_normalizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      278 2022-06-13 17:50:32.000000 nlu-5.3.1rc3/nlu/components/normalizers/document_normalizer/spark_nlp_document_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/normalizers/drug_normalizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/normalizers/drug_normalizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      246 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/normalizers/drug_normalizer/drug_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/normalizers/normalizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/normalizers/normalizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      449 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/normalizers/normalizer/spark_nlp_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/relation_extractors/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1066 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor/relation_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor_dl/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor_dl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      939 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor_dl/relation_extractor_dl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/relation_extractors/zero_shot_relation_extractor/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/zero_shot_relation_extractor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      710 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/relation_extractors/zero_shot_relation_extractor/zero_shot_relation_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/resolutions/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/resolutions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/resolutions/chunk_entity_resolver/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/resolutions/chunk_entity_resolver/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1247 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/resolutions/chunk_entity_resolver/chunk_resolver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/resolutions/sentence_entity_resolver/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/resolutions/sentence_entity_resolver/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1154 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/resolutions/sentence_entity_resolver/sentence_resolver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/sentence_detectors/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/sentence_detectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/sentence_detectors/deep_sentence_detector/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/sentence_detectors/deep_sentence_detector/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      700 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/sentence_detectors/deep_sentence_detector/deep_sentence_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/sentence_detectors/pragmatic_sentence_detector/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/sentence_detectors/pragmatic_sentence_detector/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      233 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/sentence_detectors/pragmatic_sentence_detector/sentence_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/bart_transformer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-09-10 22:53:52.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/bart_transformer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      299 2023-09-10 22:53:54.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/bart_transformer/bart_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/gpt2/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/gpt2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      442 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/gpt2/gpt2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/marian/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/marian/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      455 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/marian/marian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/med_summarizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 18:22:55.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/med_summarizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      382 2023-07-29 18:22:55.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/med_summarizer/med_summarizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/med_text_generator/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-09-10 22:53:54.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/med_text_generator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      397 2023-09-10 22:53:55.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/med_text_generator/med_text_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/openai_completion/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 04:11:12.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/openai_completion/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-03-05 04:11:12.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/openai_completion/openai_completion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/t5/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/t5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      419 2023-06-14 00:49:59.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/t5/t5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/seq2seqs/tapas_qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/tapas_qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      479 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/seq2seqs/tapas_qa/tapas_qa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/spell_checkers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/spell_checkers/context_spell/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/context_spell/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      644 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/context_spell/context_spell_checker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.093540 nlu-5.3.1rc3/nlu/components/spell_checkers/norvig_spell/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/norvig_spell/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      705 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/norvig_spell/norvig_spell_checker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/spell_checkers/symmetric_spell/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/symmetric_spell/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      627 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/spell_checkers/symmetric_spell/symmetric_spell_checker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/stemmers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/stemmers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/stemmers/stemmer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/stemmers/stemmer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/stemmers/stemmer/spark_nlp_stemmer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/stopwordscleaners/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/stopwordscleaners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/stopwordscleaners/stopwordcleaner/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/stopwordscleaners/stopwordcleaner/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      459 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/stopwordscleaners/stopwordcleaner/nlustopwordcleaner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/tokenizers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/tokenizers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/tokenizers/default_tokenizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/tokenizers/default_tokenizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      212 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/tokenizers/default_tokenizer/default_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/tokenizers/regex_tokenizer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/tokenizers/regex_tokenizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      210 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/tokenizers/regex_tokenizer/regex_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/tokenizers/word_segmenter/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/tokenizers/word_segmenter/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      942 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/tokenizers/word_segmenter/word_segmenter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/audio_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/utils/audio_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      231 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/utils/audio_assembler/audio_assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/chunk_2_doc/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/chunk_2_doc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      219 2023-07-29 18:22:55.000000 nlu-5.3.1rc3/nlu/components/utils/chunk_2_doc/doc_2_chunk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/chunk_merger/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/utils/chunk_merger/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      248 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/utils/chunk_merger/chunk_merger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/deep_sentence_detector/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/deep_sentence_detector/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      254 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/deep_sentence_detector/sentence_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/doc2chunk/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/utils/doc2chunk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/utils/doc2chunk/doc_2_chunk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/document_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/document_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      261 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/document_assembler/spark_nlp_document_assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/feature_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/feature_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      743 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/utils/feature_assembler/feature_assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/image_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/utils/image_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      222 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/utils/image_assembler/spark_nlp_image_assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/multi_document_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/utils/multi_document_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      300 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/components/utils/multi_document_assembler/spark_nlp_multi_document_assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/ner_to_chunk_converter/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/ner_to_chunk_converter/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      236 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/ner_to_chunk_converter/ner_to_chunk_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/ner_to_chunk_converter_licensed/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/ner_to_chunk_converter_licensed/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      284 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/components/utils/ner_to_chunk_converter_licensed/ner_to_chunk_converter_licensed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/sdf_finisher/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/utils/sdf_finisher/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/components/utils/sdf_finisher/sdf_finisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/sentence_detector/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/sentence_detector/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      232 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/sentence_detector/sentence_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/sentence_embeddings/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/sentence_embeddings/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      308 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/components/utils/sentence_embeddings/spark_nlp_sentence_embedding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/table_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/utils/table_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      239 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/components/utils/table_assembler/spark_nlp_multi_document_assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/components/utils/token_assembler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/components/utils/token_assembler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7815 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/discovery.py
+-rw-rw-r--   0 root         (0) root         (0)     5620 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/finance.py
+-rw-rw-r--   0 root         (0) root         (0)     7379 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/ocr_components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/pdf_builders/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/ocr_components/pdf_builders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/pdf_builders/text2pdf/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/ocr_components/pdf_builders/text2pdf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-24 18:05:28.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/doc_table_extractor/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/doc_table_extractor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      232 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/doc_table_extractor/doc2table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image2table/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image2table/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image2table/image2table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image2table_cell/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image2table_cell/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      311 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image2table_cell/image2table_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image_table_cell2text/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image_table_cell2text/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      313 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/image_table_cell2text/image_table_cell2text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/pdf_table_extractor/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-24 18:05:28.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/pdf_table_extractor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      232 2022-03-24 18:05:28.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/pdf_table_extractor/pdf2table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/ppt_table_extractor/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/ppt_table_extractor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      232 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/ocr_components/table_extractors/ppt_table_extractor/ppt2table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/doc2text/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 03:48:20.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/doc2text/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      216 2022-03-20 03:48:20.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/doc2text/doc2text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/img2text/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 03:48:20.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/img2text/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      282 2022-03-20 03:48:20.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/img2text/img2text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/pdf2text/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 03:48:20.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/pdf2text/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      257 2022-03-20 03:48:20.000000 nlu-5.3.1rc3/nlu/ocr_components/text_recognizers/pdf2text/pdf2text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/utils/binary2image/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/binary2image/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      229 2022-05-04 18:56:01.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/binary2image/binary2image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/utils/image2hocr/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-20 15:03:43.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/image2hocr/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      220 2022-05-20 15:03:43.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/image2hocr/image2hocr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/utils/image_split_regions/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/image_split_regions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      348 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/ocr_components/utils/image_split_regions/image_split_regions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/visual_classifiers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/ocr_components/visual_classifiers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/ocr_components/visual_classifiers/visual_document_classifier/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 13:49:14.000000 nlu-5.3.1rc3/nlu/ocr_components/visual_classifiers/visual_document_classifier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      413 2024-03-05 13:49:14.000000 nlu-5.3.1rc3/nlu/ocr_components/visual_classifiers/visual_document_classifier/visual_document_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.097540 nlu-5.3.1rc3/nlu/pipe/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/pipe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/col_substitution/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13549 2024-03-06 20:46:50.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/col_name_substitution_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    19512 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/col_substitution_HC.py
+-rw-rw-r--   0 root         (0) root         (0)     2302 2024-03-05 13:49:14.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/col_substitution_OCR.py
+-rw-rw-r--   0 root         (0) root         (0)    58659 2024-01-26 01:30:49.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/col_substitution_OS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/col_substitution/name_deduction/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/name_deduction/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1365 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_HC.py
+-rw-rw-r--   0 root         (0) root         (0)     3270 2024-03-05 04:12:31.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_OS.py
+-rw-rw-r--   0 root         (0) root         (0)     2269 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/substitution_map_HC.py
+-rw-rw-r--   0 root         (0) root         (0)     1028 2024-03-06 20:40:38.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/substitution_map_OCR.py
+-rw-rw-r--   0 root         (0) root         (0)     7139 2024-03-05 04:11:12.000000 nlu-5.3.1rc3/nlu/pipe/col_substitution/substitution_map_OS.py
+-rw-rw-r--   0 root         (0) root         (0)    16332 2024-01-11 02:26:48.000000 nlu-5.3.1rc3/nlu/pipe/component_resolution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/extractors/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/pipe/extractors/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4092 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extraction_resolver_HC.py
+-rw-rw-r--   0 root         (0) root         (0)     9570 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extraction_resolver_OS.py
+-rw-rw-r--   0 root         (0) root         (0)     8685 2024-03-05 03:50:14.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_base_data_classes.py
+-rw-rw-r--   0 root         (0) root         (0)     7670 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_configs_HC.py
+-rw-rw-r--   0 root         (0) root         (0)     1793 2024-03-05 03:50:14.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_configs_OCR.py
+-rw-rw-r--   0 root         (0) root         (0)    16014 2024-01-26 01:30:49.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_configs_OS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17860 2024-03-05 13:49:14.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/base_extractor_methods.py
+-rw-rw-r--   0 root         (0) root         (0)     9574 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/helper_extractor_methods.py
+-rw-rw-r--   0 root         (0) root         (0)     2023 2024-03-05 13:49:14.000000 nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/ocr_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)    10975 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/pipe/nlu_component.py
+-rw-rw-r--   0 root         (0) root         (0)    43285 2023-06-20 10:22:32.000000 nlu-5.3.1rc3/nlu/pipe/pipe_logic.py
+-rw-rw-r--   0 root         (0) root         (0)    59785 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/pipe/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/pipe/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5545 2024-03-08 03:33:58.000000 nlu-5.3.1rc3/nlu/pipe/utils/audio_data_conversion_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    12486 2024-01-20 19:09:31.000000 nlu-5.3.1rc3/nlu/pipe/utils/component_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    22703 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/pipe/utils/data_conversion_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4587 2024-03-08 03:33:58.000000 nlu-5.3.1rc3/nlu/pipe/utils/ocr_data_conversion_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     7784 2024-01-26 01:30:49.000000 nlu-5.3.1rc3/nlu/pipe/utils/output_level_resolution_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    45177 2024-03-05 03:13:40.000000 nlu-5.3.1rc3/nlu/pipe/utils/pipe_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    19805 2024-03-17 10:45:01.000000 nlu-5.3.1rc3/nlu/pipe/utils/predict_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/utils/resolution/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/pipe/utils/resolution/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6139 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/pipe/utils/resolution/nlu_ref_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4913 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/pipe/utils/resolution/storage_ref_resolution_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3852 2022-07-16 00:46:01.000000 nlu-5.3.1rc3/nlu/pipe/utils/resolution/storage_ref_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      328 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/utils/resolution/uid_to_storage_ref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/viz/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-11 14:21:10.000000 nlu-5.3.1rc3/nlu/pipe/viz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-06-03 18:35:35.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1151 2021-06-03 18:35:35.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/gen_streamlit_code.py
+-rw-rw-r--   0 root         (0) root         (0)   447301 2021-06-03 18:35:35.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/logo.py
+-rw-rw-r--   0 root         (0) root         (0)    23290 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_dashboard_OS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      509 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_utils/viz_dependency_validation_OS.py
+-rw-rw-r--   0 root         (0) root         (0)     7458 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_utils_OS.py
+-rw-rw-r--   0 root         (0) root         (0)    52331 2022-04-25 18:48:19.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_viz_tracker.py
+-rw-rw-r--   0 root         (0) root         (0)     1272 2021-06-03 18:35:35.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/styles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-16 02:25:56.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:56.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4917 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/entity_manifold_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4887 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/classifier.py
+-rw-rw-r--   0 root         (0) root         (0)     1890 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/dep_tree.py
+-rw-rw-r--   0 root         (0) root         (0)    10443 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/entity_embedding_manifold.py
+-rw-rw-r--   0 root         (0) root         (0)     3760 2022-04-25 18:48:20.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/ner.py
+-rw-rw-r--   0 root         (0) root         (0)    14451 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/sentence_embedding_manifold.py
+-rw-rw-r--   0 root         (0) root         (0)     4381 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/token_features.py
+-rw-rw-r--   0 root         (0) root         (0)    12575 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_embedding_manifold.py
+-rw-rw-r--   0 root         (0) root         (0)    13387 2022-04-25 18:48:20.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_similarity.py
+-rw-rw-r--   0 root         (0) root         (0)      817 2022-02-28 15:19:47.000000 nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_dependency_validation_OS.py
+-rw-rw-r--   0 root         (0) root         (0)     3788 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/pipe/viz/vis_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    12510 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/pipe/viz/vis_utils_HC.py
+-rw-rw-r--   0 root         (0) root         (0)     5305 2022-07-17 17:01:42.000000 nlu-5.3.1rc3/nlu/pipe/viz/vis_utils_OS.py
+-rw-rw-r--   0 root         (0) root         (0)  1776142 2024-03-05 13:47:55.000000 nlu-5.3.1rc3/nlu/spellbook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/universe/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:57.000000 nlu-5.3.1rc3/nlu/universe/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    19866 2024-03-05 13:41:34.000000 nlu-5.3.1rc3/nlu/universe/annotator_class_universe.py
+-rw-rw-r--   0 root         (0) root         (0)     1339 2022-07-16 00:42:45.000000 nlu-5.3.1rc3/nlu/universe/atoms.py
+-rw-rw-r--   0 root         (0) root         (0)   365699 2024-03-15 06:36:57.000000 nlu-5.3.1rc3/nlu/universe/component_universes.py
+-rw-rw-r--   0 root         (0) root         (0)    21541 2024-03-05 13:41:57.000000 nlu-5.3.1rc3/nlu/universe/feature_node_ids.py
+-rw-rw-r--   0 root         (0) root         (0)    36685 2024-03-05 13:49:14.000000 nlu-5.3.1rc3/nlu/universe/feature_node_universes.py
+-rw-rw-r--   0 root         (0) root         (0)     8081 2024-03-05 03:50:14.000000 nlu-5.3.1rc3/nlu/universe/feature_resolutions.py
+-rw-rw-r--   0 root         (0) root         (0)     6343 2024-01-11 21:35:47.000000 nlu-5.3.1rc3/nlu/universe/feature_universes.py
+-rw-rw-r--   0 root         (0) root         (0)     3504 2023-05-09 22:51:38.000000 nlu-5.3.1rc3/nlu/universe/logic_universes.py
+-rw-rw-r--   0 root         (0) root         (0)     1443 2023-06-07 06:50:17.000000 nlu-5.3.1rc3/nlu/universe/universes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-06-03 18:35:35.000000 nlu-5.3.1rc3/nlu/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.101540 nlu-5.3.1rc3/nlu/utils/environment/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:57.000000 nlu-5.3.1rc3/nlu/utils/environment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13341 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/utils/environment/authentication.py
+-rw-rw-r--   0 root         (0) root         (0)     4917 2024-03-19 20:05:42.000000 nlu-5.3.1rc3/nlu/utils/environment/env_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      693 2021-06-03 18:35:35.000000 nlu-5.3.1rc3/nlu/utils/environment/env_verification.py
+-rw-rw-r--   0 root         (0) root         (0)     4414 2023-03-29 16:59:00.000000 nlu-5.3.1rc3/nlu/utils/environment/offline_load_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      549 2022-05-20 15:03:43.000000 nlu-5.3.1rc3/nlu/utils/environment/offline_load_utils_licensed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.105540 nlu-5.3.1rc3/nlu/utils/modelhub/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-12-18 23:19:57.000000 nlu-5.3.1rc3/nlu/utils/modelhub/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3551 2022-04-25 18:48:20.000000 nlu-5.3.1rc3/nlu/utils/modelhub/modelhub_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:21:36.085540 nlu-5.3.1rc3/nlu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)   108800 2024-03-19 22:21:36.000000 nlu-5.3.1rc3/nlu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22430 2024-03-19 22:21:36.000000 nlu-5.3.1rc3/nlu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 22:21:36.000000 nlu-5.3.1rc3/nlu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-03-19 22:21:36.000000 nlu-5.3.1rc3/nlu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-03-19 22:21:36.000000 nlu-5.3.1rc3/nlu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 22:21:36.105540 nlu-5.3.1rc3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1628 2024-03-05 14:54:38.000000 nlu-5.3.1rc3/setup.py
```

### Comparing `nlu-5.3.1rc2/LICENSE` & `nlu-5.3.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/PKG-INFO` & `nlu-5.3.1rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6c 750a  : 2.1.Name: nlu.
 00000020: 5665 7273 696f 6e3a 2035 2e33 2e31 7263  Version: 5.3.1rc
-00000030: 320a 5375 6d6d 6172 793a 204a 6f68 6e20  2.Summary: John 
+00000030: 330a 5375 6d6d 6172 793a 204a 6f68 6e20  3.Summary: John 
 00000040: 536e 6f77 204c 6162 7320 4e4c 5520 7072  Snow Labs NLU pr
 00000050: 6f76 6964 6573 2073 7461 7465 206f 6620  ovides state of 
 00000060: 7468 6520 6172 7420 616c 676f 7269 7468  the art algorith
 00000070: 6d73 2066 6f72 204e 4c50 264e 4c55 2077  ms for NLP&NLU w
 00000080: 6974 6820 3230 3030 302b 206f 6620 7072  ith 20000+ of pr
 00000090: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
 000000a0: 696e 2032 3030 2b20 6c61 6e67 7561 6765  in 200+ language
```

### Comparing `nlu-5.3.1rc2/README.md` & `nlu-5.3.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/__init__.py` & `nlu-5.3.1rc3/nlu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '5.3.1rc2'
+__version__ = '5.3.1rc3'
 
 
 import nlu.utils.environment.env_utils as env_utils
 
 if not env_utils.try_import_pyspark_in_streamlit():
     raise ImportError("You ned to install Pyspark to run nlu. Run pip install pyspark==3.0.1")
 if not env_utils.try_import_spark_nlp():
```

### Comparing `nlu-5.3.1rc2/nlu/components/assertions/assertion_dl/assertion_dl.py` & `nlu-5.3.1rc3/nlu/components/assertions/assertion_dl/assertion_dl.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/assertions/assertion_log_reg/assertion_log_reg.py` & `nlu-5.3.1rc3/nlu/components/assertions/assertion_log_reg/assertion_log_reg.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/chunkers/chunk_mapper/chunk_mapper.py` & `nlu-5.3.1rc3/nlu/components/chunkers/chunk_mapper/chunk_mapper.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/chunkers/contextual_parser/contextual_parser.py` & `nlu-5.3.1rc3/nlu/components/chunkers/contextual_parser/contextual_parser.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/bart_zero_shot_classification/bart_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/bart_zero_shot_classification/bart_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/bert_zero_shot_classification/bert_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/bert_zero_shot_classification/bert_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/classifier_dl/classifier_dl.py` & `nlu-5.3.1rc3/nlu/components/classifiers/classifier_dl/classifier_dl.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/deberta_zero_shot/deberta_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/deberta_zero_shot/deberta_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/distil_bert_zero_shot_classification/distil_bert_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/distil_bert_zero_shot_classification/distil_bert_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/generic_classifier/generic_classifier.py` & `nlu-5.3.1rc3/nlu/components/classifiers/generic_classifier/generic_classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/image_classification_swin/swin.py` & `nlu-5.3.1rc3/nlu/components/classifiers/image_classification_swin/swin.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/image_classification_vit/convnext_image_classification.py` & `nlu-5.3.1rc3/nlu/components/classifiers/image_classification_vit/convnext_image_classification.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/image_classification_vit/vit_image_classifier.py` & `nlu-5.3.1rc3/nlu/components/classifiers/image_classification_vit/vit_image_classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/multi_classifier/multi_classifier.py` & `nlu-5.3.1rc3/nlu/components/classifiers/multi_classifier/multi_classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/named_entity_recognizer_crf/ner_crf.py` & `nlu-5.3.1rc3/nlu/components/classifiers/named_entity_recognizer_crf/ner_crf.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/ner/ner_dl.py` & `nlu-5.3.1rc3/nlu/components/classifiers/ner/ner_dl.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/ner_healthcare/ner_dl_healthcare.py` & `nlu-5.3.1rc3/nlu/components/classifiers/ner_healthcare/ner_dl_healthcare.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/ner_zero_shot/ner_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/ner_zero_shot/ner_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/pos/part_of_speech_jsl.py` & `nlu-5.3.1rc3/nlu/components/classifiers/pos/part_of_speech_jsl.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/roberta_zero_shot_classification/roberta_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/roberta_zero_shot_classification/roberta_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/sentiment_dl/sentiment_dl.py` & `nlu-5.3.1rc3/nlu/components/classifiers/sentiment_dl/sentiment_dl.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_albert/seq_albert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_albert/seq_albert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_bert/seq_bert_classifier.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_bert/seq_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_camembert/seq_camembert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_camembert/seq_camembert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_deberta/seq_deberta_classifier.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_deberta/seq_deberta_classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_distilbert/seq_distilbert_classifier.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_distilbert/seq_distilbert_classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_longformer/seq_longformer.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_longformer/seq_longformer.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_roberta/seq_roberta.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_roberta/seq_roberta.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_xlm_roberta/seq_xlm_roberta.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_xlm_roberta/seq_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/seq_xlnet/seq_xlnet.py` & `nlu-5.3.1rc3/nlu/components/classifiers/seq_xlnet/seq_xlnet.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_albert/span_albert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_albert/span_albert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_bert/span_bert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_bert/span_bert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_camembert/span_camembert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_camembert/span_camembert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_deberta/span_deberta.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_deberta/span_deberta.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_distilbert/span_distilbert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_distilbert/span_distilbert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_longformer/span_longformer.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_longformer/span_longformer.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_medical/span_medical.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_medical/span_medical.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_roberta/span_roberta.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_roberta/span_roberta.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/span_xlm_roberta/span_xlm_roberta.py` & `nlu-5.3.1rc3/nlu/components/classifiers/span_xlm_roberta/span_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/token_bert_healthcare/token_bert_healthcare.py` & `nlu-5.3.1rc3/nlu/components/classifiers/token_bert_healthcare/token_bert_healthcare.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/token_camembert/token_camembert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/token_camembert/token_camembert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/token_distilbert/token_distilbert.py` & `nlu-5.3.1rc3/nlu/components/classifiers/token_distilbert/token_distilbert.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/token_longformer/token_longformer.py` & `nlu-5.3.1rc3/nlu/components/classifiers/token_longformer/token_longformer.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/token_xlm_roberta/token_xlmroberta.py` & `nlu-5.3.1rc3/nlu/components/classifiers/token_xlm_roberta/token_xlmroberta.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/vivekn_sentiment/vivekn_sentiment_detector.py` & `nlu-5.3.1rc3/nlu/components/classifiers/vivekn_sentiment/vivekn_sentiment_detector.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/classifiers/xlm_roberta_zero_shot_classification/xlm_roberta_zero_shot.py` & `nlu-5.3.1rc3/nlu/components/classifiers/xlm_roberta_zero_shot_classification/xlm_roberta_zero_shot.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/deidentifiers/deidentifier/deidentifier.py` & `nlu-5.3.1rc3/nlu/components/deidentifiers/deidentifier/deidentifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/dependency_typeds/labeled_dependency_parser/labeled_dependency_parser.py` & `nlu-5.3.1rc3/nlu/components/dependency_typeds/labeled_dependency_parser/labeled_dependency_parser.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/dependency_untypeds/unlabeled_dependency_parser/unlabeled_dependency_parser.py` & `nlu-5.3.1rc3/nlu/components/dependency_untypeds/unlabeled_dependency_parser/unlabeled_dependency_parser.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/embeddings/bert_sentence_chunk/bert_sentence_chunk.py` & `nlu-5.3.1rc3/nlu/components/embeddings/bert_sentence_chunk/bert_sentence_chunk.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/embeddings/doc2vec/doc2vec.py` & `nlu-5.3.1rc3/nlu/components/embeddings/doc2vec/doc2vec.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/embeddings/instructor_sentence/InstructorEmbeddings.py` & `nlu-5.3.1rc3/nlu/components/embeddings/instructor_sentence/InstructorEmbeddings.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/embeddings/sentence_roberta/RobertaSentenceEmbedding.py` & `nlu-5.3.1rc3/nlu/components/embeddings/sentence_roberta/RobertaSentenceEmbedding.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/embeddings/sentence_xlm/sentence_xlm.py` & `nlu-5.3.1rc3/nlu/components/embeddings/sentence_xlm/sentence_xlm.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/embeddings/word2vec/word2vec.py` & `nlu-5.3.1rc3/nlu/components/embeddings/word2vec/word2vec.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/lemmatizers/lemmatizer/spark_nlp_lemmatizer.py` & `nlu-5.3.1rc3/nlu/components/lemmatizers/lemmatizer/spark_nlp_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/matchers/context_parser/context_parser.py` & `nlu-5.3.1rc3/nlu/components/matchers/context_parser/context_parser.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/matchers/regex_matcher/regex_matcher.py` & `nlu-5.3.1rc3/nlu/components/matchers/regex_matcher/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/matchers/text_matcher/text_matcher.py` & `nlu-5.3.1rc3/nlu/components/matchers/text_matcher/text_matcher.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor/relation_extractor.py` & `nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor/relation_extractor.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/relation_extractors/relation_extractor_dl/relation_extractor_dl.py` & `nlu-5.3.1rc3/nlu/components/relation_extractors/relation_extractor_dl/relation_extractor_dl.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/relation_extractors/zero_shot_relation_extractor/zero_shot_relation_extractor.py` & `nlu-5.3.1rc3/nlu/components/relation_extractors/zero_shot_relation_extractor/zero_shot_relation_extractor.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/resolutions/chunk_entity_resolver/chunk_resolver.py` & `nlu-5.3.1rc3/nlu/components/resolutions/chunk_entity_resolver/chunk_resolver.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/resolutions/sentence_entity_resolver/sentence_resolver.py` & `nlu-5.3.1rc3/nlu/components/resolutions/sentence_entity_resolver/sentence_resolver.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/sentence_detectors/deep_sentence_detector/deep_sentence_detector.py` & `nlu-5.3.1rc3/nlu/components/sentence_detectors/deep_sentence_detector/deep_sentence_detector.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/spell_checkers/context_spell/context_spell_checker.py` & `nlu-5.3.1rc3/nlu/components/spell_checkers/context_spell/context_spell_checker.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/spell_checkers/norvig_spell/norvig_spell_checker.py` & `nlu-5.3.1rc3/nlu/components/spell_checkers/norvig_spell/norvig_spell_checker.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/spell_checkers/symmetric_spell/symmetric_spell_checker.py` & `nlu-5.3.1rc3/nlu/components/spell_checkers/symmetric_spell/symmetric_spell_checker.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/tokenizers/word_segmenter/word_segmenter.py` & `nlu-5.3.1rc3/nlu/components/tokenizers/word_segmenter/word_segmenter.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/components/utils/feature_assembler/feature_assembler.py` & `nlu-5.3.1rc3/nlu/components/utils/feature_assembler/feature_assembler.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/discovery.py` & `nlu-5.3.1rc3/nlu/discovery.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/finance.py` & `nlu-5.3.1rc3/nlu/finance.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/info.py` & `nlu-5.3.1rc3/nlu/info.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/col_name_substitution_utils.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/col_name_substitution_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/col_substitution_HC.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/col_substitution_HC.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/col_substitution_OCR.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/col_substitution_OCR.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/col_substitution_OS.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/col_substitution_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_HC.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_HC.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_OS.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/name_deduction/name_deductable_annotators_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/substitution_map_HC.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/substitution_map_HC.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/substitution_map_OCR.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/substitution_map_OCR.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/col_substitution/substitution_map_OS.py` & `nlu-5.3.1rc3/nlu/pipe/col_substitution/substitution_map_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/component_resolution.py` & `nlu-5.3.1rc3/nlu/pipe/component_resolution.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extraction_resolver_HC.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extraction_resolver_HC.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extraction_resolver_OS.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extraction_resolver_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_base_data_classes.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_base_data_classes.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_configs_HC.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_configs_HC.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_configs_OCR.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_configs_OCR.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_configs_OS.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_configs_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/base_extractor_methods.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/base_extractor_methods.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/helper_extractor_methods.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/helper_extractor_methods.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/extractors/extractor_methods/ocr_extractors.py` & `nlu-5.3.1rc3/nlu/pipe/extractors/extractor_methods/ocr_extractors.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/nlu_component.py` & `nlu-5.3.1rc3/nlu/pipe/nlu_component.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/pipe_logic.py` & `nlu-5.3.1rc3/nlu/pipe/pipe_logic.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/pipeline.py` & `nlu-5.3.1rc3/nlu/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/audio_data_conversion_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/audio_data_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/component_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/component_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/data_conversion_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/data_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/ocr_data_conversion_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/ocr_data_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/output_level_resolution_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/output_level_resolution_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/pipe_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/pipe_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/predict_helper.py` & `nlu-5.3.1rc3/nlu/pipe/utils/predict_helper.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/resolution/nlu_ref_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/resolution/nlu_ref_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/resolution/storage_ref_resolution_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/resolution/storage_ref_resolution_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/utils/resolution/storage_ref_utils.py` & `nlu-5.3.1rc3/nlu/pipe/utils/resolution/storage_ref_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/gen_streamlit_code.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/gen_streamlit_code.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/logo.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/logo.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_dashboard_OS.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_dashboard_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_utils_OS.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_utils_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/streamlit_viz_tracker.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/streamlit_viz_tracker.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/styles.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/styles.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/entity_manifold_utils.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/block_utils/entity_manifold_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/classifier.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/classifier.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/dep_tree.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/dep_tree.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/entity_embedding_manifold.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/entity_embedding_manifold.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/ner.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/ner.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/sentence_embedding_manifold.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/sentence_embedding_manifold.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/token_features.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/token_features.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_embedding_manifold.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_embedding_manifold.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_similarity.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_building_blocks/word_similarity.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/streamlit_viz/viz_dependency_validation_OS.py` & `nlu-5.3.1rc3/nlu/pipe/viz/streamlit_viz/viz_dependency_validation_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/vis_utils.py` & `nlu-5.3.1rc3/nlu/pipe/viz/vis_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/vis_utils_HC.py` & `nlu-5.3.1rc3/nlu/pipe/viz/vis_utils_HC.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/pipe/viz/vis_utils_OS.py` & `nlu-5.3.1rc3/nlu/pipe/viz/vis_utils_OS.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/spellbook.py` & `nlu-5.3.1rc3/nlu/spellbook.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/annotator_class_universe.py` & `nlu-5.3.1rc3/nlu/universe/annotator_class_universe.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/atoms.py` & `nlu-5.3.1rc3/nlu/universe/atoms.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/component_universes.py` & `nlu-5.3.1rc3/nlu/universe/component_universes.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/feature_node_ids.py` & `nlu-5.3.1rc3/nlu/universe/feature_node_ids.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/feature_node_universes.py` & `nlu-5.3.1rc3/nlu/universe/feature_node_universes.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/feature_resolutions.py` & `nlu-5.3.1rc3/nlu/universe/feature_resolutions.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/feature_universes.py` & `nlu-5.3.1rc3/nlu/universe/feature_universes.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/logic_universes.py` & `nlu-5.3.1rc3/nlu/universe/logic_universes.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/universe/universes.py` & `nlu-5.3.1rc3/nlu/universe/universes.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/utils/environment/authentication.py` & `nlu-5.3.1rc3/nlu/utils/environment/authentication.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/utils/environment/env_utils.py` & `nlu-5.3.1rc3/nlu/utils/environment/env_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import os, sys
 import logging
+import os
+import sys
 
 logger = logging.getLogger('nlu')
 
 
 def get_pyspark_version():
     import pyspark
     return pyspark.version.__version__
@@ -16,14 +17,15 @@
 
 def is_env_pyspark_3_1():
     v = get_pyspark_major_and_minor()
     if v[0] == '3' and v[1] == '1':
         return True
     return False
 
+
 def is_env_pyspark_3_2():
     v = get_pyspark_major_and_minor()
     if v[0] == '3' and v[1] == '2':
         return True
     return False
 
 
@@ -43,25 +45,25 @@
 
 def is_env_pyspark_2_3():
     v = get_pyspark_major_and_minor()
     if v[0] == '2' and v[1] == '3':
         return True
     return False
 
+
 def is_env_pyspark_2_x():
     v = get_pyspark_major_and_minor()
     return int(v[0]) <= 2
 
+
 def is_env_pyspark_3_x():
     v = get_pyspark_major_and_minor()
     return int(v[0]) == 3
 
 
-
-
 def check_pyspark_install():
     try:
         from pyspark.sql import SparkSession
         try:
             import sparknlp
             v = sparknlp.start().version
             spark_major = int(v.split('.')[0])
@@ -73,25 +75,29 @@
             return False
     except:
         print(
             "No Pyspark installed!\nPlease run '!pip install pyspark==2.4.7' or install any pyspark>=2.4.0 with pyspark<3")
         return False
     return True
 
+
 def try_import_streamlit():
     try:
         import streamlit as st
     except  ImportError:
         print("You need to install Streamlit to run this functionality.")
 
 
 def is_running_in_databricks():
     """ Check if the currently running Python Process is running in Databricks or not
      If any Environment Variable name contains 'DATABRICKS' this will return True, otherwise False"""
-    for k in os.environ.keys():
+    keys = os.environ.keys()
+    if 'DB_ENDPOINT_ENV' in keys:
+        return False
+    for k in keys:
         if 'DATABRICKS' in k:
             return True
     return False
 
 
 def install_and_import_package(pkg_name, version='', import_name=''):
     """ Install Spark-NLP-Healthcare PyPI Package in current environment if it cannot be imported and license
@@ -129,15 +135,14 @@
         # import name is not always the same name as pkg_name we want to import, so it must be specified via import name
         if import_name != '':
             globals()[import_name] = importlib.import_module(import_name)
         else:
             globals()[pkg_name] = importlib.import_module(pkg_name)
 
 
-
 def try_import_pyspark_in_streamlit():
     """Try importing Pyspark or display warn message in streamlit"""
     try:
         import pyspark
         from pyspark.sql import SparkSession
     except:
         print("You need Pyspark installed to run NLU. Run <pip install pyspark==3.0.2>")
@@ -146,15 +151,16 @@
             st.error(
                 "You need Pyspark, Sklearn, Pyplot, Pandas, Numpy installed to run this app. Run <pip install pyspark==3.0.2 sklearn pyplot numpy pandas>")
         except:
             return False
         return False
     return True
 
+
 def try_import_spark_nlp():
     """Try importing Spark NLP"""
     try:
         import sparknlp
     except:
         print("You need Spark NLP to run NLU. run pip install spark-nlp")
         return False
-    return True
+    return True
```

### Comparing `nlu-5.3.1rc2/nlu/utils/environment/env_verification.py` & `nlu-5.3.1rc3/nlu/utils/environment/env_verification.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/utils/environment/offline_load_utils.py` & `nlu-5.3.1rc3/nlu/utils/environment/offline_load_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/utils/environment/offline_load_utils_licensed.py` & `nlu-5.3.1rc3/nlu/utils/environment/offline_load_utils_licensed.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu/utils/modelhub/modelhub_utils.py` & `nlu-5.3.1rc3/nlu/utils/modelhub/modelhub_utils.py`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/nlu.egg-info/PKG-INFO` & `nlu-5.3.1rc3/nlu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6c 750a  : 2.1.Name: nlu.
 00000020: 5665 7273 696f 6e3a 2035 2e33 2e31 7263  Version: 5.3.1rc
-00000030: 320a 5375 6d6d 6172 793a 204a 6f68 6e20  2.Summary: John 
+00000030: 330a 5375 6d6d 6172 793a 204a 6f68 6e20  3.Summary: John 
 00000040: 536e 6f77 204c 6162 7320 4e4c 5520 7072  Snow Labs NLU pr
 00000050: 6f76 6964 6573 2073 7461 7465 206f 6620  ovides state of 
 00000060: 7468 6520 6172 7420 616c 676f 7269 7468  the art algorith
 00000070: 6d73 2066 6f72 204e 4c50 264e 4c55 2077  ms for NLP&NLU w
 00000080: 6974 6820 3230 3030 302b 206f 6620 7072  ith 20000+ of pr
 00000090: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
 000000a0: 696e 2032 3030 2b20 6c61 6e67 7561 6765  in 200+ language
```

### Comparing `nlu-5.3.1rc2/nlu.egg-info/SOURCES.txt` & `nlu-5.3.1rc3/nlu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlu-5.3.1rc2/setup.py` & `nlu-5.3.1rc3/setup.py`

 * *Files identical despite different names*

