# Comparing `tmp/spark-nlp-5.0.1.tar.gz` & `tmp/spark-nlp-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spark-nlp-5.0.1.tar", last modified: Tue Jul 18 19:38:49 2023, max compression
+gzip compressed data, was "dist/spark-nlp-5.0.2.tar", last modified: Wed Aug  2 18:17:57 2023, max compression
```

## Comparing `spark-nlp-5.0.1.tar` & `spark-nlp-5.0.2.tar`

### file list

```diff
@@ -1,254 +1,255 @@
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    53719 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/PKG-INFO
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    51979 2023-07-18 14:37:07.000000 spark-nlp-5.0.1/README.md
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/com/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/com/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/com/johnsnowlabs/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/com/johnsnowlabs/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/com/johnsnowlabs/nlp/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      294 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/com/johnsnowlabs/nlp/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       67 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/setup.cfg
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6281 2023-07-18 14:37:07.000000 spark-nlp-5.0.1/setup.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/spark_nlp.egg-info/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    53719 2023-07-18 19:38:49.000000 spark-nlp-5.0.1/spark_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     9926 2023-07-18 19:38:49.000000 spark-nlp-5.0.1/spark_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        1 2023-07-18 19:38:49.000000 spark-nlp-5.0.1/spark_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       13 2023-07-18 19:38:49.000000 spark-nlp-5.0.1/spark_nlp.egg-info/top_level.txt
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/sparknlp/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    13588 2023-07-18 14:37:07.000000 spark-nlp-5.0.1/sparknlp/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5635 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotation.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1917 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotation_audio.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2547 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotation_image.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/sparknlp/annotator/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     3325 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.490210 spark-nlp-5.0.1/sparknlp/annotator/audio/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      702 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/audio/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7859 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/audio/hubert_for_ctc.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6210 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/audio/wav2vec2_for_ctc.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3141 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/chunk2_doc.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     5174 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/chunker.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.494210 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3281 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6517 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/albert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7842 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/albert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6839 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/albert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6433 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7800 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6668 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8351 2023-07-18 11:30:02.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_zero_shot_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6510 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/camembert_for_question_answering.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7962 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/camembert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6522 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/camembert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    12672 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/classifier_dl.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6486 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/deberta_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7773 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/deberta_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6738 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/deberta_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6552 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7926 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6832 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_token_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8485 2023-05-30 15:19:20.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_zero_shot_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6553 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/longformer_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7932 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/longformer_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6848 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/longformer_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    16045 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/multi_classifier_dl.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8818 2023-05-30 15:19:20.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_bert_for_zero_shot_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6471 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7857 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7220 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    14416 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/sentiment_dl.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6317 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/tapas_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6538 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlm_roberta_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7930 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlm_roberta_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6850 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlm_roberta_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7811 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlnet_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6739 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlnet_for_token_classification.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.494210 spark-nlp-5.0.1/sparknlp/annotator/coref/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       53 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/coref/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8407 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/coref/spanbert_coref.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.494210 spark-nlp-5.0.1/sparknlp/annotator/cv/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      793 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/cv/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    11874 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/cv/convnext_for_image_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    11603 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/cv/swin_for_image_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     9159 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/cv/vit_for_image_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     3152 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/date2_chunk.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.494210 spark-nlp-5.0.1/sparknlp/annotator/dependency/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      774 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/dependency/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    11212 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/dependency/dependency_parser.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    12456 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/dependency/typed_dependency_parser.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    10973 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/document_normalizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/embeddings/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1977 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9995 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/albert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8369 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/bert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9054 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/bert_sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8817 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/camembert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6052 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/chunk_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8649 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/deberta_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9275 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/distil_bert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13019 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/doc2vec.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7684 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/e5_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9858 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/elmo_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8670 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/instructor_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8754 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/longformer_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9135 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/roberta_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8181 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/roberta_sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     5402 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8571 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/universal_sentence_encoder.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13022 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/word2vec.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    15388 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/word_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9488 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/xlm_roberta_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8602 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/xlm_roberta_sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9336 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/embeddings/xlnet_embeddings.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/er/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      692 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/er/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8785 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/er/entity_ruler.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    14471 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/graph_extraction.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/keyword_extraction/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      720 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/keyword_extraction/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13215 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/keyword_extraction/yake_keyword_extraction.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/ld_dl/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      704 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ld_dl/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8079 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ld_dl/language_detector_dl.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8970 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/lemmatizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/matcher/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      920 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/matcher/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9785 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/matcher/big_text_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    11032 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/matcher/date_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     4475 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/matcher/multi_date_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8380 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/matcher/regex_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    10636 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/matcher/text_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     5274 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/n_gram_generator.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/ner/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      948 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     2793 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/ner_approach.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5924 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/ner_converter.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    14283 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/ner_crf.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    22123 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/ner_dl.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6798 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/ner_overwriter.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7501 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ner/zero_shot_ner_model.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8780 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/normalizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.498210 spark-nlp-5.0.1/sparknlp/annotator/param/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      750 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/param/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3005 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/param/classifier_encoder.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4998 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/param/evaluation_dl_params.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/pos/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      696 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/pos/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9863 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/pos/perceptron.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/sentence/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      767 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/sentence/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    10806 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/sentence/sentence_detector.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    17866 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/sentence/sentence_detector_dl.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/sentiment/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      766 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/sentiment/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8154 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/sentiment/sentiment_detector.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9655 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/sentiment/vivekn_sentiment.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/seq2seq/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      891 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/seq2seq/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    18481 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/seq2seq/bart_transformer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    15310 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/seq2seq/gpt2_transformer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9920 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/annotator/seq2seq/marian_transformer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    15853 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/seq2seq/t5_transformer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/similarity/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/annotator/similarity/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8815 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/annotator/similarity/document_similarity_ranker.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/spell_check/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      830 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/spell_check/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    31992 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/spell_check/context_spell_checker.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13197 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/spell_check/norvig_sweeting.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    11058 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/spell_check/symmetric_delete.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     2948 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/stemmer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7015 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/stop_words_cleaner.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6373 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/tf_ner_dl_graph_builder.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/token/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      861 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/token/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     4686 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/token/chunk_tokenizer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7967 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/token/recursive_tokenizer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7639 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/token/regex_tokenizer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    19939 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/token/tokenizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.502210 spark-nlp-5.0.1/sparknlp/annotator/ws/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      693 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ws/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    16365 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/annotator/ws/word_segmenter.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/base/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1307 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3320 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/audio_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6551 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/doc2_chunk.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6697 2023-05-30 15:19:20.000000 spark-nlp-5.0.1/sparknlp/base/document_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7659 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/embeddings_finisher.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8577 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/finisher.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4834 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/graph_finisher.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      849 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/has_recursive_fit.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      841 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/has_recursive_transform.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3719 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/image_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    16541 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/light_pipeline.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7064 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/multi_document_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4279 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/recursive_pipeline.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5102 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/table_assembler.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     2674 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/token2_chunk.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5075 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/base/token_assembler.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/common/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1148 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/common/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1765 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/annotator_approach.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1880 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/annotator_model.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4332 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/annotator_properties.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1225 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/common/annotator_type.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      823 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/coverage_result.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1678 2023-05-18 08:32:25.000000 spark-nlp-5.0.1/sparknlp/common/match_strategy.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    16627 2023-07-18 11:30:02.000000 spark-nlp-5.0.1/sparknlp/common/properties.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1226 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/read_as.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1449 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/recursive_annotator_approach.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4842 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/storage.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1306 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/common/utils.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    12120 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/functions.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/internal/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    23249 2023-07-03 17:19:06.000000 spark-nlp-5.0.1/sparknlp/internal/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1187 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/internal/annotator_java_ml.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1448 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/internal/annotator_transformer.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2240 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/internal/extended_java_wrapper.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2136 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/internal/params_getters_setters.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2756 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/internal/recursive.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/logging/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      642 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/logging/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    15958 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/logging/comet.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/pretrained/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      793 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/pretrained/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5740 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/pretrained/pretrained_pipeline.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7820 2023-05-30 15:19:20.000000 spark-nlp-5.0.1/sparknlp/pretrained/resource_downloader.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1099 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/pretrained/utils.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/training/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      852 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.506210 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    10819 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/graph_builders.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1311 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/create_graph.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2593 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/dataset_encoder.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    22502 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/ner_model.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2356 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/ner_model_saver.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      870 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/sentence_grouper.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1228 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    14939 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/core_rnn_cell.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6616 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/fused_rnn_cell.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8072 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/gru_ops.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    25976 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/lstm_ops.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    11803 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/rnn.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)   166408 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/rnn_cell.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     9794 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/graph_builders.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-07-18 19:38:49.510210 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1099 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/create_graph.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2594 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/dataset_encoder.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    23189 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2356 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model_saver.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      870 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/sentence_grouper.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6961 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/conll.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4953 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/conllu.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4091 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/pos.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3331 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/pub_tator.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6798 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/spacy_to_annotation.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      244 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/training/tfgraphs.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6018 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/upload_to_hub.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1276 2023-04-12 11:27:49.000000 spark-nlp-5.0.1/sparknlp/util.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.241217 spark-nlp-5.0.2/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    53719 2023-08-02 18:17:57.241217 spark-nlp-5.0.2/PKG-INFO
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    51979 2023-08-02 14:53:36.000000 spark-nlp-5.0.2/README.md
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.209218 spark-nlp-5.0.2/com/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/com/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.209218 spark-nlp-5.0.2/com/johnsnowlabs/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/com/johnsnowlabs/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.209218 spark-nlp-5.0.2/com/johnsnowlabs/nlp/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      294 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/com/johnsnowlabs/nlp/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       67 2023-08-02 18:17:57.241217 spark-nlp-5.0.2/setup.cfg
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6281 2023-08-02 14:53:36.000000 spark-nlp-5.0.2/setup.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.209218 spark-nlp-5.0.2/spark_nlp.egg-info/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    53719 2023-08-02 18:17:57.000000 spark-nlp-5.0.2/spark_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    10003 2023-08-02 18:17:57.000000 spark-nlp-5.0.2/spark_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        1 2023-08-02 18:17:57.000000 spark-nlp-5.0.2/spark_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       13 2023-08-02 18:17:57.000000 spark-nlp-5.0.2/spark_nlp.egg-info/top_level.txt
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.213218 spark-nlp-5.0.2/sparknlp/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    13588 2023-08-02 14:53:36.000000 spark-nlp-5.0.2/sparknlp/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5635 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotation.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1917 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotation_audio.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2547 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotation_image.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.213218 spark-nlp-5.0.2/sparknlp/annotator/
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     3325 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.213218 spark-nlp-5.0.2/sparknlp/annotator/audio/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      702 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/audio/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7859 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/audio/hubert_for_ctc.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6210 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/audio/wav2vec2_for_ctc.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3141 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/chunk2_doc.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     5174 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/chunker.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.217218 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3368 2023-08-02 14:53:36.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6517 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/albert_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7842 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/albert_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6839 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/albert_for_token_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6433 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7800 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6668 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_token_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8351 2023-07-18 20:20:40.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_zero_shot_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6510 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/camembert_for_question_answering.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7962 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/camembert_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6522 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/camembert_for_token_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    12672 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/classifier_dl.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6486 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/deberta_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7773 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/deberta_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6738 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/deberta_for_token_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6552 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7926 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6832 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_token_classification.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8485 2023-05-30 15:19:20.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_zero_shot_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6553 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/longformer_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7932 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/longformer_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6848 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/longformer_for_token_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    16045 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/multi_classifier_dl.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8818 2023-05-30 15:19:20.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_bert_for_zero_shot_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6471 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7857 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7220 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_for_token_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    14416 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/sentiment_dl.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6317 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/tapas_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6538 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_question_answering.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7930 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6850 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_token_classification.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8899 2023-08-02 14:53:36.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_zero_shot_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7811 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlnet_for_sequence_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6739 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlnet_for_token_classification.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.217218 spark-nlp-5.0.2/sparknlp/annotator/coref/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       53 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/coref/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8407 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/coref/spanbert_coref.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.217218 spark-nlp-5.0.2/sparknlp/annotator/cv/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      793 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/cv/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    11874 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/cv/convnext_for_image_classification.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    11603 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/cv/swin_for_image_classification.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     9159 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/cv/vit_for_image_classification.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     3152 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/date2_chunk.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.217218 spark-nlp-5.0.2/sparknlp/annotator/dependency/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      774 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/dependency/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    11212 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/dependency/dependency_parser.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    12456 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/dependency/typed_dependency_parser.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    10973 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/document_normalizer.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.221217 spark-nlp-5.0.2/sparknlp/annotator/embeddings/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1977 2023-07-03 17:19:06.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9995 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/albert_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8369 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/bert_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9054 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/bert_sentence_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8817 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/camembert_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6052 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/chunk_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8649 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/deberta_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9275 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/distil_bert_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13019 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/doc2vec.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7684 2023-07-03 17:19:06.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/e5_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9858 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/elmo_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8670 2023-07-03 17:19:06.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/instructor_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8754 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/longformer_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9135 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/roberta_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8181 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/roberta_sentence_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     5402 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/sentence_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8571 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/universal_sentence_encoder.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13022 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/word2vec.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    15388 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/word_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9488 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/xlm_roberta_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8602 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/xlm_roberta_sentence_embeddings.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9336 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/embeddings/xlnet_embeddings.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.221217 spark-nlp-5.0.2/sparknlp/annotator/er/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      692 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/er/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8785 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/er/entity_ruler.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    14471 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/graph_extraction.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.221217 spark-nlp-5.0.2/sparknlp/annotator/keyword_extraction/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      720 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/keyword_extraction/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13215 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/keyword_extraction/yake_keyword_extraction.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.221217 spark-nlp-5.0.2/sparknlp/annotator/ld_dl/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      704 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ld_dl/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8079 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ld_dl/language_detector_dl.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8970 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/lemmatizer.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/matcher/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      920 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/matcher/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9785 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/matcher/big_text_matcher.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    11032 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/matcher/date_matcher.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     4475 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/matcher/multi_date_matcher.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8380 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/matcher/regex_matcher.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    10636 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/matcher/text_matcher.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     5274 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/n_gram_generator.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/ner/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      948 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     2793 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/ner_approach.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5924 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/ner_converter.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    14283 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/ner_crf.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    22123 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/ner_dl.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     6798 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/ner_overwriter.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7501 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ner/zero_shot_ner_model.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8780 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/normalizer.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/param/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      750 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/param/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3005 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/param/classifier_encoder.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4998 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/param/evaluation_dl_params.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/pos/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      696 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/pos/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9863 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/pos/perceptron.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/sentence/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      767 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/sentence/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    10806 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/sentence/sentence_detector.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    17866 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/sentence/sentence_detector_dl.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/sentiment/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      766 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/sentiment/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     8154 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/sentiment/sentiment_detector.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9655 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/sentiment/vivekn_sentiment.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/seq2seq/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      891 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/seq2seq/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    18481 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/seq2seq/bart_transformer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    15310 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/seq2seq/gpt2_transformer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     9920 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/annotator/seq2seq/marian_transformer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    15853 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/seq2seq/t5_transformer.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.225217 spark-nlp-5.0.2/sparknlp/annotator/similarity/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-07-03 17:19:06.000000 spark-nlp-5.0.2/sparknlp/annotator/similarity/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8815 2023-07-03 17:19:06.000000 spark-nlp-5.0.2/sparknlp/annotator/similarity/document_similarity_ranker.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.229217 spark-nlp-5.0.2/sparknlp/annotator/spell_check/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      830 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/spell_check/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    31992 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/spell_check/context_spell_checker.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    13197 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/spell_check/norvig_sweeting.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    11058 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/spell_check/symmetric_delete.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     2948 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/stemmer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7015 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/stop_words_cleaner.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6373 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/tf_ner_dl_graph_builder.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.229217 spark-nlp-5.0.2/sparknlp/annotator/token/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      861 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/token/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     4686 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/token/chunk_tokenizer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7967 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/token/recursive_tokenizer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     7639 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/token/regex_tokenizer.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    19939 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/token/tokenizer.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.229217 spark-nlp-5.0.2/sparknlp/annotator/ws/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      693 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ws/__init__.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)    16365 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/annotator/ws/word_segmenter.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.229217 spark-nlp-5.0.2/sparknlp/base/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1307 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3320 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/audio_assembler.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6551 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/doc2_chunk.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6697 2023-05-30 15:19:20.000000 spark-nlp-5.0.2/sparknlp/base/document_assembler.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7659 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/embeddings_finisher.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8577 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/finisher.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4834 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/graph_finisher.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      849 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/has_recursive_fit.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      841 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/has_recursive_transform.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3719 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/image_assembler.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    16541 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/light_pipeline.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7064 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/multi_document_assembler.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4279 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/recursive_pipeline.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5102 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/table_assembler.py
+-rwxrwxr-x   0 maziyar   (1000) maziyar   (1000)     2674 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/token2_chunk.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5075 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/base/token_assembler.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.233217 spark-nlp-5.0.2/sparknlp/common/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1148 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/common/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1765 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/annotator_approach.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1880 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/annotator_model.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4332 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/annotator_properties.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1225 2023-07-03 17:19:06.000000 spark-nlp-5.0.2/sparknlp/common/annotator_type.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      823 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/coverage_result.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1678 2023-05-18 08:32:25.000000 spark-nlp-5.0.2/sparknlp/common/match_strategy.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    16627 2023-07-18 20:20:40.000000 spark-nlp-5.0.2/sparknlp/common/properties.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1226 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/read_as.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1449 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/recursive_annotator_approach.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4842 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/storage.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1306 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/common/utils.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    12120 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/functions.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.233217 spark-nlp-5.0.2/sparknlp/internal/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    23559 2023-08-02 14:53:36.000000 spark-nlp-5.0.2/sparknlp/internal/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1187 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/internal/annotator_java_ml.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1448 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/internal/annotator_transformer.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2240 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/internal/extended_java_wrapper.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2136 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/internal/params_getters_setters.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2756 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/internal/recursive.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.233217 spark-nlp-5.0.2/sparknlp/logging/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      642 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/logging/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    15958 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/logging/comet.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.233217 spark-nlp-5.0.2/sparknlp/pretrained/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      793 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/pretrained/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     5740 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/pretrained/pretrained_pipeline.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     7820 2023-05-30 15:19:20.000000 spark-nlp-5.0.2/sparknlp/pretrained/resource_downloader.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1099 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/pretrained/utils.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.233217 spark-nlp-5.0.2/sparknlp/training/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      852 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.233217 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    10819 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/graph_builders.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.237217 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1311 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/create_graph.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2593 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/dataset_encoder.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    22502 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/ner_model.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2356 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/ner_model_saver.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      870 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/sentence_grouper.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.237217 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1228 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    14939 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/core_rnn_cell.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6616 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/fused_rnn_cell.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     8072 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/gru_ops.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    25976 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/lstm_ops.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    11803 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/rnn.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)   166408 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/rnn_cell.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.237217 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     9794 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/graph_builders.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-08-02 18:17:57.241217 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1099 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/create_graph.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2594 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/dataset_encoder.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    23189 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     2356 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model_saver.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      870 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/sentence_grouper.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6961 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/conll.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4953 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/conllu.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     4091 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/pos.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     3331 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/pub_tator.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6798 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/spacy_to_annotation.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      244 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/training/tfgraphs.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6018 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/upload_to_hub.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     1276 2023-04-12 11:27:49.000000 spark-nlp-5.0.2/sparknlp/util.py
```

### Comparing `spark-nlp-5.0.1/PKG-INFO` & `spark-nlp-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-nlp
-Version: 5.0.1
+Version: 5.0.2
 Summary: John Snow Labs Spark NLP is a natural language processing library built on top of Apache Spark ML. It provides simple, performant & accurate NLP annotations for machine learning pipelines, that scale easily in a distributed environment.
 Home-page: https://github.com/JohnSnowLabs/spark-nlp
 Author: John Snow Labs
 Keywords: NLP spark vision speech deep learning transformer tensorflow BERT GPT-2 Wav2Vec2 ViT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -195,15 +195,15 @@
 To use Spark NLP you need the following requirements:
 
 - Java 8 and 11
 - Apache Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x
 
 **GPU (optional):**
 
