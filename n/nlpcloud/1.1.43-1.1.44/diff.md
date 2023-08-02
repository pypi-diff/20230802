# Comparing `tmp/nlpcloud-1.1.43.tar.gz` & `tmp/nlpcloud-1.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpcloud-1.1.43.tar", last modified: Wed Jul  5 06:26:03 2023, max compression
+gzip compressed data, was "nlpcloud-1.1.44.tar", last modified: Wed Aug  2 09:03:18 2023, max compression
```

## Comparing `nlpcloud-1.1.43.tar` & `nlpcloud-1.1.44.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     1053 2021-01-19 13:02:30.000000 nlpcloud-1.1.43/LICENSE
--rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)     1109 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/PKG-INFO
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)    16934 2023-06-05 09:52:34.000000 nlpcloud-1.1.43/README.md
-drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/nlpcloud/
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)    13808 2023-06-27 09:40:51.000000 nlpcloud-1.1.43/nlpcloud/__init__.py
-drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/nlpcloud.egg-info/
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     1109 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/PKG-INFO
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)      206 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/SOURCES.txt
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        1 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/dependency_links.txt
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/requires.txt
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/top_level.txt
--rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)       38 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/setup.cfg
--rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)     1257 2023-07-05 06:25:23.000000 nlpcloud-1.1.43/setup.py
+drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-08-02 09:03:18.630973 nlpcloud-1.1.44/
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     1053 2021-01-19 13:02:30.000000 nlpcloud-1.1.44/LICENSE
+-rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)     1109 2023-08-02 09:03:18.630973 nlpcloud-1.1.44/PKG-INFO
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)    15729 2023-08-02 09:02:40.000000 nlpcloud-1.1.44/README.md
+drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-08-02 09:03:18.626973 nlpcloud-1.1.44/nlpcloud/
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)    13424 2023-08-02 09:02:02.000000 nlpcloud-1.1.44/nlpcloud/__init__.py
+drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-08-02 09:03:18.626973 nlpcloud-1.1.44/nlpcloud.egg-info/
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     1109 2023-08-02 09:03:18.000000 nlpcloud-1.1.44/nlpcloud.egg-info/PKG-INFO
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)      206 2023-08-02 09:03:18.000000 nlpcloud-1.1.44/nlpcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        1 2023-08-02 09:03:18.000000 nlpcloud-1.1.44/nlpcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2023-08-02 09:03:18.000000 nlpcloud-1.1.44/nlpcloud.egg-info/requires.txt
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2023-08-02 09:03:18.000000 nlpcloud-1.1.44/nlpcloud.egg-info/top_level.txt
+-rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)       38 2023-08-02 09:03:18.630973 nlpcloud-1.1.44/setup.cfg
+-rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)     1257 2023-08-02 09:00:52.000000 nlpcloud-1.1.44/setup.py
```

### Comparing `nlpcloud-1.1.43/LICENSE` & `nlpcloud-1.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpcloud-1.1.43/PKG-INFO` & `nlpcloud-1.1.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpcloud
-Version: 1.1.43
+Version: 1.1.44
 Summary: Python client for the NLP Cloud API
 Home-page: https://github.com/nlpcloud/nlpcloud-python
 Author: Julien Salinas
 Author-email: all@juliensalinas.com
 License: MIT
 Keywords: api,NLP,ai,deep learning,machine learning,data science,nlpcloud
 Platform: UNKNOWN
```

### Comparing `nlpcloud-1.1.43/README.md` & `nlpcloud-1.1.44/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -224,29 +224,24 @@
 The above command returns a JSON object.
 
 ### Generation Endpoint
 
 Call the `generation()` method and pass the following arguments:
 
 1. The block of text that starts the generated text. 256 tokens maximum for GPT-J on CPU, 1024 tokens maximum for GPT-J and GPT-NeoX 20B on GPU, and 2048 tokens maximum for Fast GPT-J and Finetuned GPT-NeoX 20B on GPU.
-1. (Optional) `min_length`: The minimum number of tokens that the generated text should contain. 256 tokens maximum for GPT-J on CPU, 1024 tokens maximum for GPT-J and GPT-NeoX 20B on GPU, and 2048 tokens maximum for Fast GPT-J and Finetuned GPT-NeoX 20B on GPU.. If `length_no_input` is false, the size of the generated text is the difference between `min_length` and the length of your input text. If `length_no_input` is true, the size of the generated text simply is `min_length`. Defaults to 10.
 1. (Optional) `max_length`: Optional. The maximum number of tokens that the generated text should contain. 256 tokens maximum for GPT-J on CPU, 1024 tokens maximum for GPT-J and GPT-NeoX 20B on GPU, and 2048 tokens maximum for Fast GPT-J and Finetuned GPT-NeoX 20B on GPU. If `length_no_input` is false, the size of the generated text is the difference between `max_length` and the length of your input text. If `length_no_input` is true, the size of the generated text simply is `max_length`. Defaults to 50.
 1. (Optional) `length_no_input`: Whether `min_length` and `max_length` should not include the length of the input text, as a boolean. If false, `min_length` and `max_length` include the length of the input text. If true, min_length and `max_length` don't include the length of the input text. Defaults to false.
 1. (Optional) `end_sequence`: A specific token that should be the end of the generated sequence, as a string. For example if could be `.` or `\n` or `###` or anything else below 10 characters.
 1. (Optional) `remove_input`: Whether you want to remove the input text form the result, as a boolean. Defaults to false.
