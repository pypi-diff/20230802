# Comparing `tmp/cybrex-1.1.9.tar.gz` & `tmp/cybrex-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.9.tar", last modified: Wed Aug  2 08:54:10 2023, max compression
+gzip compressed data, was "cybrex-1.2.1.tar", last modified: Wed Aug  2 13:49:20 2023, max compression
```

## Comparing `cybrex-1.1.9.tar` & `cybrex-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 08:54:10.653321 cybrex-1.1.9/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.9/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 08:54:10.652108 cybrex-1.1.9/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.9/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 08:54:10.643014 cybrex-1.1.9/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.9/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 21:12:18.000000 cybrex-1.1.9/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11975 2023-08-01 21:12:18.000000 cybrex-1.1.9/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13694 2023-08-02 08:53:55.000000 cybrex-1.1.9/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 08:54:10.650039 cybrex-1.1.9/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-02 08:53:55.000000 cybrex-1.1.9/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.9/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-02 08:54:10.653718 cybrex-1.1.9/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 13:49:20.473761 cybrex-1.2.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 13:49:20.473211 cybrex-1.2.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.1/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 13:49:20.465872 cybrex-1.2.1/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.1/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5682 2023-08-02 10:33:10.000000 cybrex-1.2.1/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    12036 2023-08-02 13:48:53.000000 cybrex-1.2.1/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13577 2023-08-02 11:14:42.000000 cybrex-1.2.1/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 13:49:20.472366 cybrex-1.2.1/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-02 13:49:20.000000 cybrex-1.2.1/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-02 13:48:57.000000 cybrex-1.2.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-02 13:49:20.473949 cybrex-1.2.1/setup.cfg
```

### Comparing `cybrex-1.1.9/PKG-INFO` & `cybrex-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.9
+Version: 1.2.1
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.9/README.md` & `cybrex-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.9/cybrex/cli.py` & `cybrex-1.2.1/cybrex/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,23 +75,23 @@
         :param n_results: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         :param n_summa_documents: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
-            response, documents = await cybrex.chat_science(
+            answer, documents, summa_documents = await cybrex.chat_science(
                 query=query,
                 n_results=n_results,
                 n_summa_documents=n_summa_documents,
             )
-            response = re.sub(r'\(DOI: ([^)]+)\)', r'(https://doi.org/\g<1>)', response)
-            documents = [f'{document["doi"]}: {document["title"]}' for document in documents]
-            sources = '\n'.join(documents)
-            print(f"{colored('A', 'green')}: {response}")
+            answer = re.sub(r'\(DOI: ([^)]+)\)', r'(https://doi.org/\g<1>)', answer)
+            summa_documents = [f'{summa_document["doi"]}: {summa_document["title"]}' for summa_document in summa_documents]
+            sources = '\n'.join(summa_documents)
+            print(f"{colored('A', 'green')}: {answer}")
             print(f"{colored('References', 'green')}:\n{textwrap.indent(sources, ' - ')}")
 
     async def sum_doc(self, field: str, value: str):
         """
         Summarization of the document
 
         :param field: name of the field in document used for selection
```

### Comparing `cybrex-1.1.9/cybrex/cybrex_ai.py` & `cybrex-1.2.1/cybrex/cybrex_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,18 +169,21 @@
         return metadatas, texts
 
     async def add_full_documents(self, documents: List[dict], skip_downloading_pdf: bool = True):
         if not documents:
             return
         metadatas, texts = await self._get_missing_documents_chunks(documents, skip_downloading_pdf=skip_downloading_pdf)
         if texts:
-            self.collection.upsert(
-                documents=texts,
-                metadatas=metadatas,
-                ids=[str(uuid.uuid1()) for _ in range(len(texts))]
+            await asyncio.get_running_loop().run_in_executor(
+                None,
+                lambda: self.collection.upsert(
+                    documents=texts,
+                    metadatas=metadatas,
+                    ids=[str(uuid.uuid1()) for _ in range(len(texts))]
+                )
             )
 
     async def add_full_document_by_field_value(self, field, value) -> List[Document]:
         documents = await self.geck.get_summa_client().search_documents([{
             'index_alias': 'nexus_science',
             'collectors': [{'top_docs': {'limit': 1}}],
             'query': {'term': {'field': field, 'value': value}}
@@ -246,19 +249,20 @@
         return result
 
     async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
         full_documents = await self.keywords_search(query, n_summa_documents)
         await self.add_full_documents(full_documents)
 
         documents = await self._query(query, n_results)
-        result = await asyncio.get_running_loop().run_in_executor(
+        answer = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: self.model.llm.query_documents(query, documents),
         )
-        return result, await self.get_summa_documents_from_documents(documents)
+
+        return answer, documents, await self.get_summa_documents_from_documents(documents)
 
     async def _query(self, query: str, n_results: int = 3, where: Optional[dict] = None):
         response = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: self.collection.query(
                 query_embeddings=[self.model.embedder.embed_query(query)],
                 n_results=n_results,
@@ -300,15 +304,14 @@
         for summa_document in _summa_documents:
             summa_documents.append(summa_document[0])
         return summa_documents
 
     async def semantic_search(self, query: str, n_results: int = 10, n_summa_documents: int = 30):
         full_documents = await self.keywords_search(query, n_summa_documents)
         await self.add_full_documents(full_documents)
-        documents = await self._query(query, n_results)
-        return await self.get_summa_documents_from_documents(documents)
+        return await self._query(query, n_results)
 
     async def summarize_document(self, field, value):
         documents = await self.add_full_document_by_field_value(field, value)
         chain = load_summarize_chain(llm=self.model.llm, chain_type="map_reduce")
         result = chain.run(documents)
         return result.strip()
```

### Comparing `cybrex-1.1.9/cybrex/models.py` & `cybrex-1.2.1/cybrex/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 from collections import OrderedDict
 from typing import List
 
 from ctransformers import AutoModelForCausalLM
 from keybert import KeyBERT
 from langchain import OpenAI
 from langchain.embeddings import HuggingFaceInstructEmbeddings, OpenAIEmbeddings
@@ -206,18 +205,15 @@
         else:
             raise ValueError("Unsupported embedding model")
 
     @lazy
     def llm(self):
         if self.config['llm']['model_type'] == 'llama':
             return LLM(
-                llm=AutoModelForCausalLM.from_pretrained(
-                    **self.config['llm']['config'],
-                    cache_dir=os.environ.get('TRANSFORMERS_CACHE'),
-                ),
+                llm=AutoModelForCausalLM.from_pretrained(**self.config['llm']['config']),
                 prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type'])
             )
         elif self.config['llm']['model_type'] == 'openai':
             return LLM(
                 llm=OpenAI(**self.config['llm']['config']),
                 prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type']),
             )
```

### Comparing `cybrex-1.1.9/cybrex.egg-info/PKG-INFO` & `cybrex-1.2.1/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.9
+Version: 1.2.1
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.9/pyproject.toml` & `cybrex-1.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.9"
+version = "1.2.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