-Spark NLP 5.0.1 is built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum following NVIDIA® software are only required for GPU support:
+Spark NLP 5.0.2 is built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum following NVIDIA® software are only required for GPU support:
 
 - NVIDIA® GPU drivers version 450.80.02 or higher
 - CUDA® Toolkit 11.2
 - cuDNN SDK 8.1.0
 
 ## Quick Start
 
@@ -211,15 +211,15 @@
 
 ```sh
 $ java -version
 # should be Java 8 or 11 (Oracle or OpenJDK)
 $ conda create -n sparknlp python=3.7 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==5.0.1 pyspark==3.3.1
+$ pip install spark-nlp==5.0.2 pyspark==3.3.1
 ```
 
 In Python console or Jupyter `Python3` kernel:
 
 ```python
 # Import Spark NLP
 from sparknlp.base import *
@@ -256,15 +256,15 @@
 Output: ['Mona Lisa', 'Leonardo', 'Louvre', 'Paris']
 ```
 
 For more examples, you can visit our dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples) to showcase all Spark NLP use cases!
 
 ## Apache Spark Support
 
-Spark NLP *5.0.1* has been built on top of Apache Spark 3.4 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
+Spark NLP *5.0.2* has been built on top of Apache Spark 3.4 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
 
 | Spark NLP | Apache Spark 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache Spark 3.2.x | Apache Spark 3.3.x | Apache Spark 3.4.x |
 |-----------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
 | 5.0.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | YES                |
 | 4.4.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | YES                |
 | 4.3.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | NO                 |
 | 4.2.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | NO                 |
@@ -295,15 +295,15 @@
 | 3.2.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 3.1.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 3.0.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 2.7.x     | YES        | YES        | NO         | NO         | NO         | YES        | NO         |
 
 ## Databricks Support
 
-Spark NLP 5.0.1 has been tested and is compatible with the following runtimes:
+Spark NLP 5.0.2 has been tested and is compatible with the following runtimes:
 
 **CPU:**
 
 - 9.1
 - 9.1 ML
 - 10.1
 - 10.1 ML
@@ -353,15 +353,15 @@
 - 12.2 ML & GPU
 - 13.0 ML & GPU
 - 13.1 ML & GPU
 - 13.2 ML & GPU
 
 ## EMR Support
 
-Spark NLP 5.0.1 has been tested and is compatible with the following EMR releases:
+Spark NLP 5.0.2 has been tested and is compatible with the following EMR releases:
 
 - emr-6.2.0
 - emr-6.3.0
 - emr-6.3.1
 - emr-6.4.0
 - emr-6.5.0
 - emr-6.6.0
@@ -397,74 +397,74 @@
 Spark NLP supports all major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x, Apache Spark 3.3.x, and Apache Spark 3.4.x
 
 #### Apache Spark 3.x (3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x - Scala 2.12)
 
 ```sh
 # CPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 The `spark-nlp` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp).
 
 ```sh
 # GPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
 ```
 
 The `spark-nlp-gpu` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu).
 
 ```sh
 # AArch64
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
 ```
 
 The `spark-nlp-aarch64` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64).
 
 ```sh
 # M1/M2 (Apple Silicon)
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
 ```
 
 The `spark-nlp-silicon` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon).
 
 **NOTE**: In case you are using large pretrained models like UniversalSentenceEncoder, you need to have the following
 set in your SparkSession:
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.kryoserializer.buffer.max=2000M \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 ## Scala
 
 Spark NLP supports Scala 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x versions. Our packages are
 deployed to Maven central. To add any of our packages as a dependency in your application you can follow these
 coordinates:
@@ -474,79 +474,79 @@
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-gpu:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-gpu_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-aarch64:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64 -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-aarch64_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-silicon:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-silicon_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 ### SBT
 
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "5.0.2"
 ```
 
 **spark-nlp-gpu:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.2"
 ```
 
 **spark-nlp-aarch64:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.2"
 ```
 
 **spark-nlp-silicon:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.2"
 ```
 
 Maven
 Central: [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp)
 
 If you are interested, there is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-starter)
@@ -560,15 +560,15 @@
 ### Pip/Conda
 
 If you installed pyspark through pip/conda, you can install `spark-nlp` through the same channel.
 
 Pip:
 
 ```bash
-pip install spark-nlp==5.0.1
+pip install spark-nlp==5.0.2
 ```
 
 Conda:
 
 ```bash
 conda install -c johnsnowlabs spark-nlp
 ```
@@ -589,15 +589,15 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
     .getOrCreate()
 ```
 
 If using local jars, you can use `spark.jars` instead for comma-delimited jar files. For cluster setups, of course,
 you'll have to put the jars in a reachable location for all driver and executor nodes.
 
 **Quick example:**
@@ -660,26 +660,26 @@
 ## Apache Zeppelin
 
 Use either one of the following options
 
 - Add the following Maven Coordinates to the interpreter's library list
 
 ```bash
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 - Add a path to pre-built jar from [here](#compiled-jars) in the interpreter's library list making sure the jar is
   available to driver path
 
 ### Python in Zeppelin
 
 Apart from the previous step, install the python module through pip
 
 ```bash
-pip install spark-nlp==5.0.1
+pip install spark-nlp==5.0.2
 ```
 
 Or you can install `spark-nlp` from inside Zeppelin by using Conda:
 
 ```bash
 python.conda install -c johnsnowlabs spark-nlp
 ```
@@ -699,15 +699,15 @@
 The easiest way to get this done on Linux and macOS is to simply install `spark-nlp` and `pyspark` PyPI packages and
 launch the Jupyter from the same Python environment:
 
 ```sh
 $ conda create -n sparknlp python=3.8 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==5.0.1 pyspark==3.3.1 jupyter
+$ pip install spark-nlp==5.0.2 pyspark==3.3.1 jupyter
 $ jupyter notebook
 ```
 
 Then you can use `python3` kernel to run your code with creating SparkSession via `spark = sparknlp.start()`.
 
 **Optional:**
 
@@ -716,15 +716,15 @@
 
 ```bash
 export SPARK_HOME=/path/to/your/spark/folder
 export PYSPARK_PYTHON=python3
 export PYSPARK_DRIVER_PYTHON=jupyter
 export PYSPARK_DRIVER_PYTHON_OPTS=notebook
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 Alternatively, you can mix in using `--jars` option for pyspark + `pip install spark-nlp`
 
 If not using pyspark at all, you'll have to run the instructions
 pointed [here](#python-without-explicit-pyspark-installation)
 
@@ -743,15 +743,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.1
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.2
 ```
 
 [Spark NLP quick start on Google Colab](https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/examples/python/quick_start_google_colab.ipynb)
 is a live demo on Google Colab that performs named entity recognitions and sentiment analysis by using Spark NLP
 pretrained pipelines.
 
 ## Kaggle Kernel
@@ -766,15 +766,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.1
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.2
 ```
 
 [Spark NLP quick start on Kaggle Kernel](https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark NLP pretrained pipeline.
 
 ## Databricks Cluster
 
@@ -785,17 +785,17 @@
     ```bash
     spark.kryoserializer.buffer.max 2000M
     spark.serializer org.apache.spark.serializer.KryoSerializer
     ```
 
 3. In `Libraries` tab inside your cluster you need to follow these steps:
 
-   3.1. Install New -> PyPI -> `spark-nlp==5.0.1` -> Install
+   3.1. Install New -> PyPI -> `spark-nlp==5.0.2` -> Install
 
-   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1` -> Install
+   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2` -> Install
 
 4. Now you can attach your notebook to the cluster and use Spark NLP!
 
 NOTE: Databricks' runtimes support different Apache Spark major releases. Please make sure you choose the correct Spark
 NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-cheatsheet)
 
@@ -838,24 +838,24 @@
   "Classification": "spark-defaults",
     "Properties": {
       "spark.yarn.stagingDir": "hdfs:///tmp",
       "spark.yarn.preserve.staging.files": "true",
       "spark.kryoserializer.buffer.max": "2000M",
       "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
       "spark.driver.maxResultSize": "0",
-      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1"
+      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2"
     }
 }]
 ```
 
 A sample of AWS CLI to launch EMR cluster:
 
 ```.sh
 aws emr create-cluster \
---name "Spark NLP 5.0.1" \
+--name "Spark NLP 5.0.2" \
 --release-label emr-6.2.0 \
 --applications Name=Hadoop Name=Spark Name=Hive \
 --instance-type m4.4xlarge \
 --instance-count 3 \
 --use-default-roles \
 --log-uri "s3://<S3_BUCKET>/" \
 --bootstrap-actions Path=s3://<S3_BUCKET>/emr-bootstrap.sh,Name=custome \
@@ -911,15 +911,15 @@
   --worker-boot-disk-size=128GB \
   --num-workers=2 \
   --bucket=${BUCKET_NAME} \
   --optional-components=JUPYTER \
   --enable-component-gateway \
   --metadata 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-storage' \
   --initialization-actions gs://goog-dataproc-initialization-actions-${REGION}/python/pip-install.sh \
-  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 2. On an existing one, you need to install spark-nlp and spark-nlp-display packages from PyPI.
 
 3. Now, you can attach your notebook to the cluster and use the Spark NLP!
 
 ## Spark NLP Configuration
@@ -950,42 +950,42 @@
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.serializer", "org.apache.spark.serializer.KryoSerializer")
     .config("spark.kryoserializer.buffer.max", "2000m")
     .config("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
     .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
     .getOrCreate()
 ```
 
 **spark-shell:**
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 **pyspark:**
 
 ```sh
 pyspark \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 **Databricks:**
 
 On a new cluster or existing one you need to add the following to the `Advanced Options -> Spark` tab:
 
 ```bash
@@ -1249,24 +1249,24 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars", "/tmp/spark-nlp-assembly-5.0.1.jar")
+    .config("spark.jars", "/tmp/spark-nlp-assembly-5.0.2.jar")
     .getOrCreate()
 ```
 
 - You can download provided Fat JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/releases),
   please pay attention to pick the one that suits your environment depending on the device (CPU/GPU) and Apache Spark
   version (3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x)
 - If you are local, you can load the Fat JAR from your local FileSystem, however, if you are in a cluster setup you need
   to put the Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. (
-  i.e., `hdfs:///tmp/spark-nlp-assembly-5.0.1.jar`)
+  i.e., `hdfs:///tmp/spark-nlp-assembly-5.0.2.jar`)
 
 Example of using pretrained Models and Pipelines in offline:
 
 ```python
 # instead of using pretrained() for online:
 # french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr")
 # you download this model, extract it, and use .load
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spark-nlp Version: 5.0.1 Summary: John Snow Labs
+Metadata-Version: 2.1 Name: spark-nlp Version: 5.0.2 Summary: John Snow Labs
 Spark NLP is a natural language processing library built on top of Apache Spark
 ML. It provides simple, performant & accurate NLP annotations for machine
 learning pipelines, that scale easily in a distributed environment. Home-page:
 https://github.com/JohnSnowLabs/spark-nlp Author: John Snow Labs Keywords: NLP
 spark vision speech deep learning transformer tensorflow BERT GPT-2 Wav2Vec2
 ViT Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
@@ -113,23 +113,23 @@
 entity recognition (Deep learning) - Easy ONNX and TensorFlow integrations -
 GPU Support - Full integration with Spark ML functions - +12000 pre-trained
 models in +200 languages! - +5000 pre-trained pipelines in +200 languages! -
 Multi-lingual NER models: Arabic, Bengali, Chinese, Danish, Dutch, English,
 Finnish, French, German, Hebrew, Italian, Japanese, Korean, Norwegian, Persian,
 Polish, Portuguese, Russian, Spanish, Swedish, Urdu, and more. ## Requirements
 To use Spark NLP you need the following requirements: - Java 8 and 11 - Apache
-Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 5.0.1 is
+Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 5.0.2 is
 built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum
 following NVIDIAÂ® software are only required for GPU support: - NVIDIAÂ® GPU
 drivers version 450.80.02 or higher - CUDAÂ® Toolkit 11.2 - cuDNN SDK 8.1.0 ##
 Quick Start This is a quick example of how to use Spark NLP pre-trained
 pipeline in Python and PySpark: ```sh $ java -version # should be Java 8 or 11
 (Oracle or OpenJDK) $ conda create -n sparknlp python=3.7 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==5.0.1 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
+nlp==5.0.2 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
 ```python # Import Spark NLP from sparknlp.base import * from
 sparknlp.annotator import * from sparknlp.pretrained import PretrainedPipeline
 import sparknlp # Start SparkSession with Spark NLP # start() functions has 3
 parameters: gpu, apple_silicon, and memory # sparknlp.start(gpu=True) will
 start the session with GPU support # sparknlp.start(apple_silicon=True) will
 start the session with macOS M1 & M2 support # sparknlp.start(memory="16G") to
 change the default driver memory in SparkSession spark = sparknlp.start() #
@@ -139,15 +139,15 @@
 Louvre in Paris. """ # Annotate your testing dataset result = pipeline.annotate
 (text) # What's in the pipeline list(result.keys()) Output: ['entities',
 'stem', 'checked', 'lemma', 'document', 'pos', 'token', 'ner', 'embeddings',
 'sentence'] # Check the results result['entities'] Output: ['Mona Lisa',
 'Leonardo', 'Louvre', 'Paris'] ``` For more examples, you can visit our
 dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/
 examples) to showcase all Spark NLP use cases! ## Apache Spark Support Spark
