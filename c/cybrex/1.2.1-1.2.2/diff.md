# Comparing `tmp/cybrex-1.2.1.tar.gz` & `tmp/cybrex-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.2.1.tar", last modified: Wed Aug  2 13:49:20 2023, max compression
+gzip compressed data, was "cybrex-1.2.2.tar", last modified: Wed Aug  2 15:02:37 2023, max compression
```

## Comparing `cybrex-1.2.1.tar` & `cybrex-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 13:49:20.473761 cybrex-1.2.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 13:49:20.473211 cybrex-1.2.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.1/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 13:49:20.465872 cybrex-1.2.1/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.1/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5682 2023-08-02 10:33:10.000000 cybrex-1.2.1/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    12036 2023-08-02 13:48:53.000000 cybrex-1.2.1/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13577 2023-08-02 11:14:42.000000 cybrex-1.2.1/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 13:49:20.472366 cybrex-1.2.1/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-02 13:48:57.000000 cybrex-1.2.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-02 13:49:20.473949 cybrex-1.2.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 15:02:37.327445 cybrex-1.2.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 15:02:37.326851 cybrex-1.2.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.2/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 15:02:37.322362 cybrex-1.2.2/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.2/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5682 2023-08-02 10:33:10.000000 cybrex-1.2.2/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    12869 2023-08-02 15:02:09.000000 cybrex-1.2.2/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13592 2023-08-02 15:01:57.000000 cybrex-1.2.2/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 15:02:37.326293 cybrex-1.2.2/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-02 15:02:21.000000 cybrex-1.2.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-02 15:02:37.327668 cybrex-1.2.2/setup.cfg
```

### Comparing `cybrex-1.2.1/PKG-INFO` & `cybrex-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.1
+Version: 1.2.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.1/README.md` & `cybrex-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.1/cybrex/cli.py` & `cybrex-1.2.2/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.1/cybrex/cybrex_ai.py` & `cybrex-1.2.2/cybrex/cybrex_ai.py`

 * *Files 7% similar despite different names*

```diff
@@ -169,22 +169,30 @@
         return metadatas, texts
 
     async def add_full_documents(self, documents: List[dict], skip_downloading_pdf: bool = True):
         if not documents:
             return
         metadatas, texts = await self._get_missing_documents_chunks(documents, skip_downloading_pdf=skip_downloading_pdf)
         if texts:
+            logging.getLogger('statbox').info({
+                'action': 'add_full_documents',
+                'n': len(texts),
+            })
             await asyncio.get_running_loop().run_in_executor(
                 None,
                 lambda: self.collection.upsert(
                     documents=texts,
                     metadatas=metadatas,
                     ids=[str(uuid.uuid1()) for _ in range(len(texts))]
                 )
             )
+            logging.getLogger('statbox').info({
+                'action': 'added_full_documents',
+                'n': len(texts),
+            })
 
     async def add_full_document_by_field_value(self, field, value) -> List[Document]:
         documents = await self.geck.get_summa_client().search_documents([{
             'index_alias': 'nexus_science',
             'collectors': [{'top_docs': {'limit': 1}}],
             'query': {'term': {'field': field, 'value': value}}
         }])
@@ -239,32 +247,39 @@
 
     async def chat_document(self, field, value, query, n_results: int):
         await self.add_full_document_by_field_value(field, value)
 
         documents = await self._query(query, n_results, where={field: value})
         result = await asyncio.get_running_loop().run_in_executor(
             None,
-            lambda: self.model.llm.query_documents(query, documents),
+            lambda: self.model.llm.ask_documents(query, documents),
         )
 
         return result
 
     async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
         full_documents = await self.keywords_search(query, n_summa_documents)
+
         await self.add_full_documents(full_documents)
 
         documents = await self._query(query, n_results)
         answer = await asyncio.get_running_loop().run_in_executor(
             None,
-            lambda: self.model.llm.query_documents(query, documents),
+            lambda: self.model.llm.ask_documents(query, documents),
         )
 
         return answer, documents, await self.get_summa_documents_from_documents(documents)
 
     async def _query(self, query: str, n_results: int = 3, where: Optional[dict] = None):
+        logging.getLogger('statbox').info({
+            'action': 'query',
+            'query': query,
+            'n_results': n_results,
+            'where': where,
+        })
         response = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: self.collection.query(
                 query_embeddings=[self.model.embedder.embed_query(query)],
                 n_results=n_results,
                 include=['documents', 'metadatas', 'distances'],
                 where=where,
@@ -274,18 +289,29 @@
         for (text, metadata, distance) in zip(response['documents'][0], response['metadatas'][0], response['distances'][0]):
             documents.append({'text': text, 'metadata': metadata, 'distance': distance})
         return documents
 
     async def keywords_search(self, query: str, n_summa_documents: int):
         if not n_summa_documents:
             return []
-        keywords = self.model.keyword_extractor.extract_keywords(
-            query,
-            keyphrase_ngram_range=(1, 1),
+        logging.getLogger('statbox').info({
+            'action': 'extract_keywords',
+            'query': query,
+        })
+        keywords = await asyncio.get_running_loop().run_in_executor(
+            None,
+            lambda: self.model.keyword_extractor.extract_keywords(
+                query,
+                keyphrase_ngram_range=(1, 1),
+            )
         )
+        logging.getLogger('statbox').info({
+            'action': 'extracted_keywords',
+            'keywords': keywords,
+        })
         topic = ' '.join(map(lambda x: x[0], filter(lambda x: x[1] > 0.5, keywords)))
         documents = await get_documents_on_topic(
             summa_client=self.geck.get_summa_client(),
             topic=topic,
             documents=n_summa_documents,
         )
         return documents
```

### Comparing `cybrex-1.2.1/cybrex/models.py` & `cybrex-1.2.2/cybrex/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,17 @@
 FINAL ANSWER:""".format(question=question, summary=self.generate_summary(documents))
 
 class LLM:
     def __init__(self, llm, prompter):
         self.llm = llm
         self.prompter = prompter
 
-    def query_documents(self, question, documents):
+    def ask_documents(self, question, documents):
         prompt = self.prompter.qa_prompt(question, documents)
-        logging.getLogger('statbox').info({'action': 'send_prompt', 'prompt': prompt})
+        logging.getLogger('statbox').info({'action': 'ask_documents', 'mode': 'llm', 'prompt': prompt})
         return self.llm(prompt).strip()
 
 
 def get_embedding_function(model_name):
     if model_name.startswith('hkunlp/instructor'):
         return HuggingFaceInstructEmbeddings(
             model_name=model_name,
```

### Comparing `cybrex-1.2.1/cybrex.egg-info/PKG-INFO` & `cybrex-1.2.2/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.1
+Version: 1.2.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.1/pyproject.toml` & `cybrex-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.2.1"
+version = "1.2.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