-1. (Optional) `do_sample`: Whether or not to use sampling ; use greedy decoding otherwise, as a boolean. Defaults to true.
 1. (Optional) `num_beams`: Number of beams for beam search. 1 means no beam search. This is an integer. Defaults to 1.
-1. (Optional) `early_stopping`: Whether to stop the beam search when at least num_beams sentences are finished per batch or not, as a boolean. Defaults to false.
-1. (Optional) `no_repeat_ngram_size`: If set to int > 0, all ngrams of that size can only occur once. This is an integer. Defaults to 0.
 1. (Optional) `num_return_sequences`: The number of independently computed returned sequences for each element in the batch, as an integer. Defaults to 1.
 1. (Optional) `top_k`: The number of highest probability vocabulary tokens to keep for top-k-filtering, as an integer. Maximum 1000 tokens. Defaults to 0.
 1. (Optional) `top_p`: If set to float < 1, only the most probable tokens with probabilities that add up to top_p or higher are kept for generation. This is a float. Should be between 0 and 1. Defaults to 0.7.
 1. (Optional) `temperature`: The value used to module the next token probabilities, as a float. Should be between 0 and 1. Defaults to 1.
 1. (Optional) `repetition_penalty`: The parameter for repetition penalty, as a float. 1.0 means no penalty. Defaults to 1.0.
-1. (Optional) `length_penalty`: Exponential penalty to the length, as a float. 1.0 means no penalty. Set to values < 1.0 in order to encourage the model to generate shorter sequences, or to a value > 1.0 in order to encourage the model to produce longer sequences. Defaults to 1.0.
 1. (Optional) `bad_words`: List of tokens that are not allowed to be generated, as a list of strings. Defaults to null.
 1. (Optional) `remove_end_sequence`: Optional. Whether you want to remove the `end_sequence` string from the result. Defaults to false.
 
 ```python
 client.generation("<Your input text>")
 ```
```

### Comparing `nlpcloud-1.1.43/nlpcloud/__init__.py` & `nlpcloud-1.1.44/nlpcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,39 +184,33 @@
             if "<!DOCTYPE html>" in r.text:
                 raise HTTPError(str(err))
 
             raise HTTPError(str(err) + ": " + str(r.text))
 
         return r.json()
 
-    def generation(self, text, min_length=None, max_length=None, length_no_input=None,
-                   end_sequence=None, remove_input=None, do_sample=None, num_beams=None, early_stopping=None,
-                   no_repeat_ngram_size=None, num_return_sequences=None, top_k=None, top_p=None,
-                   temperature=None, repetition_penalty=None, length_penalty=None, bad_words=None, remove_end_sequence=None,
-                   is_instruct=None):
+    def generation(self, text, max_length=None, length_no_input=None,
+                   end_sequence=None, remove_input=None, num_beams=None,
+                   num_return_sequences=None, top_k=None, top_p=None,
+                   temperature=None, repetition_penalty=None, bad_words=None,
+                   remove_end_sequence=None):
         payload = {
             "text": text,
-            "min_length": min_length,
             "max_length": max_length,
             "length_no_input": length_no_input,
             "end_sequence": end_sequence,
             "remove_input": remove_input,
-            "do_sample": do_sample,
             "num_beams": num_beams,
-            "early_stopping": early_stopping,
-            "no_repeat_ngram_size": no_repeat_ngram_size,
             "num_return_sequences": num_return_sequences,
             "top_k": top_k,
             "top_p": top_p,
             "temperature": temperature,
             "repetition_penalty": repetition_penalty,
-            "length_penalty": length_penalty,
             "bad_words": bad_words,
             "remove_end_sequence": remove_end_sequence,
-            "is_instruct": is_instruct,
         }
 
         r = requests.post(
             "{}/{}".format(self.root_url, "generation"), json=payload, headers=self.headers)
 
         try:
             r.raise_for_status()
```

### Comparing `nlpcloud-1.1.43/nlpcloud.egg-info/PKG-INFO` & `nlpcloud-1.1.44/nlpcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpcloud
-Version: 1.1.43
+Version: 1.1.44
 Summary: Python client for the NLP Cloud API
 Home-page: https://github.com/nlpcloud/nlpcloud-python
 Author: Julien Salinas
 Author-email: all@juliensalinas.com
 License: MIT
 Keywords: api,NLP,ai,deep learning,machine learning,data science,nlpcloud
 Platform: UNKNOWN
```

### Comparing `nlpcloud-1.1.43/setup.py` & `nlpcloud-1.1.44/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='nlpcloud',
-    version='1.1.43',
+    version='1.1.44',
     description='Python client for the NLP Cloud API',
     long_description="NLP Cloud serves high performance pre-trained or custom models for NER, sentiment-analysis, classification, summarization, paraphrasing, grammar and spelling correction, keywords and keyphrases extraction, chatbot, product description and ad generation, intent classification, text generation, image generation, code generation, question answering, automatic speech recognition, machine translation, language detection, semantic search, semantic similarity, speech synthesis, tokenization, POS tagging, embeddings, and dependency parsing. It is ready for production, served through a REST API.\n\nThis is the Python client for the API.\n\nMore details here: https://nlpcloud.io\n\nDocumentation: https://docs.nlpcloud.io\n\nGithub: https://github.com/nlpcloud/nlpcloud-python",
     packages=['nlpcloud'],
     author='Julien Salinas',
     author_email='all@juliensalinas.com',
     license='MIT',
     keywords=['api', 'NLP', 'ai', 'deep learning', 'machine learning',
```