-NLP *5.0.1* has been built on top of Apache Spark 3.4 while fully supports
+NLP *5.0.2* has been built on top of Apache Spark 3.4 while fully supports
 Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x | Spark NLP | Apache Spark
 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache
 Spark 3.2.x | Apache Spark 3.3.x | Apache Spark 3.4.x | |-----------|----------
 ----------|--------------------|--------------------|--------------------|-----
 ---------------|--------------------|--------------------| | 5.0.x | NO | NO |
 YES | YES | YES | YES | YES | | 4.4.x | NO | NO | YES | YES | YES | YES | YES |
 | 4.3.x | NO | NO | YES | YES | YES | YES | NO | | 4.2.x | NO | NO | YES | YES
@@ -164,24 +164,24 @@
 | NO | YES | YES | YES | YES | NO | YES | | 4.4.x | NO | YES | YES | YES | YES
 | NO | YES | | 4.3.x | YES | YES | YES | YES | YES | NO | YES | | 4.2.x | YES |
 YES | YES | YES | YES | NO | YES | | 4.1.x | YES | YES | YES | YES | NO | NO |
 YES | | 4.0.x | YES | YES | YES | YES | NO | NO | YES | | 3.4.x | YES | YES |
 YES | YES | NO | YES | YES | | 3.3.x | YES | YES | YES | NO | NO | YES | YES |
 | 3.2.x | YES | YES | YES | NO | NO | YES | YES | | 3.1.x | YES | YES | YES |
 NO | NO | YES | YES | | 3.0.x | YES | YES | YES | NO | NO | YES | YES | | 2.7.x
-| YES | YES | NO | NO | NO | YES | NO | ## Databricks Support Spark NLP 5.0.1
+| YES | YES | NO | NO | NO | YES | NO | ## Databricks Support Spark NLP 5.0.2
 has been tested and is compatible with the following runtimes: **CPU:** - 9.1 -
 9.1 ML - 10.1 - 10.1 ML - 10.2 - 10.2 ML - 10.3 - 10.3 ML - 10.4 - 10.4 ML -
 10.5 - 10.5 ML - 11.0 - 11.0 ML - 11.1 - 11.1 ML - 11.2 - 11.2 ML - 11.3 - 11.3
 ML - 12.0 - 12.0 ML - 12.1 - 12.1 ML - 12.2 - 12.2 ML - 13.0 - 13.0 ML - 13.1 -
 13.1 ML - 13.2 - 13.2 ML **GPU:** - 9.1 ML & GPU - 10.1 ML & GPU - 10.2 ML &
 GPU - 10.3 ML & GPU - 10.4 ML & GPU - 10.5 ML & GPU - 11.0 ML & GPU - 11.1 ML &
 GPU - 11.2 ML & GPU - 11.3 ML & GPU - 12.0 ML & GPU - 12.1 ML & GPU - 12.2 ML &
 GPU - 13.0 ML & GPU - 13.1 ML & GPU - 13.2 ML & GPU ## EMR Support Spark NLP
-5.0.1 has been tested and is compatible with the following EMR releases: - emr-
+5.0.2 has been tested and is compatible with the following EMR releases: - emr-
 6.2.0 - emr-6.3.0 - emr-6.3.1 - emr-6.4.0 - emr-6.5.0 - emr-6.6.0 - emr-6.7.0 -
 emr-6.8.0 - emr-6.9.0 - emr-6.10.0 - emr-6.11.0 Full list of [Amazon EMR 6.x
 releases](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-release-
 6x.html) NOTE: The EMR 6.1.0 and 6.1.1 are not supported. ## Usage ## Packages
 Cheatsheet This is a cheatsheet for corresponding Spark NLP Maven package to
 Apache Spark / PySpark major version: | Apache Spark | Spark NLP on CPU | Spark
 NLP on GPU | Spark NLP on AArch64 (linux) | Spark NLP on Apple Silicon | |-----
@@ -194,75 +194,75 @@
 these architectures are limited by the community and we had to build most of
 the dependencies by ourselves to make them compatible. We support these two
 architectures, however, they may not work in some environments. ## Spark
 Packages ### Command line (requires internet connection) Spark NLP supports all
 major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x,
 Apache Spark 3.3.x, and Apache Spark 3.4.x #### Apache Spark 3.x (3.0.x, 3.1.x,
 3.2.x, 3.3.x, and 3.4.x - Scala 2.12) ```sh # CPU spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` The `spark-nlp` has been
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` The `spark-nlp` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp). ```sh # GPU spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 ``` The `spark-nlp-gpu` has been
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 ``` The `spark-nlp-gpu` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-gpu). ```sh # AArch64 spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 ``` The `spark-nlp-aarch64`
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 ``` The `spark-nlp-aarch64`
 has been published to the [Maven Repository](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64). ```sh # M1/M2 (Apple Silicon)
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1 spark-
-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1 ``` The
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2 spark-
+submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2 ``` The
 `spark-nlp-silicon` has been published to the [Maven Repository](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon). **NOTE**:
 In case you are using large pretrained models like UniversalSentenceEncoder,
 you need to have the following set in your SparkSession: ```sh spark-shell \ --
 driver-memory 16g \ --conf spark.kryoserializer.buffer.max=2000M \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` ## Scala Spark NLP supports Scala
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` ## Scala Spark NLP supports Scala
 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
 versions. Our packages are deployed to Maven central. To add any of our
 packages as a dependency in your application you can follow these coordinates:
 ### Maven **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
-```xml   com.johnsnowlabs.nlp spark-nlp_2.12 5.0.1  ``` **spark-nlp-gpu:**
-```xml   com.johnsnowlabs.nlp spark-nlp-gpu_2.12 5.0.1  ``` **spark-nlp-
-aarch64:** ```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 5.0.1  ```
+```xml   com.johnsnowlabs.nlp spark-nlp_2.12 5.0.2  ``` **spark-nlp-gpu:**
+```xml   com.johnsnowlabs.nlp spark-nlp-gpu_2.12 5.0.2  ``` **spark-nlp-
+aarch64:** ```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 5.0.2  ```
 **spark-nlp-silicon:** ```xml   com.johnsnowlabs.nlp spark-nlp-silicon_2.12
-5.0.1  ``` ### SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x,
+5.0.2  ``` ### SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x,
 and 3.4.x: ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp libraryDependencies += "com.johnsnowlabs.nlp" %%
-"spark-nlp" % "5.0.1" ``` **spark-nlp-gpu:** ```sbtshell // https://
+"spark-nlp" % "5.0.2" ``` **spark-nlp-gpu:** ```sbtshell // https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.1" ```
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.2" ```
 **spark-nlp-aarch64:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-aarch64 libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.1" ``` **spark-nlp-
+"com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.2" ``` **spark-nlp-
 silicon:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-silicon libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.1" ``` Maven Central:
+"com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.2" ``` Maven Central:
 [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp) If you are interested, there
 is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-
 starter) ## Python Spark NLP supports Python 3.6.x and above depending on your
 major PySpark version. ### Python without explicit Pyspark installation ###
 Pip/Conda If you installed pyspark through pip/conda, you can install `spark-
-nlp` through the same channel. Pip: ```bash pip install spark-nlp==5.0.1 ```
+nlp` through the same channel. Pip: ```bash pip install spark-nlp==5.0.2 ```
 Conda: ```bash conda install -c johnsnowlabs spark-nlp ``` PyPI [spark-nlp
 package](https://pypi.org/project/spark-nlp/) / Anaconda [spark-nlp package]
 (https://anaconda.org/JohnSnowLabs/spark-nlp) Then you'll have to create a
 SparkSession either from Spark NLP: ```python import sparknlp spark =
 sparknlp.start() ``` or manually: ```python spark = SparkSession.builder
 .appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config
 ("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars.packages",
-"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1") .getOrCreate() ``` If using local
+"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2") .getOrCreate() ``` If using local
 jars, you can use `spark.jars` instead for comma-delimited jar files. For
 cluster setups, of course, you'll have to put the jars in a reachable location
 for all driver and executor nodes. **Quick example:** ```python import sparknlp
 from sparknlp.pretrained import PretrainedPipeline # create or get Spark
 Session spark = sparknlp.start() sparknlp.version() spark.version # download,
 load and annotate a text by pre-trained pipeline pipeline = PretrainedPipeline
 ('recognize_entities_dl', 'en') result = pipeline.annotate('The Mona Lisa is a
@@ -275,72 +275,72 @@
 some reason you need to use the JAR, you can either download the Fat JARs
 provided here or download it from [Maven Central](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp). To add JARs to spark programs use the `--jars`
 option: ```sh spark-shell --jars spark-nlp.jar ``` The preferred way to use the
 library when running spark programs is using the `--packages` option as
 specified in the `spark-packages` section. ## Apache Zeppelin Use either one of
 the following options - Add the following Maven Coordinates to the
-interpreter's library list ```bash com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+interpreter's library list ```bash com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ``` - Add a path to pre-built jar from [here](#compiled-jars) in the
 interpreter's library list making sure the jar is available to driver path ###
 Python in Zeppelin Apart from the previous step, install the python module
-through pip ```bash pip install spark-nlp==5.0.1 ``` Or you can install `spark-
+through pip ```bash pip install spark-nlp==5.0.2 ``` Or you can install `spark-
 nlp` from inside Zeppelin by using Conda: ```bash python.conda install -
 c johnsnowlabs spark-nlp ``` Configure Zeppelin properly, use cells with
 %spark.pyspark or any interpreter name you chose. Finally, in Zeppelin
 interpreter settings, make sure you set properly zeppelin.python to the python
 you want to use and install the pip library with (e.g. `python3`). An
 alternative option would be to set `SPARK_SUBMIT_OPTIONS` (zeppelin-env.sh) and
 make sure `--packages` is there as shown earlier since it includes both scala
 and python side installation. ## Jupyter Notebook (Python) **Recommended:** The
 easiest way to get this done on Linux and macOS is to simply install `spark-
 nlp` and `pyspark` PyPI packages and launch the Jupyter from the same Python
 environment: ```sh $ conda create -n sparknlp python=3.8 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==5.0.1 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
+nlp==5.0.2 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
 `python3` kernel to run your code with creating SparkSession via `spark =
 sparknlp.start()`. **Optional:** If you are in different operating systems and
 require to make Jupyter Notebook run by using pyspark, you can follow these
 steps: ```bash export SPARK_HOME=/path/to/your/spark/folder export
 PYSPARK_PYTHON=python3 export PYSPARK_DRIVER_PYTHON=jupyter export
 PYSPARK_DRIVER_PYTHON_OPTS=notebook pyspark --packages com.johnsnowlabs.nlp:
-spark-nlp_2.12:5.0.1 ``` Alternatively, you can mix in using `--jars` option
+spark-nlp_2.12:5.0.2 ``` Alternatively, you can mix in using `--jars` option
 for pyspark + `pip install spark-nlp` If not using pyspark at all, you'll have
 to run the instructions pointed [here](#python-without-explicit-pyspark-
 installation) ## Google Colab Notebook Google Colab is perhaps the easiest way
 to get started with spark-nlp. It requires no installation or setup other than
 having a Google account. Run the following code in Google Colab notebook and
 start using spark-nlp right away. ```sh # This is only to setup PySpark and
 Spark NLP on Colab !wget https://setup.johnsnowlabs.com/colab.sh -O - | bash
 ``` This script comes with the two options to define `pyspark` and `spark-nlp`
 versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -g will
 enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 5.0.1 ``` [Spark NLP quick start on Google Colab]
+bash /dev/stdin -p 3.2.3 -s 5.0.2 ``` [Spark NLP quick start on Google Colab]
 (https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/
 examples/python/quick_start_google_colab.ipynb) is a live demo on Google Colab
 that performs named entity recognitions and sentiment analysis by using Spark
 NLP pretrained pipelines. ## Kaggle Kernel Run the following code in Kaggle
 Kernel and start using spark-nlp right away. ```sh # Let's setup Kaggle for
 Spark NLP and PySpark !wget https://setup.johnsnowlabs.com/kaggle.sh -O - |
 bash ``` This script comes with the two options to define `pyspark` and `spark-
 nlp` versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -
 g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 5.0.1 ``` [Spark NLP quick start on Kaggle Kernel]
+bash /dev/stdin -p 3.2.3 -s 5.0.2 ``` [Spark NLP quick start on Kaggle Kernel]
 (https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark
 NLP pretrained pipeline. ## Databricks Cluster 1. Create a cluster if you don't
 have one already 2. On a new cluster or existing one you need to add the
 following to the `Advanced Options -> Spark` tab: ```bash
 spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer ``` 3. In `Libraries` tab inside
 your cluster you need to follow these steps: 3.1. Install New -> PyPI -
-> `spark-nlp==5.0.1` -> Install 3.2. Install New -> Maven -> Coordinates -
-> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1` -> Install 4. Now you can attach
+> `spark-nlp==5.0.2` -> Install 3.2. Install New -> Maven -> Coordinates -
+> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2` -> Install 4. Now you can attach
 your notebook to the cluster and use Spark NLP! NOTE: Databricks' runtimes
 support different Apache Spark major releases. Please make sure you choose the
 correct Spark NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-
 cheatsheet) ## EMR Cluster To launch EMR clusters with Apache Spark/PySpark and
 Spark NLP correctly you need to have bootstrap and software configuration. A
 sample of your bootstrap script ```.sh #!/bin/bash set -x -e echo -e 'export
@@ -351,16 +351,16 @@
 S3 (must be public access): ```.json [{ "Classification": "spark-env",
 "Configurations": [{ "Classification": "export", "Properties":
 { "PYSPARK_PYTHON": "/usr/bin/python3" } }] }, { "Classification": "spark-
 defaults", "Properties": { "spark.yarn.stagingDir": "hdfs:///tmp",
 "spark.yarn.preserve.staging.files": "true", "spark.kryoserializer.buffer.max":
 "2000M", "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
 "spark.driver.maxResultSize": "0", "spark.jars.packages":
-"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1" } }] ``` A sample of AWS CLI to
-launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 5.0.1" \
+"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2" } }] ``` A sample of AWS CLI to
+launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 5.0.2" \
 --release-label emr-6.2.0 \ --applications Name=Hadoop Name=Spark Name=Hive \ -
 -instance-type m4.4xlarge \ --instance-count 3 \ --use-default-roles \ --log-
 uri "s3:///" \ --bootstrap-actions Path=s3:///emr-bootstrap.sh,Name=custome \ -
 -configurations "https:///sparknlp-config.json" \ --ec2-attributes
 KeyName=,EmrManagedMasterSecurityGroup=,EmrManagedSlaveSecurityGroup= \ --
 profile  ``` ## GCP Dataproc 1. Create a cluster if you don't have one already
 as follows. At gcloud shell: ```bash gcloud services enable
@@ -379,15 +379,15 @@
 boot-disk-size=128GB \ --num-workers=2 \ --bucket=${BUCKET_NAME} \ --optional-
 components=JUPYTER \ --enable-component-gateway \ --metadata
 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-
 storage' \ --initialization-actions gs://goog-dataproc-initialization-actions-$
 {REGION}/python/pip-install.sh \ --properties spark:
 spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:
 spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:
-spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` 2. On an
+spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` 2. On an
 existing one, you need to install spark-nlp and spark-nlp-display packages from
 PyPI. 3. Now, you can attach your notebook to the cluster and use the Spark
 NLP! ## Spark NLP Configuration You can change the following Spark NLP
 configurations via Spark Configuration: | Property Name | Default | Meaning |
 |--------------------------------------------------------|---------------------
 -|-----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -423,28 +423,28 @@
 configurations. ```python from pyspark.sql import SparkSession spark =
 SparkSession.builder .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config("spark.serializer",
 "org.apache.spark.serializer.KryoSerializer") .config
 ("spark.kryoserializer.buffer.max", "2000m") .config
 ("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
 .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
 .getOrCreate() ``` **spark-shell:** ```sh spark-shell \ --driver-memory 16g \ -
 -conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` **pyspark:** ```sh pyspark \ --
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` **pyspark:** ```sh pyspark \ --
 driver-memory 16g \ --conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` **Databricks:** On a new cluster
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` **Databricks:** On a new cluster
 or existing one you need to add the following to the `Advanced Options -
 > Spark` tab: ```bash spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer
 spark.jsl.settings.pretrained.cache_folder dbfs:/PATH_TO_CACHE
 spark.jsl.settings.storage.cluster_tmp_dir dbfs:/PATH_TO_STORAGE
 spark.jsl.settings.annotator.log_folder dbfs:/PATH_TO_LOGS ``` NOTE: If this is
 an existing cluster, after adding new configs or changing existing properties
@@ -578,22 +578,22 @@
 pipelines or the `.pretrained()` function to download pretrained models, you
 will need to manually download your pipeline/model from [Models Hub](https://
 sparknlp.org/models), extract it, and load it. Example of `SparkSession` with
 Fat JAR to have Spark NLP offline: ```python spark = SparkSession.builder
 .appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config
 ("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars", "/tmp/spark-
-nlp-assembly-5.0.1.jar") .getOrCreate() ``` - You can download provided Fat
+nlp-assembly-5.0.2.jar") .getOrCreate() ``` - You can download provided Fat
 JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/
 releases), please pay attention to pick the one that suits your environment
 depending on the device (CPU/GPU) and Apache Spark version (3.0.x, 3.1.x,
 3.2.x, 3.3.x, and 3.4.x) - If you are local, you can load the Fat JAR from your
 local FileSystem, however, if you are in a cluster setup you need to put the
 Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. ( i.e., `hdfs:
-///tmp/spark-nlp-assembly-5.0.1.jar`) Example of using pretrained Models and
+///tmp/spark-nlp-assembly-5.0.2.jar`) Example of using pretrained Models and
 Pipelines in offline: ```python # instead of using pretrained() for online: #
 french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr") # you download
 this model, extract it, and use .load french_pos = PerceptronModel.load("/tmp/
 pos_ud_gsd_fr_2.0.2_2.4_1556531457346/") .setInputCols("document", "token")
 .setOutputCol("pos") # example for pipelines # instead of using
 PretrainedPipeline # pipeline = PretrainedPipeline('explain_document_dl',
 lang='en') # you download this pipeline, extract it, and use PipelineModel
```

### Comparing `spark-nlp-5.0.1/README.md` & `spark-nlp-5.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 To use Spark NLP you need the following requirements:
 
 - Java 8 and 11
 - Apache Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x
 
 **GPU (optional):**
 
-Spark NLP 5.0.1 is built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum following NVIDIA® software are only required for GPU support:
+Spark NLP 5.0.2 is built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum following NVIDIA® software are only required for GPU support:
 
 - NVIDIA® GPU drivers version 450.80.02 or higher
 - CUDA® Toolkit 11.2
 - cuDNN SDK 8.1.0
 
 ## Quick Start
 
@@ -179,15 +179,15 @@
 
 ```sh
 $ java -version
 # should be Java 8 or 11 (Oracle or OpenJDK)
 $ conda create -n sparknlp python=3.7 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==5.0.1 pyspark==3.3.1
+$ pip install spark-nlp==5.0.2 pyspark==3.3.1
 ```
 
 In Python console or Jupyter `Python3` kernel:
 
 ```python
 # Import Spark NLP
 from sparknlp.base import *
@@ -224,15 +224,15 @@
 Output: ['Mona Lisa', 'Leonardo', 'Louvre', 'Paris']
 ```
 
 For more examples, you can visit our dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples) to showcase all Spark NLP use cases!
 
 ## Apache Spark Support
 
-Spark NLP *5.0.1* has been built on top of Apache Spark 3.4 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
+Spark NLP *5.0.2* has been built on top of Apache Spark 3.4 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
 
 | Spark NLP | Apache Spark 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache Spark 3.2.x | Apache Spark 3.3.x | Apache Spark 3.4.x |
 |-----------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
 | 5.0.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | YES                |
 | 4.4.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | YES                |
 | 4.3.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | NO                 |
 | 4.2.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | NO                 |
@@ -263,15 +263,15 @@
 | 3.2.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 3.1.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 3.0.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 2.7.x     | YES        | YES        | NO         | NO         | NO         | YES        | NO         |
 
 ## Databricks Support
 
-Spark NLP 5.0.1 has been tested and is compatible with the following runtimes:
+Spark NLP 5.0.2 has been tested and is compatible with the following runtimes:
 
 **CPU:**
 
 - 9.1
 - 9.1 ML
 - 10.1
 - 10.1 ML
@@ -321,15 +321,15 @@
 - 12.2 ML & GPU
 - 13.0 ML & GPU
 - 13.1 ML & GPU
 - 13.2 ML & GPU
 
 ## EMR Support
 
-Spark NLP 5.0.1 has been tested and is compatible with the following EMR releases:
+Spark NLP 5.0.2 has been tested and is compatible with the following EMR releases:
 
 - emr-6.2.0
 - emr-6.3.0
 - emr-6.3.1
 - emr-6.4.0
 - emr-6.5.0
 - emr-6.6.0
@@ -365,74 +365,74 @@
 Spark NLP supports all major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x, Apache Spark 3.3.x, and Apache Spark 3.4.x
 
 #### Apache Spark 3.x (3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x - Scala 2.12)
 
 ```sh
 # CPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 The `spark-nlp` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp).
 
 ```sh
 # GPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
 ```
 
 The `spark-nlp-gpu` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu).
 
 ```sh
 # AArch64
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
 ```
 
 The `spark-nlp-aarch64` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64).
 
 ```sh
 # M1/M2 (Apple Silicon)
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
 ```
 
 The `spark-nlp-silicon` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon).
 
 **NOTE**: In case you are using large pretrained models like UniversalSentenceEncoder, you need to have the following
 set in your SparkSession:
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.kryoserializer.buffer.max=2000M \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 ## Scala
 
 Spark NLP supports Scala 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x versions. Our packages are
 deployed to Maven central. To add any of our packages as a dependency in your application you can follow these
 coordinates:
@@ -442,79 +442,79 @@
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-gpu:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-gpu_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-aarch64:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64 -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-aarch64_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-silicon:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-silicon_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 ### SBT
 
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "5.0.2"
 ```
 
 **spark-nlp-gpu:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.2"
 ```
 
 **spark-nlp-aarch64:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.2"
 ```
 
 **spark-nlp-silicon:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.2"
 ```
 
 Maven
 Central: [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp)
 
 If you are interested, there is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-starter)
@@ -528,15 +528,15 @@
 ### Pip/Conda
 
 If you installed pyspark through pip/conda, you can install `spark-nlp` through the same channel.
 
 Pip:
 
 ```bash
-pip install spark-nlp==5.0.1
+pip install spark-nlp==5.0.2
 ```
 
 Conda:
 
 ```bash
 conda install -c johnsnowlabs spark-nlp
 ```
@@ -557,15 +557,15 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
     .getOrCreate()
 ```
 
 If using local jars, you can use `spark.jars` instead for comma-delimited jar files. For cluster setups, of course,
 you'll have to put the jars in a reachable location for all driver and executor nodes.
 
 **Quick example:**
@@ -628,26 +628,26 @@
 ## Apache Zeppelin
 
 Use either one of the following options
 
 - Add the following Maven Coordinates to the interpreter's library list
 
 ```bash
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 - Add a path to pre-built jar from [here](#compiled-jars) in the interpreter's library list making sure the jar is
   available to driver path
 
 ### Python in Zeppelin
 
 Apart from the previous step, install the python module through pip
 
 ```bash
-pip install spark-nlp==5.0.1
+pip install spark-nlp==5.0.2
 ```
 
 Or you can install `spark-nlp` from inside Zeppelin by using Conda:
 
 ```bash
 python.conda install -c johnsnowlabs spark-nlp
 ```
@@ -667,15 +667,15 @@
 The easiest way to get this done on Linux and macOS is to simply install `spark-nlp` and `pyspark` PyPI packages and
 launch the Jupyter from the same Python environment:
 
 ```sh
 $ conda create -n sparknlp python=3.8 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==5.0.1 pyspark==3.3.1 jupyter
+$ pip install spark-nlp==5.0.2 pyspark==3.3.1 jupyter
 $ jupyter notebook
 ```
 
 Then you can use `python3` kernel to run your code with creating SparkSession via `spark = sparknlp.start()`.
 
 **Optional:**
 
@@ -684,15 +684,15 @@
 
 ```bash
 export SPARK_HOME=/path/to/your/spark/folder
 export PYSPARK_PYTHON=python3
 export PYSPARK_DRIVER_PYTHON=jupyter
 export PYSPARK_DRIVER_PYTHON_OPTS=notebook
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 Alternatively, you can mix in using `--jars` option for pyspark + `pip install spark-nlp`
 
 If not using pyspark at all, you'll have to run the instructions
 pointed [here](#python-without-explicit-pyspark-installation)
 
@@ -711,15 +711,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.1
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.2
 ```
 
 [Spark NLP quick start on Google Colab](https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/examples/python/quick_start_google_colab.ipynb)
 is a live demo on Google Colab that performs named entity recognitions and sentiment analysis by using Spark NLP
 pretrained pipelines.
 
 ## Kaggle Kernel
@@ -734,15 +734,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.1
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.2
 ```
 
 [Spark NLP quick start on Kaggle Kernel](https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark NLP pretrained pipeline.
 
 ## Databricks Cluster
 
@@ -753,17 +753,17 @@
     ```bash
     spark.kryoserializer.buffer.max 2000M
     spark.serializer org.apache.spark.serializer.KryoSerializer
     ```
 
 3. In `Libraries` tab inside your cluster you need to follow these steps:
 
-   3.1. Install New -> PyPI -> `spark-nlp==5.0.1` -> Install
+   3.1. Install New -> PyPI -> `spark-nlp==5.0.2` -> Install
 
-   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1` -> Install
+   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2` -> Install
 
 4. Now you can attach your notebook to the cluster and use Spark NLP!
 
 NOTE: Databricks' runtimes support different Apache Spark major releases. Please make sure you choose the correct Spark
 NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-cheatsheet)
 
@@ -806,24 +806,24 @@
   "Classification": "spark-defaults",
     "Properties": {
       "spark.yarn.stagingDir": "hdfs:///tmp",
       "spark.yarn.preserve.staging.files": "true",
       "spark.kryoserializer.buffer.max": "2000M",
       "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
       "spark.driver.maxResultSize": "0",
-      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1"
+      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2"
     }
 }]
 ```
 
 A sample of AWS CLI to launch EMR cluster:
 
 ```.sh
 aws emr create-cluster \
---name "Spark NLP 5.0.1" \
+--name "Spark NLP 5.0.2" \
 --release-label emr-6.2.0 \
 --applications Name=Hadoop Name=Spark Name=Hive \
 --instance-type m4.4xlarge \
 --instance-count 3 \
 --use-default-roles \
 --log-uri "s3://<S3_BUCKET>/" \
 --bootstrap-actions Path=s3://<S3_BUCKET>/emr-bootstrap.sh,Name=custome \
@@ -879,15 +879,15 @@
   --worker-boot-disk-size=128GB \
   --num-workers=2 \
   --bucket=${BUCKET_NAME} \
   --optional-components=JUPYTER \
   --enable-component-gateway \
   --metadata 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-storage' \
   --initialization-actions gs://goog-dataproc-initialization-actions-${REGION}/python/pip-install.sh \
-  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 2. On an existing one, you need to install spark-nlp and spark-nlp-display packages from PyPI.
 
 3. Now, you can attach your notebook to the cluster and use the Spark NLP!
 
 ## Spark NLP Configuration
@@ -918,42 +918,42 @@
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.serializer", "org.apache.spark.serializer.KryoSerializer")
     .config("spark.kryoserializer.buffer.max", "2000m")
     .config("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
     .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
     .getOrCreate()
 ```
 
 **spark-shell:**
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 **pyspark:**
 
 ```sh
 pyspark \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 **Databricks:**
 
 On a new cluster or existing one you need to add the following to the `Advanced Options -> Spark` tab:
 
 ```bash
@@ -1217,24 +1217,24 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars", "/tmp/spark-nlp-assembly-5.0.1.jar")
+    .config("spark.jars", "/tmp/spark-nlp-assembly-5.0.2.jar")
     .getOrCreate()
 ```
 
 - You can download provided Fat JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/releases),
   please pay attention to pick the one that suits your environment depending on the device (CPU/GPU) and Apache Spark
   version (3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x)
 - If you are local, you can load the Fat JAR from your local FileSystem, however, if you are in a cluster setup you need
   to put the Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. (
-  i.e., `hdfs:///tmp/spark-nlp-assembly-5.0.1.jar`)
+  i.e., `hdfs:///tmp/spark-nlp-assembly-5.0.2.jar`)
 
 Example of using pretrained Models and Pipelines in offline:
 
 ```python
 # instead of using pretrained() for online:
 # french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr")
 # you download this model, extract it, and use .load
```

#### html2text {}

```diff
@@ -90,23 +90,23 @@
 entity recognition (Deep learning) - Easy ONNX and TensorFlow integrations -
 GPU Support - Full integration with Spark ML functions - +12000 pre-trained
 models in +200 languages! - +5000 pre-trained pipelines in +200 languages! -
 Multi-lingual NER models: Arabic, Bengali, Chinese, Danish, Dutch, English,
 Finnish, French, German, Hebrew, Italian, Japanese, Korean, Norwegian, Persian,
 Polish, Portuguese, Russian, Spanish, Swedish, Urdu, and more. ## Requirements
 To use Spark NLP you need the following requirements: - Java 8 and 11 - Apache
-Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 5.0.1 is
+Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 5.0.2 is
 built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum
 following NVIDIAÂ® software are only required for GPU support: - NVIDIAÂ® GPU
 drivers version 450.80.02 or higher - CUDAÂ® Toolkit 11.2 - cuDNN SDK 8.1.0 ##
 Quick Start This is a quick example of how to use Spark NLP pre-trained
 pipeline in Python and PySpark: ```sh $ java -version # should be Java 8 or 11
 (Oracle or OpenJDK) $ conda create -n sparknlp python=3.7 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==5.0.1 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
+nlp==5.0.2 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
 ```python # Import Spark NLP from sparknlp.base import * from
 sparknlp.annotator import * from sparknlp.pretrained import PretrainedPipeline
 import sparknlp # Start SparkSession with Spark NLP # start() functions has 3
 parameters: gpu, apple_silicon, and memory # sparknlp.start(gpu=True) will
 start the session with GPU support # sparknlp.start(apple_silicon=True) will
 start the session with macOS M1 & M2 support # sparknlp.start(memory="16G") to
 change the default driver memory in SparkSession spark = sparknlp.start() #
@@ -116,15 +116,15 @@
 Louvre in Paris. """ # Annotate your testing dataset result = pipeline.annotate
 (text) # What's in the pipeline list(result.keys()) Output: ['entities',
 'stem', 'checked', 'lemma', 'document', 'pos', 'token', 'ner', 'embeddings',
 'sentence'] # Check the results result['entities'] Output: ['Mona Lisa',
 'Leonardo', 'Louvre', 'Paris'] ``` For more examples, you can visit our
 dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/
 examples) to showcase all Spark NLP use cases! ## Apache Spark Support Spark
-NLP *5.0.1* has been built on top of Apache Spark 3.4 while fully supports
+NLP *5.0.2* has been built on top of Apache Spark 3.4 while fully supports
 Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x | Spark NLP | Apache Spark
 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache
 Spark 3.2.x | Apache Spark 3.3.x | Apache Spark 3.4.x | |-----------|----------
 ----------|--------------------|--------------------|--------------------|-----
 ---------------|--------------------|--------------------| | 5.0.x | NO | NO |
 YES | YES | YES | YES | YES | | 4.4.x | NO | NO | YES | YES | YES | YES | YES |
 | 4.3.x | NO | NO | YES | YES | YES | YES | NO | | 4.2.x | NO | NO | YES | YES
@@ -141,24 +141,24 @@
 | NO | YES | YES | YES | YES | NO | YES | | 4.4.x | NO | YES | YES | YES | YES
 | NO | YES | | 4.3.x | YES | YES | YES | YES | YES | NO | YES | | 4.2.x | YES |
 YES | YES | YES | YES | NO | YES | | 4.1.x | YES | YES | YES | YES | NO | NO |
 YES | | 4.0.x | YES | YES | YES | YES | NO | NO | YES | | 3.4.x | YES | YES |
 YES | YES | NO | YES | YES | | 3.3.x | YES | YES | YES | NO | NO | YES | YES |
 | 3.2.x | YES | YES | YES | NO | NO | YES | YES | | 3.1.x | YES | YES | YES |
 NO | NO | YES | YES | | 3.0.x | YES | YES | YES | NO | NO | YES | YES | | 2.7.x
-| YES | YES | NO | NO | NO | YES | NO | ## Databricks Support Spark NLP 5.0.1
+| YES | YES | NO | NO | NO | YES | NO | ## Databricks Support Spark NLP 5.0.2
 has been tested and is compatible with the following runtimes: **CPU:** - 9.1 -
 9.1 ML - 10.1 - 10.1 ML - 10.2 - 10.2 ML - 10.3 - 10.3 ML - 10.4 - 10.4 ML -
 10.5 - 10.5 ML - 11.0 - 11.0 ML - 11.1 - 11.1 ML - 11.2 - 11.2 ML - 11.3 - 11.3
 ML - 12.0 - 12.0 ML - 12.1 - 12.1 ML - 12.2 - 12.2 ML - 13.0 - 13.0 ML - 13.1 -
 13.1 ML - 13.2 - 13.2 ML **GPU:** - 9.1 ML & GPU - 10.1 ML & GPU - 10.2 ML &
 GPU - 10.3 ML & GPU - 10.4 ML & GPU - 10.5 ML & GPU - 11.0 ML & GPU - 11.1 ML &
 GPU - 11.2 ML & GPU - 11.3 ML & GPU - 12.0 ML & GPU - 12.1 ML & GPU - 12.2 ML &
 GPU - 13.0 ML & GPU - 13.1 ML & GPU - 13.2 ML & GPU ## EMR Support Spark NLP
-5.0.1 has been tested and is compatible with the following EMR releases: - emr-
+5.0.2 has been tested and is compatible with the following EMR releases: - emr-
 6.2.0 - emr-6.3.0 - emr-6.3.1 - emr-6.4.0 - emr-6.5.0 - emr-6.6.0 - emr-6.7.0 -
 emr-6.8.0 - emr-6.9.0 - emr-6.10.0 - emr-6.11.0 Full list of [Amazon EMR 6.x
 releases](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-release-
 6x.html) NOTE: The EMR 6.1.0 and 6.1.1 are not supported. ## Usage ## Packages
 Cheatsheet This is a cheatsheet for corresponding Spark NLP Maven package to
 Apache Spark / PySpark major version: | Apache Spark | Spark NLP on CPU | Spark
 NLP on GPU | Spark NLP on AArch64 (linux) | Spark NLP on Apple Silicon | |-----
@@ -171,75 +171,75 @@
 these architectures are limited by the community and we had to build most of
 the dependencies by ourselves to make them compatible. We support these two
 architectures, however, they may not work in some environments. ## Spark
 Packages ### Command line (requires internet connection) Spark NLP supports all
 major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x,
 Apache Spark 3.3.x, and Apache Spark 3.4.x #### Apache Spark 3.x (3.0.x, 3.1.x,
 3.2.x, 3.3.x, and 3.4.x - Scala 2.12) ```sh # CPU spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` The `spark-nlp` has been
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` The `spark-nlp` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp). ```sh # GPU spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 ``` The `spark-nlp-gpu` has been
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 ``` The `spark-nlp-gpu` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-gpu). ```sh # AArch64 spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 ``` The `spark-nlp-aarch64`
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 ``` The `spark-nlp-aarch64`
 has been published to the [Maven Repository](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64). ```sh # M1/M2 (Apple Silicon)
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1 spark-
-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1 ``` The
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2 spark-
+submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2 ``` The
 `spark-nlp-silicon` has been published to the [Maven Repository](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon). **NOTE**:
 In case you are using large pretrained models like UniversalSentenceEncoder,
 you need to have the following set in your SparkSession: ```sh spark-shell \ --
 driver-memory 16g \ --conf spark.kryoserializer.buffer.max=2000M \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` ## Scala Spark NLP supports Scala
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` ## Scala Spark NLP supports Scala
 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
 versions. Our packages are deployed to Maven central. To add any of our
 packages as a dependency in your application you can follow these coordinates:
 ### Maven **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
-```xml   com.johnsnowlabs.nlp spark-nlp_2.12 5.0.1  ``` **spark-nlp-gpu:**
-```xml   com.johnsnowlabs.nlp spark-nlp-gpu_2.12 5.0.1  ``` **spark-nlp-
-aarch64:** ```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 5.0.1  ```
+```xml   com.johnsnowlabs.nlp spark-nlp_2.12 5.0.2  ``` **spark-nlp-gpu:**
+```xml   com.johnsnowlabs.nlp spark-nlp-gpu_2.12 5.0.2  ``` **spark-nlp-
+aarch64:** ```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 5.0.2  ```
 **spark-nlp-silicon:** ```xml   com.johnsnowlabs.nlp spark-nlp-silicon_2.12
-5.0.1  ``` ### SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x,
+5.0.2  ``` ### SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x,
 and 3.4.x: ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp libraryDependencies += "com.johnsnowlabs.nlp" %%
-"spark-nlp" % "5.0.1" ``` **spark-nlp-gpu:** ```sbtshell // https://
+"spark-nlp" % "5.0.2" ``` **spark-nlp-gpu:** ```sbtshell // https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.1" ```
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.2" ```
 **spark-nlp-aarch64:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-aarch64 libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.1" ``` **spark-nlp-
+"com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.2" ``` **spark-nlp-
 silicon:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-silicon libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.1" ``` Maven Central:
+"com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.2" ``` Maven Central:
 [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp) If you are interested, there
 is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-
 starter) ## Python Spark NLP supports Python 3.6.x and above depending on your
 major PySpark version. ### Python without explicit Pyspark installation ###
 Pip/Conda If you installed pyspark through pip/conda, you can install `spark-
-nlp` through the same channel. Pip: ```bash pip install spark-nlp==5.0.1 ```
+nlp` through the same channel. Pip: ```bash pip install spark-nlp==5.0.2 ```
 Conda: ```bash conda install -c johnsnowlabs spark-nlp ``` PyPI [spark-nlp
 package](https://pypi.org/project/spark-nlp/) / Anaconda [spark-nlp package]
 (https://anaconda.org/JohnSnowLabs/spark-nlp) Then you'll have to create a
 SparkSession either from Spark NLP: ```python import sparknlp spark =
 sparknlp.start() ``` or manually: ```python spark = SparkSession.builder
 .appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config
 ("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars.packages",
-"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1") .getOrCreate() ``` If using local
+"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2") .getOrCreate() ``` If using local
 jars, you can use `spark.jars` instead for comma-delimited jar files. For
 cluster setups, of course, you'll have to put the jars in a reachable location
 for all driver and executor nodes. **Quick example:** ```python import sparknlp
 from sparknlp.pretrained import PretrainedPipeline # create or get Spark
 Session spark = sparknlp.start() sparknlp.version() spark.version # download,
 load and annotate a text by pre-trained pipeline pipeline = PretrainedPipeline
 ('recognize_entities_dl', 'en') result = pipeline.annotate('The Mona Lisa is a
@@ -252,72 +252,72 @@
 some reason you need to use the JAR, you can either download the Fat JARs
 provided here or download it from [Maven Central](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp). To add JARs to spark programs use the `--jars`
 option: ```sh spark-shell --jars spark-nlp.jar ``` The preferred way to use the
 library when running spark programs is using the `--packages` option as
 specified in the `spark-packages` section. ## Apache Zeppelin Use either one of
 the following options - Add the following Maven Coordinates to the
-interpreter's library list ```bash com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+interpreter's library list ```bash com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ``` - Add a path to pre-built jar from [here](#compiled-jars) in the
 interpreter's library list making sure the jar is available to driver path ###
 Python in Zeppelin Apart from the previous step, install the python module
-through pip ```bash pip install spark-nlp==5.0.1 ``` Or you can install `spark-
+through pip ```bash pip install spark-nlp==5.0.2 ``` Or you can install `spark-
 nlp` from inside Zeppelin by using Conda: ```bash python.conda install -
 c johnsnowlabs spark-nlp ``` Configure Zeppelin properly, use cells with
 %spark.pyspark or any interpreter name you chose. Finally, in Zeppelin
 interpreter settings, make sure you set properly zeppelin.python to the python
 you want to use and install the pip library with (e.g. `python3`). An
 alternative option would be to set `SPARK_SUBMIT_OPTIONS` (zeppelin-env.sh) and
 make sure `--packages` is there as shown earlier since it includes both scala
 and python side installation. ## Jupyter Notebook (Python) **Recommended:** The
 easiest way to get this done on Linux and macOS is to simply install `spark-
 nlp` and `pyspark` PyPI packages and launch the Jupyter from the same Python
 environment: ```sh $ conda create -n sparknlp python=3.8 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==5.0.1 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
+nlp==5.0.2 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
 `python3` kernel to run your code with creating SparkSession via `spark =
 sparknlp.start()`. **Optional:** If you are in different operating systems and
 require to make Jupyter Notebook run by using pyspark, you can follow these
 steps: ```bash export SPARK_HOME=/path/to/your/spark/folder export
 PYSPARK_PYTHON=python3 export PYSPARK_DRIVER_PYTHON=jupyter export
 PYSPARK_DRIVER_PYTHON_OPTS=notebook pyspark --packages com.johnsnowlabs.nlp:
-spark-nlp_2.12:5.0.1 ``` Alternatively, you can mix in using `--jars` option
+spark-nlp_2.12:5.0.2 ``` Alternatively, you can mix in using `--jars` option
 for pyspark + `pip install spark-nlp` If not using pyspark at all, you'll have
 to run the instructions pointed [here](#python-without-explicit-pyspark-
 installation) ## Google Colab Notebook Google Colab is perhaps the easiest way
 to get started with spark-nlp. It requires no installation or setup other than
 having a Google account. Run the following code in Google Colab notebook and
 start using spark-nlp right away. ```sh # This is only to setup PySpark and
 Spark NLP on Colab !wget https://setup.johnsnowlabs.com/colab.sh -O - | bash
 ``` This script comes with the two options to define `pyspark` and `spark-nlp`
 versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -g will
 enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 5.0.1 ``` [Spark NLP quick start on Google Colab]
+bash /dev/stdin -p 3.2.3 -s 5.0.2 ``` [Spark NLP quick start on Google Colab]
 (https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/
 examples/python/quick_start_google_colab.ipynb) is a live demo on Google Colab
 that performs named entity recognitions and sentiment analysis by using Spark
 NLP pretrained pipelines. ## Kaggle Kernel Run the following code in Kaggle
 Kernel and start using spark-nlp right away. ```sh # Let's setup Kaggle for
 Spark NLP and PySpark !wget https://setup.johnsnowlabs.com/kaggle.sh -O - |
 bash ``` This script comes with the two options to define `pyspark` and `spark-
 nlp` versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -
 g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 5.0.1 ``` [Spark NLP quick start on Kaggle Kernel]
+bash /dev/stdin -p 3.2.3 -s 5.0.2 ``` [Spark NLP quick start on Kaggle Kernel]
 (https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark
 NLP pretrained pipeline. ## Databricks Cluster 1. Create a cluster if you don't
 have one already 2. On a new cluster or existing one you need to add the
 following to the `Advanced Options -> Spark` tab: ```bash
 spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer ``` 3. In `Libraries` tab inside
 your cluster you need to follow these steps: 3.1. Install New -> PyPI -
-> `spark-nlp==5.0.1` -> Install 3.2. Install New -> Maven -> Coordinates -
-> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1` -> Install 4. Now you can attach
+> `spark-nlp==5.0.2` -> Install 3.2. Install New -> Maven -> Coordinates -
+> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2` -> Install 4. Now you can attach
 your notebook to the cluster and use Spark NLP! NOTE: Databricks' runtimes
 support different Apache Spark major releases. Please make sure you choose the
 correct Spark NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-
 cheatsheet) ## EMR Cluster To launch EMR clusters with Apache Spark/PySpark and
 Spark NLP correctly you need to have bootstrap and software configuration. A
 sample of your bootstrap script ```.sh #!/bin/bash set -x -e echo -e 'export
@@ -328,16 +328,16 @@
 S3 (must be public access): ```.json [{ "Classification": "spark-env",
 "Configurations": [{ "Classification": "export", "Properties":
 { "PYSPARK_PYTHON": "/usr/bin/python3" } }] }, { "Classification": "spark-
 defaults", "Properties": { "spark.yarn.stagingDir": "hdfs:///tmp",
 "spark.yarn.preserve.staging.files": "true", "spark.kryoserializer.buffer.max":
 "2000M", "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
 "spark.driver.maxResultSize": "0", "spark.jars.packages":
-"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1" } }] ``` A sample of AWS CLI to
-launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 5.0.1" \
+"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2" } }] ``` A sample of AWS CLI to
+launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 5.0.2" \
 --release-label emr-6.2.0 \ --applications Name=Hadoop Name=Spark Name=Hive \ -
 -instance-type m4.4xlarge \ --instance-count 3 \ --use-default-roles \ --log-
 uri "s3:///" \ --bootstrap-actions Path=s3:///emr-bootstrap.sh,Name=custome \ -
 -configurations "https:///sparknlp-config.json" \ --ec2-attributes
 KeyName=,EmrManagedMasterSecurityGroup=,EmrManagedSlaveSecurityGroup= \ --
 profile  ``` ## GCP Dataproc 1. Create a cluster if you don't have one already
 as follows. At gcloud shell: ```bash gcloud services enable
@@ -356,15 +356,15 @@
 boot-disk-size=128GB \ --num-workers=2 \ --bucket=${BUCKET_NAME} \ --optional-
 components=JUPYTER \ --enable-component-gateway \ --metadata
 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-
 storage' \ --initialization-actions gs://goog-dataproc-initialization-actions-$
 {REGION}/python/pip-install.sh \ --properties spark:
 spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:
 spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:
-spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` 2. On an
+spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` 2. On an
 existing one, you need to install spark-nlp and spark-nlp-display packages from
 PyPI. 3. Now, you can attach your notebook to the cluster and use the Spark
 NLP! ## Spark NLP Configuration You can change the following Spark NLP
 configurations via Spark Configuration: | Property Name | Default | Meaning |
 |--------------------------------------------------------|---------------------
 -|-----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -400,28 +400,28 @@
 configurations. ```python from pyspark.sql import SparkSession spark =
 SparkSession.builder .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config("spark.serializer",
 "org.apache.spark.serializer.KryoSerializer") .config
 ("spark.kryoserializer.buffer.max", "2000m") .config
 ("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
 .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
 .getOrCreate() ``` **spark-shell:** ```sh spark-shell \ --driver-memory 16g \ -
 -conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` **pyspark:** ```sh pyspark \ --
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` **pyspark:** ```sh pyspark \ --
 driver-memory 16g \ --conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` **Databricks:** On a new cluster
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` **Databricks:** On a new cluster
 or existing one you need to add the following to the `Advanced Options -
 > Spark` tab: ```bash spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer
 spark.jsl.settings.pretrained.cache_folder dbfs:/PATH_TO_CACHE
 spark.jsl.settings.storage.cluster_tmp_dir dbfs:/PATH_TO_STORAGE
 spark.jsl.settings.annotator.log_folder dbfs:/PATH_TO_LOGS ``` NOTE: If this is
 an existing cluster, after adding new configs or changing existing properties
@@ -555,22 +555,22 @@
 pipelines or the `.pretrained()` function to download pretrained models, you
 will need to manually download your pipeline/model from [Models Hub](https://
 sparknlp.org/models), extract it, and load it. Example of `SparkSession` with
 Fat JAR to have Spark NLP offline: ```python spark = SparkSession.builder
 .appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config
 ("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars", "/tmp/spark-
-nlp-assembly-5.0.1.jar") .getOrCreate() ``` - You can download provided Fat
+nlp-assembly-5.0.2.jar") .getOrCreate() ``` - You can download provided Fat
 JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/
 releases), please pay attention to pick the one that suits your environment
 depending on the device (CPU/GPU) and Apache Spark version (3.0.x, 3.1.x,
 3.2.x, 3.3.x, and 3.4.x) - If you are local, you can load the Fat JAR from your
 local FileSystem, however, if you are in a cluster setup you need to put the
 Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. ( i.e., `hdfs:
-///tmp/spark-nlp-assembly-5.0.1.jar`) Example of using pretrained Models and
+///tmp/spark-nlp-assembly-5.0.2.jar`) Example of using pretrained Models and
 Pipelines in offline: ```python # instead of using pretrained() for online: #
 french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr") # you download
 this model, extract it, and use .load french_pos = PerceptronModel.load("/tmp/
 pos_ud_gsd_fr_2.0.2_2.4_1556531457346/") .setInputCols("document", "token")
 .setOutputCol("pos") # example for pipelines # instead of using
 PretrainedPipeline # pipeline = PretrainedPipeline('explain_document_dl',
 lang='en') # you download this pipeline, extract it, and use PipelineModel
```

### Comparing `spark-nlp-5.0.1/setup.py` & `spark-nlp-5.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
 
-    version='5.0.1',  # Required
+    version='5.0.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the 'Summary' metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='John Snow Labs Spark NLP is a natural language processing library built on top of Apache Spark ML. It provides simple, performant & accurate NLP annotations for machine learning pipelines, that scale easily in a distributed environment.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `spark-nlp-5.0.1/spark_nlp.egg-info/PKG-INFO` & `spark-nlp-5.0.2/spark_nlp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-nlp
-Version: 5.0.1
+Version: 5.0.2
 Summary: John Snow Labs Spark NLP is a natural language processing library built on top of Apache Spark ML. It provides simple, performant & accurate NLP annotations for machine learning pipelines, that scale easily in a distributed environment.
 Home-page: https://github.com/JohnSnowLabs/spark-nlp
 Author: John Snow Labs
 Keywords: NLP spark vision speech deep learning transformer tensorflow BERT GPT-2 Wav2Vec2 ViT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -195,15 +195,15 @@
 To use Spark NLP you need the following requirements:
 
 - Java 8 and 11
 - Apache Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x
 
 **GPU (optional):**
 
-Spark NLP 5.0.1 is built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum following NVIDIA® software are only required for GPU support:
+Spark NLP 5.0.2 is built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum following NVIDIA® software are only required for GPU support:
 
 - NVIDIA® GPU drivers version 450.80.02 or higher
 - CUDA® Toolkit 11.2
 - cuDNN SDK 8.1.0
 
 ## Quick Start
 
@@ -211,15 +211,15 @@
 
 ```sh
 $ java -version
 # should be Java 8 or 11 (Oracle or OpenJDK)
 $ conda create -n sparknlp python=3.7 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==5.0.1 pyspark==3.3.1
+$ pip install spark-nlp==5.0.2 pyspark==3.3.1
 ```
 
 In Python console or Jupyter `Python3` kernel:
 
 ```python
 # Import Spark NLP
 from sparknlp.base import *
@@ -256,15 +256,15 @@
 Output: ['Mona Lisa', 'Leonardo', 'Louvre', 'Paris']
 ```
 
 For more examples, you can visit our dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples) to showcase all Spark NLP use cases!
 
 ## Apache Spark Support
 
-Spark NLP *5.0.1* has been built on top of Apache Spark 3.4 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
+Spark NLP *5.0.2* has been built on top of Apache Spark 3.4 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
 
 | Spark NLP | Apache Spark 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache Spark 3.2.x | Apache Spark 3.3.x | Apache Spark 3.4.x |
 |-----------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
 | 5.0.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | YES                |
 | 4.4.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | YES                |
 | 4.3.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | NO                 |
 | 4.2.x     | NO                 | NO                 | YES                | YES                | YES                | YES                | NO                 |
@@ -295,15 +295,15 @@
 | 3.2.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 3.1.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 3.0.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
 | 2.7.x     | YES        | YES        | NO         | NO         | NO         | YES        | NO         |
 
 ## Databricks Support
 
-Spark NLP 5.0.1 has been tested and is compatible with the following runtimes:
+Spark NLP 5.0.2 has been tested and is compatible with the following runtimes:
 
 **CPU:**
 
 - 9.1
 - 9.1 ML
 - 10.1
 - 10.1 ML
@@ -353,15 +353,15 @@
 - 12.2 ML & GPU
 - 13.0 ML & GPU
 - 13.1 ML & GPU
 - 13.2 ML & GPU
 
 ## EMR Support
 
-Spark NLP 5.0.1 has been tested and is compatible with the following EMR releases:
+Spark NLP 5.0.2 has been tested and is compatible with the following EMR releases:
 
 - emr-6.2.0
 - emr-6.3.0
 - emr-6.3.1
 - emr-6.4.0
 - emr-6.5.0
 - emr-6.6.0
@@ -397,74 +397,74 @@
 Spark NLP supports all major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x, Apache Spark 3.3.x, and Apache Spark 3.4.x
 
 #### Apache Spark 3.x (3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x - Scala 2.12)
 
 ```sh
 # CPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 The `spark-nlp` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp).
 
 ```sh
 # GPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2
 
 ```
 
 The `spark-nlp-gpu` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu).
 
 ```sh
 # AArch64
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2
 
 ```
 
 The `spark-nlp-aarch64` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64).
 
 ```sh
 # M1/M2 (Apple Silicon)
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
 
 ```
 
 The `spark-nlp-silicon` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon).
 
 **NOTE**: In case you are using large pretrained models like UniversalSentenceEncoder, you need to have the following
 set in your SparkSession:
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.kryoserializer.buffer.max=2000M \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 ## Scala
 
 Spark NLP supports Scala 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x versions. Our packages are
 deployed to Maven central. To add any of our packages as a dependency in your application you can follow these
 coordinates:
@@ -474,79 +474,79 @@
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-gpu:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-gpu_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-aarch64:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64 -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-aarch64_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 **spark-nlp-silicon:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-silicon_2.12</artifactId>
-    <version>5.0.1</version>
+    <version>5.0.2</version>
 </dependency>
 ```
 
 ### SBT
 
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "5.0.2"
 ```
 
 **spark-nlp-gpu:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.2"
 ```
 
 **spark-nlp-aarch64:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.2"
 ```
 
 **spark-nlp-silicon:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.1"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.2"
 ```
 
 Maven
 Central: [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp)
 
 If you are interested, there is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-starter)
@@ -560,15 +560,15 @@
 ### Pip/Conda
 
 If you installed pyspark through pip/conda, you can install `spark-nlp` through the same channel.
 
 Pip:
 
 ```bash
-pip install spark-nlp==5.0.1
+pip install spark-nlp==5.0.2
 ```
 
 Conda:
 
 ```bash
 conda install -c johnsnowlabs spark-nlp
 ```
@@ -589,15 +589,15 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
     .getOrCreate()
 ```
 
 If using local jars, you can use `spark.jars` instead for comma-delimited jar files. For cluster setups, of course,
 you'll have to put the jars in a reachable location for all driver and executor nodes.
 
 **Quick example:**
@@ -660,26 +660,26 @@
 ## Apache Zeppelin
 
 Use either one of the following options
 
 - Add the following Maven Coordinates to the interpreter's library list
 
 ```bash
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 - Add a path to pre-built jar from [here](#compiled-jars) in the interpreter's library list making sure the jar is
   available to driver path
 
 ### Python in Zeppelin
 
 Apart from the previous step, install the python module through pip
 
 ```bash
-pip install spark-nlp==5.0.1
+pip install spark-nlp==5.0.2
 ```
 
 Or you can install `spark-nlp` from inside Zeppelin by using Conda:
 
 ```bash
 python.conda install -c johnsnowlabs spark-nlp
 ```
@@ -699,15 +699,15 @@
 The easiest way to get this done on Linux and macOS is to simply install `spark-nlp` and `pyspark` PyPI packages and
 launch the Jupyter from the same Python environment:
 
 ```sh
 $ conda create -n sparknlp python=3.8 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==5.0.1 pyspark==3.3.1 jupyter
+$ pip install spark-nlp==5.0.2 pyspark==3.3.1 jupyter
 $ jupyter notebook
 ```
 
 Then you can use `python3` kernel to run your code with creating SparkSession via `spark = sparknlp.start()`.
 
 **Optional:**
 
@@ -716,15 +716,15 @@
 
 ```bash
 export SPARK_HOME=/path/to/your/spark/folder
 export PYSPARK_PYTHON=python3
 export PYSPARK_DRIVER_PYTHON=jupyter
 export PYSPARK_DRIVER_PYTHON_OPTS=notebook
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 Alternatively, you can mix in using `--jars` option for pyspark + `pip install spark-nlp`
 
 If not using pyspark at all, you'll have to run the instructions
 pointed [here](#python-without-explicit-pyspark-installation)
 
@@ -743,15 +743,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.1
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.2
 ```
 
 [Spark NLP quick start on Google Colab](https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/examples/python/quick_start_google_colab.ipynb)
 is a live demo on Google Colab that performs named entity recognitions and sentiment analysis by using Spark NLP
 pretrained pipelines.
 
 ## Kaggle Kernel
@@ -766,15 +766,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.1
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 5.0.2
 ```
 
 [Spark NLP quick start on Kaggle Kernel](https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark NLP pretrained pipeline.
 
 ## Databricks Cluster
 
@@ -785,17 +785,17 @@
     ```bash
     spark.kryoserializer.buffer.max 2000M
     spark.serializer org.apache.spark.serializer.KryoSerializer
     ```
 
 3. In `Libraries` tab inside your cluster you need to follow these steps:
 
-   3.1. Install New -> PyPI -> `spark-nlp==5.0.1` -> Install
+   3.1. Install New -> PyPI -> `spark-nlp==5.0.2` -> Install
 
-   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1` -> Install
+   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2` -> Install
 
 4. Now you can attach your notebook to the cluster and use Spark NLP!
 
 NOTE: Databricks' runtimes support different Apache Spark major releases. Please make sure you choose the correct Spark
 NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-cheatsheet)
 
@@ -838,24 +838,24 @@
   "Classification": "spark-defaults",
     "Properties": {
       "spark.yarn.stagingDir": "hdfs:///tmp",
       "spark.yarn.preserve.staging.files": "true",
       "spark.kryoserializer.buffer.max": "2000M",
       "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
       "spark.driver.maxResultSize": "0",
-      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1"
+      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2"
     }
 }]
 ```
 
 A sample of AWS CLI to launch EMR cluster:
 
 ```.sh
 aws emr create-cluster \
---name "Spark NLP 5.0.1" \
+--name "Spark NLP 5.0.2" \
 --release-label emr-6.2.0 \
 --applications Name=Hadoop Name=Spark Name=Hive \
 --instance-type m4.4xlarge \
 --instance-count 3 \
 --use-default-roles \
 --log-uri "s3://<S3_BUCKET>/" \
 --bootstrap-actions Path=s3://<S3_BUCKET>/emr-bootstrap.sh,Name=custome \
@@ -911,15 +911,15 @@
   --worker-boot-disk-size=128GB \
   --num-workers=2 \
   --bucket=${BUCKET_NAME} \
   --optional-components=JUPYTER \
   --enable-component-gateway \
   --metadata 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-storage' \
   --initialization-actions gs://goog-dataproc-initialization-actions-${REGION}/python/pip-install.sh \
-  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 2. On an existing one, you need to install spark-nlp and spark-nlp-display packages from PyPI.
 
 3. Now, you can attach your notebook to the cluster and use the Spark NLP!
 
 ## Spark NLP Configuration
@@ -950,42 +950,42 @@
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.serializer", "org.apache.spark.serializer.KryoSerializer")
     .config("spark.kryoserializer.buffer.max", "2000m")
     .config("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
     .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
     .getOrCreate()
 ```
 
 **spark-shell:**
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 **pyspark:**
 
 ```sh
 pyspark \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ```
 
 **Databricks:**
 
 On a new cluster or existing one you need to add the following to the `Advanced Options -> Spark` tab:
 
 ```bash
@@ -1249,24 +1249,24 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars", "/tmp/spark-nlp-assembly-5.0.1.jar")
+    .config("spark.jars", "/tmp/spark-nlp-assembly-5.0.2.jar")
     .getOrCreate()
 ```
 
 - You can download provided Fat JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/releases),
   please pay attention to pick the one that suits your environment depending on the device (CPU/GPU) and Apache Spark
   version (3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x)
 - If you are local, you can load the Fat JAR from your local FileSystem, however, if you are in a cluster setup you need
   to put the Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. (
-  i.e., `hdfs:///tmp/spark-nlp-assembly-5.0.1.jar`)
+  i.e., `hdfs:///tmp/spark-nlp-assembly-5.0.2.jar`)
 
 Example of using pretrained Models and Pipelines in offline:
 
 ```python
 # instead of using pretrained() for online:
 # french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr")
 # you download this model, extract it, and use .load
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spark-nlp Version: 5.0.1 Summary: John Snow Labs
+Metadata-Version: 2.1 Name: spark-nlp Version: 5.0.2 Summary: John Snow Labs
 Spark NLP is a natural language processing library built on top of Apache Spark
 ML. It provides simple, performant & accurate NLP annotations for machine
 learning pipelines, that scale easily in a distributed environment. Home-page:
 https://github.com/JohnSnowLabs/spark-nlp Author: John Snow Labs Keywords: NLP
 spark vision speech deep learning transformer tensorflow BERT GPT-2 Wav2Vec2
 ViT Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
@@ -113,23 +113,23 @@
 entity recognition (Deep learning) - Easy ONNX and TensorFlow integrations -
 GPU Support - Full integration with Spark ML functions - +12000 pre-trained
 models in +200 languages! - +5000 pre-trained pipelines in +200 languages! -
 Multi-lingual NER models: Arabic, Bengali, Chinese, Danish, Dutch, English,
 Finnish, French, German, Hebrew, Italian, Japanese, Korean, Norwegian, Persian,
 Polish, Portuguese, Russian, Spanish, Swedish, Urdu, and more. ## Requirements
 To use Spark NLP you need the following requirements: - Java 8 and 11 - Apache
-Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 5.0.1 is
+Spark 3.4.x, 3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 5.0.2 is
 built with ONNX 1.15.1 and TensorFlow 2.7.1 deep learning engines. The minimum
 following NVIDIAÂ® software are only required for GPU support: - NVIDIAÂ® GPU
 drivers version 450.80.02 or higher - CUDAÂ® Toolkit 11.2 - cuDNN SDK 8.1.0 ##
 Quick Start This is a quick example of how to use Spark NLP pre-trained
 pipeline in Python and PySpark: ```sh $ java -version # should be Java 8 or 11
 (Oracle or OpenJDK) $ conda create -n sparknlp python=3.7 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==5.0.1 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
+nlp==5.0.2 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
 ```python # Import Spark NLP from sparknlp.base import * from
 sparknlp.annotator import * from sparknlp.pretrained import PretrainedPipeline
 import sparknlp # Start SparkSession with Spark NLP # start() functions has 3
 parameters: gpu, apple_silicon, and memory # sparknlp.start(gpu=True) will
 start the session with GPU support # sparknlp.start(apple_silicon=True) will
 start the session with macOS M1 & M2 support # sparknlp.start(memory="16G") to
 change the default driver memory in SparkSession spark = sparknlp.start() #
@@ -139,15 +139,15 @@
 Louvre in Paris. """ # Annotate your testing dataset result = pipeline.annotate
 (text) # What's in the pipeline list(result.keys()) Output: ['entities',
 'stem', 'checked', 'lemma', 'document', 'pos', 'token', 'ner', 'embeddings',
 'sentence'] # Check the results result['entities'] Output: ['Mona Lisa',
 'Leonardo', 'Louvre', 'Paris'] ``` For more examples, you can visit our
 dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/
 examples) to showcase all Spark NLP use cases! ## Apache Spark Support Spark
-NLP *5.0.1* has been built on top of Apache Spark 3.4 while fully supports
+NLP *5.0.2* has been built on top of Apache Spark 3.4 while fully supports
 Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x | Spark NLP | Apache Spark
 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache
 Spark 3.2.x | Apache Spark 3.3.x | Apache Spark 3.4.x | |-----------|----------
 ----------|--------------------|--------------------|--------------------|-----
 ---------------|--------------------|--------------------| | 5.0.x | NO | NO |
 YES | YES | YES | YES | YES | | 4.4.x | NO | NO | YES | YES | YES | YES | YES |
 | 4.3.x | NO | NO | YES | YES | YES | YES | NO | | 4.2.x | NO | NO | YES | YES
@@ -164,24 +164,24 @@
 | NO | YES | YES | YES | YES | NO | YES | | 4.4.x | NO | YES | YES | YES | YES
 | NO | YES | | 4.3.x | YES | YES | YES | YES | YES | NO | YES | | 4.2.x | YES |
 YES | YES | YES | YES | NO | YES | | 4.1.x | YES | YES | YES | YES | NO | NO |
 YES | | 4.0.x | YES | YES | YES | YES | NO | NO | YES | | 3.4.x | YES | YES |
 YES | YES | NO | YES | YES | | 3.3.x | YES | YES | YES | NO | NO | YES | YES |
 | 3.2.x | YES | YES | YES | NO | NO | YES | YES | | 3.1.x | YES | YES | YES |
 NO | NO | YES | YES | | 3.0.x | YES | YES | YES | NO | NO | YES | YES | | 2.7.x
-| YES | YES | NO | NO | NO | YES | NO | ## Databricks Support Spark NLP 5.0.1
+| YES | YES | NO | NO | NO | YES | NO | ## Databricks Support Spark NLP 5.0.2
 has been tested and is compatible with the following runtimes: **CPU:** - 9.1 -
 9.1 ML - 10.1 - 10.1 ML - 10.2 - 10.2 ML - 10.3 - 10.3 ML - 10.4 - 10.4 ML -
 10.5 - 10.5 ML - 11.0 - 11.0 ML - 11.1 - 11.1 ML - 11.2 - 11.2 ML - 11.3 - 11.3
 ML - 12.0 - 12.0 ML - 12.1 - 12.1 ML - 12.2 - 12.2 ML - 13.0 - 13.0 ML - 13.1 -
 13.1 ML - 13.2 - 13.2 ML **GPU:** - 9.1 ML & GPU - 10.1 ML & GPU - 10.2 ML &
 GPU - 10.3 ML & GPU - 10.4 ML & GPU - 10.5 ML & GPU - 11.0 ML & GPU - 11.1 ML &
 GPU - 11.2 ML & GPU - 11.3 ML & GPU - 12.0 ML & GPU - 12.1 ML & GPU - 12.2 ML &
 GPU - 13.0 ML & GPU - 13.1 ML & GPU - 13.2 ML & GPU ## EMR Support Spark NLP
-5.0.1 has been tested and is compatible with the following EMR releases: - emr-
+5.0.2 has been tested and is compatible with the following EMR releases: - emr-
 6.2.0 - emr-6.3.0 - emr-6.3.1 - emr-6.4.0 - emr-6.5.0 - emr-6.6.0 - emr-6.7.0 -
 emr-6.8.0 - emr-6.9.0 - emr-6.10.0 - emr-6.11.0 Full list of [Amazon EMR 6.x
 releases](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-release-
 6x.html) NOTE: The EMR 6.1.0 and 6.1.1 are not supported. ## Usage ## Packages
 Cheatsheet This is a cheatsheet for corresponding Spark NLP Maven package to
 Apache Spark / PySpark major version: | Apache Spark | Spark NLP on CPU | Spark
 NLP on GPU | Spark NLP on AArch64 (linux) | Spark NLP on Apple Silicon | |-----
@@ -194,75 +194,75 @@
 these architectures are limited by the community and we had to build most of
 the dependencies by ourselves to make them compatible. We support these two
 architectures, however, they may not work in some environments. ## Spark
 Packages ### Command line (requires internet connection) Spark NLP supports all
 major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x,
 Apache Spark 3.3.x, and Apache Spark 3.4.x #### Apache Spark 3.x (3.0.x, 3.1.x,
 3.2.x, 3.3.x, and 3.4.x - Scala 2.12) ```sh # CPU spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` The `spark-nlp` has been
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` The `spark-nlp` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp). ```sh # GPU spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.1 ``` The `spark-nlp-gpu` has been
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:5.0.2 ``` The `spark-nlp-gpu` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-gpu). ```sh # AArch64 spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.1 ``` The `spark-nlp-aarch64`
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:5.0.2 ``` The `spark-nlp-aarch64`
 has been published to the [Maven Repository](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64). ```sh # M1/M2 (Apple Silicon)
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1 spark-
-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.1 ``` The
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2 spark-
+submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:5.0.2 ``` The
 `spark-nlp-silicon` has been published to the [Maven Repository](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon). **NOTE**:
 In case you are using large pretrained models like UniversalSentenceEncoder,
 you need to have the following set in your SparkSession: ```sh spark-shell \ --
 driver-memory 16g \ --conf spark.kryoserializer.buffer.max=2000M \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` ## Scala Spark NLP supports Scala
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` ## Scala Spark NLP supports Scala
 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x
 versions. Our packages are deployed to Maven central. To add any of our
 packages as a dependency in your application you can follow these coordinates:
 ### Maven **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x, and 3.4.x:
-```xml   com.johnsnowlabs.nlp spark-nlp_2.12 5.0.1  ``` **spark-nlp-gpu:**
-```xml   com.johnsnowlabs.nlp spark-nlp-gpu_2.12 5.0.1  ``` **spark-nlp-
-aarch64:** ```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 5.0.1  ```
+```xml   com.johnsnowlabs.nlp spark-nlp_2.12 5.0.2  ``` **spark-nlp-gpu:**
+```xml   com.johnsnowlabs.nlp spark-nlp-gpu_2.12 5.0.2  ``` **spark-nlp-
+aarch64:** ```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 5.0.2  ```
 **spark-nlp-silicon:** ```xml   com.johnsnowlabs.nlp spark-nlp-silicon_2.12
-5.0.1  ``` ### SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x,
+5.0.2  ``` ### SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, 3.3.x,
 and 3.4.x: ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp libraryDependencies += "com.johnsnowlabs.nlp" %%
-"spark-nlp" % "5.0.1" ``` **spark-nlp-gpu:** ```sbtshell // https://
+"spark-nlp" % "5.0.2" ``` **spark-nlp-gpu:** ```sbtshell // https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.1" ```
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "5.0.2" ```
 **spark-nlp-aarch64:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-aarch64 libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.1" ``` **spark-nlp-
+"com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "5.0.2" ``` **spark-nlp-
 silicon:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-silicon libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.1" ``` Maven Central:
+"com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "5.0.2" ``` Maven Central:
 [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp) If you are interested, there
 is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-
 starter) ## Python Spark NLP supports Python 3.6.x and above depending on your
 major PySpark version. ### Python without explicit Pyspark installation ###
 Pip/Conda If you installed pyspark through pip/conda, you can install `spark-
-nlp` through the same channel. Pip: ```bash pip install spark-nlp==5.0.1 ```
+nlp` through the same channel. Pip: ```bash pip install spark-nlp==5.0.2 ```
 Conda: ```bash conda install -c johnsnowlabs spark-nlp ``` PyPI [spark-nlp
 package](https://pypi.org/project/spark-nlp/) / Anaconda [spark-nlp package]
 (https://anaconda.org/JohnSnowLabs/spark-nlp) Then you'll have to create a
 SparkSession either from Spark NLP: ```python import sparknlp spark =
 sparknlp.start() ``` or manually: ```python spark = SparkSession.builder
 .appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config
 ("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars.packages",
-"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1") .getOrCreate() ``` If using local
+"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2") .getOrCreate() ``` If using local
 jars, you can use `spark.jars` instead for comma-delimited jar files. For
 cluster setups, of course, you'll have to put the jars in a reachable location
 for all driver and executor nodes. **Quick example:** ```python import sparknlp
 from sparknlp.pretrained import PretrainedPipeline # create or get Spark
 Session spark = sparknlp.start() sparknlp.version() spark.version # download,
 load and annotate a text by pre-trained pipeline pipeline = PretrainedPipeline
 ('recognize_entities_dl', 'en') result = pipeline.annotate('The Mona Lisa is a
@@ -275,72 +275,72 @@
 some reason you need to use the JAR, you can either download the Fat JARs
 provided here or download it from [Maven Central](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp). To add JARs to spark programs use the `--jars`
 option: ```sh spark-shell --jars spark-nlp.jar ``` The preferred way to use the
 library when running spark programs is using the `--packages` option as
 specified in the `spark-packages` section. ## Apache Zeppelin Use either one of
 the following options - Add the following Maven Coordinates to the
-interpreter's library list ```bash com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1
+interpreter's library list ```bash com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2
 ``` - Add a path to pre-built jar from [here](#compiled-jars) in the
 interpreter's library list making sure the jar is available to driver path ###
 Python in Zeppelin Apart from the previous step, install the python module
-through pip ```bash pip install spark-nlp==5.0.1 ``` Or you can install `spark-
+through pip ```bash pip install spark-nlp==5.0.2 ``` Or you can install `spark-
 nlp` from inside Zeppelin by using Conda: ```bash python.conda install -
 c johnsnowlabs spark-nlp ``` Configure Zeppelin properly, use cells with
 %spark.pyspark or any interpreter name you chose. Finally, in Zeppelin
 interpreter settings, make sure you set properly zeppelin.python to the python
 you want to use and install the pip library with (e.g. `python3`). An
 alternative option would be to set `SPARK_SUBMIT_OPTIONS` (zeppelin-env.sh) and
 make sure `--packages` is there as shown earlier since it includes both scala
 and python side installation. ## Jupyter Notebook (Python) **Recommended:** The
 easiest way to get this done on Linux and macOS is to simply install `spark-
 nlp` and `pyspark` PyPI packages and launch the Jupyter from the same Python
 environment: ```sh $ conda create -n sparknlp python=3.8 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==5.0.1 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
+nlp==5.0.2 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
 `python3` kernel to run your code with creating SparkSession via `spark =
 sparknlp.start()`. **Optional:** If you are in different operating systems and
 require to make Jupyter Notebook run by using pyspark, you can follow these
 steps: ```bash export SPARK_HOME=/path/to/your/spark/folder export
 PYSPARK_PYTHON=python3 export PYSPARK_DRIVER_PYTHON=jupyter export
 PYSPARK_DRIVER_PYTHON_OPTS=notebook pyspark --packages com.johnsnowlabs.nlp:
-spark-nlp_2.12:5.0.1 ``` Alternatively, you can mix in using `--jars` option
+spark-nlp_2.12:5.0.2 ``` Alternatively, you can mix in using `--jars` option
 for pyspark + `pip install spark-nlp` If not using pyspark at all, you'll have
 to run the instructions pointed [here](#python-without-explicit-pyspark-
 installation) ## Google Colab Notebook Google Colab is perhaps the easiest way
 to get started with spark-nlp. It requires no installation or setup other than
 having a Google account. Run the following code in Google Colab notebook and
 start using spark-nlp right away. ```sh # This is only to setup PySpark and
 Spark NLP on Colab !wget https://setup.johnsnowlabs.com/colab.sh -O - | bash
 ``` This script comes with the two options to define `pyspark` and `spark-nlp`
 versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -g will
 enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 5.0.1 ``` [Spark NLP quick start on Google Colab]
+bash /dev/stdin -p 3.2.3 -s 5.0.2 ``` [Spark NLP quick start on Google Colab]
 (https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/
 examples/python/quick_start_google_colab.ipynb) is a live demo on Google Colab
 that performs named entity recognitions and sentiment analysis by using Spark
 NLP pretrained pipelines. ## Kaggle Kernel Run the following code in Kaggle
 Kernel and start using spark-nlp right away. ```sh # Let's setup Kaggle for
 Spark NLP and PySpark !wget https://setup.johnsnowlabs.com/kaggle.sh -O - |
 bash ``` This script comes with the two options to define `pyspark` and `spark-
 nlp` versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -
 g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 5.0.1 ``` [Spark NLP quick start on Kaggle Kernel]
+bash /dev/stdin -p 3.2.3 -s 5.0.2 ``` [Spark NLP quick start on Kaggle Kernel]
 (https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark
 NLP pretrained pipeline. ## Databricks Cluster 1. Create a cluster if you don't
 have one already 2. On a new cluster or existing one you need to add the
 following to the `Advanced Options -> Spark` tab: ```bash
 spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer ``` 3. In `Libraries` tab inside
 your cluster you need to follow these steps: 3.1. Install New -> PyPI -
-> `spark-nlp==5.0.1` -> Install 3.2. Install New -> Maven -> Coordinates -
-> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1` -> Install 4. Now you can attach
+> `spark-nlp==5.0.2` -> Install 3.2. Install New -> Maven -> Coordinates -
+> `com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2` -> Install 4. Now you can attach
 your notebook to the cluster and use Spark NLP! NOTE: Databricks' runtimes
 support different Apache Spark major releases. Please make sure you choose the
 correct Spark NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-
 cheatsheet) ## EMR Cluster To launch EMR clusters with Apache Spark/PySpark and
 Spark NLP correctly you need to have bootstrap and software configuration. A
 sample of your bootstrap script ```.sh #!/bin/bash set -x -e echo -e 'export
@@ -351,16 +351,16 @@
 S3 (must be public access): ```.json [{ "Classification": "spark-env",
 "Configurations": [{ "Classification": "export", "Properties":
 { "PYSPARK_PYTHON": "/usr/bin/python3" } }] }, { "Classification": "spark-
 defaults", "Properties": { "spark.yarn.stagingDir": "hdfs:///tmp",
 "spark.yarn.preserve.staging.files": "true", "spark.kryoserializer.buffer.max":
 "2000M", "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
 "spark.driver.maxResultSize": "0", "spark.jars.packages":
-"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1" } }] ``` A sample of AWS CLI to
-launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 5.0.1" \
+"com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2" } }] ``` A sample of AWS CLI to
+launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 5.0.2" \
 --release-label emr-6.2.0 \ --applications Name=Hadoop Name=Spark Name=Hive \ -
 -instance-type m4.4xlarge \ --instance-count 3 \ --use-default-roles \ --log-
 uri "s3:///" \ --bootstrap-actions Path=s3:///emr-bootstrap.sh,Name=custome \ -
 -configurations "https:///sparknlp-config.json" \ --ec2-attributes
 KeyName=,EmrManagedMasterSecurityGroup=,EmrManagedSlaveSecurityGroup= \ --
 profile  ``` ## GCP Dataproc 1. Create a cluster if you don't have one already
 as follows. At gcloud shell: ```bash gcloud services enable
@@ -379,15 +379,15 @@
 boot-disk-size=128GB \ --num-workers=2 \ --bucket=${BUCKET_NAME} \ --optional-
 components=JUPYTER \ --enable-component-gateway \ --metadata
 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-
 storage' \ --initialization-actions gs://goog-dataproc-initialization-actions-$
 {REGION}/python/pip-install.sh \ --properties spark:
 spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:
 spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:
-spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` 2. On an
+spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` 2. On an
 existing one, you need to install spark-nlp and spark-nlp-display packages from
 PyPI. 3. Now, you can attach your notebook to the cluster and use the Spark
 NLP! ## Spark NLP Configuration You can change the following Spark NLP
 configurations via Spark Configuration: | Property Name | Default | Meaning |
 |--------------------------------------------------------|---------------------
 -|-----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -423,28 +423,28 @@
 configurations. ```python from pyspark.sql import SparkSession spark =
 SparkSession.builder .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config("spark.serializer",
 "org.apache.spark.serializer.KryoSerializer") .config
 ("spark.kryoserializer.buffer.max", "2000m") .config
 ("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
 .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1")
+.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2")
 .getOrCreate() ``` **spark-shell:** ```sh spark-shell \ --driver-memory 16g \ -
 -conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` **pyspark:** ```sh pyspark \ --
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` **pyspark:** ```sh pyspark \ --
 driver-memory 16g \ --conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.1 ``` **Databricks:** On a new cluster
+com.johnsnowlabs.nlp:spark-nlp_2.12:5.0.2 ``` **Databricks:** On a new cluster
 or existing one you need to add the following to the `Advanced Options -
 > Spark` tab: ```bash spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer
 spark.jsl.settings.pretrained.cache_folder dbfs:/PATH_TO_CACHE
 spark.jsl.settings.storage.cluster_tmp_dir dbfs:/PATH_TO_STORAGE
 spark.jsl.settings.annotator.log_folder dbfs:/PATH_TO_LOGS ``` NOTE: If this is
 an existing cluster, after adding new configs or changing existing properties
@@ -578,22 +578,22 @@
 pipelines or the `.pretrained()` function to download pretrained models, you
 will need to manually download your pipeline/model from [Models Hub](https://
 sparknlp.org/models), extract it, and load it. Example of `SparkSession` with
 Fat JAR to have Spark NLP offline: ```python spark = SparkSession.builder
 .appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config
 ("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars", "/tmp/spark-
-nlp-assembly-5.0.1.jar") .getOrCreate() ``` - You can download provided Fat
+nlp-assembly-5.0.2.jar") .getOrCreate() ``` - You can download provided Fat
 JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/
 releases), please pay attention to pick the one that suits your environment
 depending on the device (CPU/GPU) and Apache Spark version (3.0.x, 3.1.x,
 3.2.x, 3.3.x, and 3.4.x) - If you are local, you can load the Fat JAR from your
 local FileSystem, however, if you are in a cluster setup you need to put the
 Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. ( i.e., `hdfs:
-///tmp/spark-nlp-assembly-5.0.1.jar`) Example of using pretrained Models and
+///tmp/spark-nlp-assembly-5.0.2.jar`) Example of using pretrained Models and
 Pipelines in offline: ```python # instead of using pretrained() for online: #
 french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr") # you download
 this model, extract it, and use .load french_pos = PerceptronModel.load("/tmp/
 pos_ud_gsd_fr_2.0.2_2.4_1556531457346/") .setInputCols("document", "token")
 .setOutputCol("pos") # example for pipelines # instead of using
 PretrainedPipeline # pipeline = PretrainedPipeline('explain_document_dl',
 lang='en') # you download this pipeline, extract it, and use PipelineModel
```

### Comparing `spark-nlp-5.0.1/spark_nlp.egg-info/SOURCES.txt` & `spark-nlp-5.0.2/spark_nlp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 sparknlp/annotator/classifier_dl/roberta_for_sequence_classification.py
 sparknlp/annotator/classifier_dl/roberta_for_token_classification.py
 sparknlp/annotator/classifier_dl/sentiment_dl.py
 sparknlp/annotator/classifier_dl/tapas_for_question_answering.py
 sparknlp/annotator/classifier_dl/xlm_roberta_for_question_answering.py
 sparknlp/annotator/classifier_dl/xlm_roberta_for_sequence_classification.py
 sparknlp/annotator/classifier_dl/xlm_roberta_for_token_classification.py
+sparknlp/annotator/classifier_dl/xlm_roberta_for_zero_shot_classification.py
 sparknlp/annotator/classifier_dl/xlnet_for_sequence_classification.py
 sparknlp/annotator/classifier_dl/xlnet_for_token_classification.py
 sparknlp/annotator/coref/__init__.py
 sparknlp/annotator/coref/spanbert_coref.py
 sparknlp/annotator/cv/__init__.py
 sparknlp/annotator/cv/convnext_for_image_classification.py
 sparknlp/annotator/cv/swin_for_image_classification.py
```

### Comparing `spark-nlp-5.0.1/sparknlp/__init__.py` & `spark-nlp-5.0.2/sparknlp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     Returns
     -------
     :class:`SparkSession`
         The initiated Spark session.
 
     """
-    current_version = "5.0.1"
+    current_version = "5.0.2"
 
     if params is None:
         params = {}
     else:
         if not isinstance(params, dict):
             raise TypeError('params must be a dictionary like {"spark.executor.memory": "8G"}')
 
@@ -305,8 +305,8 @@
     """Returns the current Spark NLP version.
 
     Returns
     -------
     str
         The current Spark NLP version.
     """
-    return '5.0.1'
+    return '5.0.2'
```

### Comparing `spark-nlp-5.0.1/sparknlp/annotation.py` & `spark-nlp-5.0.2/sparknlp/annotation.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotation_audio.py` & `spark-nlp-5.0.2/sparknlp/annotation_audio.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotation_image.py` & `spark-nlp-5.0.2/sparknlp/annotation_image.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/audio/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/audio/hubert_for_ctc.py` & `spark-nlp-5.0.2/sparknlp/annotator/audio/hubert_for_ctc.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/audio/wav2vec2_for_ctc.py` & `spark-nlp-5.0.2/sparknlp/annotator/audio/wav2vec2_for_ctc.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/chunk2_doc.py` & `spark-nlp-5.0.2/sparknlp/annotator/chunk2_doc.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/chunker.py` & `spark-nlp-5.0.2/sparknlp/annotator/chunker.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,7 +42,8 @@
 from sparknlp.annotator.classifier_dl.camembert_for_token_classification import *
 from sparknlp.annotator.classifier_dl.tapas_for_question_answering import *
 from sparknlp.annotator.classifier_dl.camembert_for_sequence_classification import *
 from sparknlp.annotator.classifier_dl.camembert_for_question_answering import *
 from sparknlp.annotator.classifier_dl.bert_for_zero_shot_classification import *
 from sparknlp.annotator.classifier_dl.distil_bert_for_zero_shot_classification import *
 from sparknlp.annotator.classifier_dl.roberta_bert_for_zero_shot_classification import *
+from sparknlp.annotator.classifier_dl.xlm_roberta_for_zero_shot_classification import *
```

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/albert_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/albert_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/albert_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/albert_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/albert_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/albert_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/bert_for_zero_shot_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/bert_for_zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/camembert_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/camembert_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/camembert_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/camembert_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/camembert_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/camembert_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/classifier_dl.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/classifier_dl.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/deberta_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/deberta_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/deberta_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/deberta_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/deberta_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/deberta_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/distil_bert_for_zero_shot_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/distil_bert_for_zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/longformer_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/longformer_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/longformer_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/longformer_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/longformer_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/longformer_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/multi_classifier_dl.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/multi_classifier_dl.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_bert_for_zero_shot_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_bert_for_zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/roberta_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/roberta_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/sentiment_dl.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/sentiment_dl.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/tapas_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/tapas_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlm_roberta_for_question_answering.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlm_roberta_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlm_roberta_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlnet_for_sequence_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlnet_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/classifier_dl/xlnet_for_token_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/classifier_dl/xlnet_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/coref/spanbert_coref.py` & `spark-nlp-5.0.2/sparknlp/annotator/coref/spanbert_coref.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/cv/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/cv/convnext_for_image_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/cv/convnext_for_image_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/cv/swin_for_image_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/cv/swin_for_image_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/cv/vit_for_image_classification.py` & `spark-nlp-5.0.2/sparknlp/annotator/cv/vit_for_image_classification.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/date2_chunk.py` & `spark-nlp-5.0.2/sparknlp/annotator/date2_chunk.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/dependency/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/dependency/dependency_parser.py` & `spark-nlp-5.0.2/sparknlp/annotator/dependency/dependency_parser.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/dependency/typed_dependency_parser.py` & `spark-nlp-5.0.2/sparknlp/annotator/dependency/typed_dependency_parser.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/document_normalizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/document_normalizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/albert_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/albert_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/bert_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/bert_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/bert_sentence_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/bert_sentence_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/camembert_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/camembert_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/chunk_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/chunk_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/deberta_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/deberta_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/distil_bert_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/distil_bert_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/doc2vec.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/doc2vec.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/e5_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/e5_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/elmo_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/elmo_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/instructor_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/instructor_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/longformer_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/longformer_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/roberta_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/roberta_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/roberta_sentence_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/roberta_sentence_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/sentence_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/sentence_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/universal_sentence_encoder.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/universal_sentence_encoder.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/word2vec.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/word_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/word_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/xlm_roberta_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/xlm_roberta_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/xlm_roberta_sentence_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/xlm_roberta_sentence_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/embeddings/xlnet_embeddings.py` & `spark-nlp-5.0.2/sparknlp/annotator/embeddings/xlnet_embeddings.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/er/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/er/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/er/entity_ruler.py` & `spark-nlp-5.0.2/sparknlp/annotator/er/entity_ruler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/graph_extraction.py` & `spark-nlp-5.0.2/sparknlp/annotator/graph_extraction.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/keyword_extraction/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/keyword_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/keyword_extraction/yake_keyword_extraction.py` & `spark-nlp-5.0.2/sparknlp/annotator/keyword_extraction/yake_keyword_extraction.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ld_dl/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/ld_dl/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ld_dl/language_detector_dl.py` & `spark-nlp-5.0.2/sparknlp/annotator/ld_dl/language_detector_dl.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/lemmatizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/matcher/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/matcher/big_text_matcher.py` & `spark-nlp-5.0.2/sparknlp/annotator/matcher/big_text_matcher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/matcher/date_matcher.py` & `spark-nlp-5.0.2/sparknlp/annotator/matcher/date_matcher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/matcher/multi_date_matcher.py` & `spark-nlp-5.0.2/sparknlp/annotator/matcher/multi_date_matcher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/matcher/regex_matcher.py` & `spark-nlp-5.0.2/sparknlp/annotator/matcher/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/matcher/text_matcher.py` & `spark-nlp-5.0.2/sparknlp/annotator/matcher/text_matcher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/n_gram_generator.py` & `spark-nlp-5.0.2/sparknlp/annotator/n_gram_generator.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/ner_approach.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/ner_approach.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/ner_converter.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/ner_converter.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/ner_crf.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/ner_crf.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/ner_dl.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/ner_dl.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/ner_overwriter.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/ner_overwriter.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ner/zero_shot_ner_model.py` & `spark-nlp-5.0.2/sparknlp/annotator/ner/zero_shot_ner_model.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/normalizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/normalizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/param/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/param/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/param/classifier_encoder.py` & `spark-nlp-5.0.2/sparknlp/annotator/param/classifier_encoder.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/param/evaluation_dl_params.py` & `spark-nlp-5.0.2/sparknlp/annotator/param/evaluation_dl_params.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/pos/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/pos/perceptron.py` & `spark-nlp-5.0.2/sparknlp/annotator/pos/perceptron.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/sentence/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/sentence/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/sentence/sentence_detector.py` & `spark-nlp-5.0.2/sparknlp/annotator/sentence/sentence_detector.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/sentence/sentence_detector_dl.py` & `spark-nlp-5.0.2/sparknlp/annotator/sentence/sentence_detector_dl.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/sentiment/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/sentiment/sentiment_detector.py` & `spark-nlp-5.0.2/sparknlp/annotator/sentiment/sentiment_detector.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/sentiment/vivekn_sentiment.py` & `spark-nlp-5.0.2/sparknlp/annotator/sentiment/vivekn_sentiment.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/seq2seq/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/seq2seq/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/seq2seq/bart_transformer.py` & `spark-nlp-5.0.2/sparknlp/annotator/seq2seq/bart_transformer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/seq2seq/gpt2_transformer.py` & `spark-nlp-5.0.2/sparknlp/annotator/seq2seq/gpt2_transformer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/seq2seq/marian_transformer.py` & `spark-nlp-5.0.2/sparknlp/annotator/seq2seq/marian_transformer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/seq2seq/t5_transformer.py` & `spark-nlp-5.0.2/sparknlp/annotator/seq2seq/t5_transformer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/similarity/document_similarity_ranker.py` & `spark-nlp-5.0.2/sparknlp/annotator/similarity/document_similarity_ranker.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/spell_check/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/spell_check/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/spell_check/context_spell_checker.py` & `spark-nlp-5.0.2/sparknlp/annotator/spell_check/context_spell_checker.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/spell_check/norvig_sweeting.py` & `spark-nlp-5.0.2/sparknlp/annotator/spell_check/norvig_sweeting.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/spell_check/symmetric_delete.py` & `spark-nlp-5.0.2/sparknlp/annotator/spell_check/symmetric_delete.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/stemmer.py` & `spark-nlp-5.0.2/sparknlp/annotator/stemmer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/stop_words_cleaner.py` & `spark-nlp-5.0.2/sparknlp/annotator/stop_words_cleaner.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/tf_ner_dl_graph_builder.py` & `spark-nlp-5.0.2/sparknlp/annotator/tf_ner_dl_graph_builder.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/token/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/token/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/token/chunk_tokenizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/token/chunk_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/token/recursive_tokenizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/token/recursive_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/token/regex_tokenizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/token/regex_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/token/tokenizer.py` & `spark-nlp-5.0.2/sparknlp/annotator/token/tokenizer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ws/__init__.py` & `spark-nlp-5.0.2/sparknlp/annotator/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/annotator/ws/word_segmenter.py` & `spark-nlp-5.0.2/sparknlp/annotator/ws/word_segmenter.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/__init__.py` & `spark-nlp-5.0.2/sparknlp/base/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/audio_assembler.py` & `spark-nlp-5.0.2/sparknlp/base/audio_assembler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/doc2_chunk.py` & `spark-nlp-5.0.2/sparknlp/base/doc2_chunk.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/document_assembler.py` & `spark-nlp-5.0.2/sparknlp/base/document_assembler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/embeddings_finisher.py` & `spark-nlp-5.0.2/sparknlp/base/embeddings_finisher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/finisher.py` & `spark-nlp-5.0.2/sparknlp/base/finisher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/graph_finisher.py` & `spark-nlp-5.0.2/sparknlp/base/graph_finisher.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/has_recursive_fit.py` & `spark-nlp-5.0.2/sparknlp/base/has_recursive_fit.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/has_recursive_transform.py` & `spark-nlp-5.0.2/sparknlp/base/has_recursive_transform.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/image_assembler.py` & `spark-nlp-5.0.2/sparknlp/base/image_assembler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/light_pipeline.py` & `spark-nlp-5.0.2/sparknlp/base/light_pipeline.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/multi_document_assembler.py` & `spark-nlp-5.0.2/sparknlp/base/multi_document_assembler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/recursive_pipeline.py` & `spark-nlp-5.0.2/sparknlp/base/recursive_pipeline.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/table_assembler.py` & `spark-nlp-5.0.2/sparknlp/base/table_assembler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/token2_chunk.py` & `spark-nlp-5.0.2/sparknlp/base/token2_chunk.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/base/token_assembler.py` & `spark-nlp-5.0.2/sparknlp/base/token_assembler.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/__init__.py` & `spark-nlp-5.0.2/sparknlp/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/annotator_approach.py` & `spark-nlp-5.0.2/sparknlp/common/annotator_approach.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/annotator_model.py` & `spark-nlp-5.0.2/sparknlp/common/annotator_model.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/annotator_properties.py` & `spark-nlp-5.0.2/sparknlp/common/annotator_properties.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/annotator_type.py` & `spark-nlp-5.0.2/sparknlp/common/annotator_type.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/coverage_result.py` & `spark-nlp-5.0.2/sparknlp/common/coverage_result.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/match_strategy.py` & `spark-nlp-5.0.2/sparknlp/common/match_strategy.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/properties.py` & `spark-nlp-5.0.2/sparknlp/common/properties.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/read_as.py` & `spark-nlp-5.0.2/sparknlp/common/read_as.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/recursive_annotator_approach.py` & `spark-nlp-5.0.2/sparknlp/common/recursive_annotator_approach.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/storage.py` & `spark-nlp-5.0.2/sparknlp/common/storage.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/common/utils.py` & `spark-nlp-5.0.2/sparknlp/common/utils.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/functions.py` & `spark-nlp-5.0.2/sparknlp/functions.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/internal/__init__.py` & `spark-nlp-5.0.2/sparknlp/internal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,10 +532,16 @@
 class _RoBertaForZeroShotClassification(ExtendedJavaWrapper):
     def __init__(self, path, jspark):
         super(_RoBertaForZeroShotClassification, self).__init__(
             "com.johnsnowlabs.nlp.annotators.classifier.dl.RoBertaForZeroShotClassification.loadSavedModel", path,
             jspark)
 
 
+class _XlmRoBertaForZeroShotClassification(ExtendedJavaWrapper):
+    def __init__(self, path, jspark):
+        super(_XlmRoBertaForZeroShotClassification, self).__init__(
+            "com.johnsnowlabs.nlp.annotators.classifier.dl.XlmRoBertaForZeroShotClassification.loadSavedModel", path,
+            jspark)
+
 class _InstructorLoader(ExtendedJavaWrapper):
     def __init__(self, path, jspark):
         super(_InstructorLoader, self).__init__("com.johnsnowlabs.nlp.embeddings.InstructorEmbeddings.loadSavedModel", path, jspark)
```

### Comparing `spark-nlp-5.0.1/sparknlp/internal/annotator_java_ml.py` & `spark-nlp-5.0.2/sparknlp/internal/annotator_java_ml.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/internal/annotator_transformer.py` & `spark-nlp-5.0.2/sparknlp/internal/annotator_transformer.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/internal/extended_java_wrapper.py` & `spark-nlp-5.0.2/sparknlp/internal/extended_java_wrapper.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/internal/params_getters_setters.py` & `spark-nlp-5.0.2/sparknlp/internal/params_getters_setters.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/internal/recursive.py` & `spark-nlp-5.0.2/sparknlp/internal/recursive.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/logging/__init__.py` & `spark-nlp-5.0.2/sparknlp/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/logging/comet.py` & `spark-nlp-5.0.2/sparknlp/logging/comet.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/pretrained/__init__.py` & `spark-nlp-5.0.2/sparknlp/pretrained/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/pretrained/pretrained_pipeline.py` & `spark-nlp-5.0.2/sparknlp/pretrained/pretrained_pipeline.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/pretrained/resource_downloader.py` & `spark-nlp-5.0.2/sparknlp/pretrained/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/pretrained/utils.py` & `spark-nlp-5.0.2/sparknlp/pretrained/utils.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/__init__.py` & `spark-nlp-5.0.2/sparknlp/training/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/graph_builders.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/graph_builders.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/create_graph.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/create_graph.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/dataset_encoder.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/dataset_encoder.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/ner_model.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/ner_model.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/ner_model_saver.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/ner_model_saver.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/ner_dl/sentence_grouper.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/ner_dl/sentence_grouper.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/__init__.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/core_rnn_cell.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/core_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/fused_rnn_cell.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/fused_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/gru_ops.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/gru_ops.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/lstm_ops.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/lstm_ops.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/rnn.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/rnn.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders/tf2contrib/rnn_cell.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders/tf2contrib/rnn_cell.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/graph_builders.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/graph_builders.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/create_graph.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/create_graph.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/dataset_encoder.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/dataset_encoder.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model_saver.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model_saver.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/_tf_graph_builders_1x/ner_dl/sentence_grouper.py` & `spark-nlp-5.0.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/sentence_grouper.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/conll.py` & `spark-nlp-5.0.2/sparknlp/training/conll.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/conllu.py` & `spark-nlp-5.0.2/sparknlp/training/conllu.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/pos.py` & `spark-nlp-5.0.2/sparknlp/training/pos.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/pub_tator.py` & `spark-nlp-5.0.2/sparknlp/training/pub_tator.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/training/spacy_to_annotation.py` & `spark-nlp-5.0.2/sparknlp/training/spacy_to_annotation.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/upload_to_hub.py` & `spark-nlp-5.0.2/sparknlp/upload_to_hub.py`

 * *Files identical despite different names*

### Comparing `spark-nlp-5.0.1/sparknlp/util.py` & `spark-nlp-5.0.2/sparknlp/util.py`

 * *Files identical despite different names*

