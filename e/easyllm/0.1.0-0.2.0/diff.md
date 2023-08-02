# Comparing `tmp/easyllm-0.1.0.tar.gz` & `tmp/easyllm-0.2.0.tar.gz`

## Comparing `easyllm-0.1.0.tar` & `easyllm-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.1.0/makefile
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 easyllm-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/check.yaml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/documentation.yaml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/clients.md
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/installation.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/prompt_utils.md
--rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/examples/chat-completion-api.ipynb
--rw-r--r--   0        0        0    49822 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/examples/stream-chat-completions.ipynb
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/cli.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/clients/__init__.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/clients/huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/evol_instruct/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/prompt_utils/__init__.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/prompt_utils/base.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/prompt_utils/llama2.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/schema/base.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/schema/openai.py
--rw-r--r--   0        0        0    21202 2020-02-02 00:00:00.000000 easyllm-0.1.0/notebooks/chat-completion-api.ipynb
--rw-r--r--   0        0        0    49822 2020-02-02 00:00:00.000000 easyllm-0.1.0/notebooks/stream-chat-completions.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.1.0/scripts/.gitkeep
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.1.0/tests/test_main.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 easyllm-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.1.0/LICENSE
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 easyllm-0.1.0/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 easyllm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 easyllm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.2.0/makefile
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 easyllm-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/documentation.yaml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/clients.md
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/installation.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/prompt_utils.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/cli.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/clients/__init__.py
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/clients/huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/evol_instruct/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/prompt_utils/__init__.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/prompt_utils/base.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/prompt_utils/llama2.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/schema/base.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/schema/openai.py
+-rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/chat-completion-api.ipynb
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/get-embeddings.ipynb
+-rw-r--r--   0        0        0    41821 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/steam-text-completions.ipynb
+-rw-r--r--   0        0        0    49555 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/stream-chat-completions.ipynb
+-rw-r--r--   0        0        0     9013 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/text-completion-api.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.2.0/scripts/.gitkeep
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.2.0/tests/test_main.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 easyllm-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 easyllm-0.2.0/README.md
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 easyllm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 easyllm-0.2.0/PKG-INFO
```

### Comparing `easyllm-0.1.0/mkdocs.yml` & `easyllm-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/.github/workflows/check.yaml` & `easyllm-0.2.0/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/.github/workflows/documentation.yaml` & `easyllm-0.2.0/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/.github/workflows/publish.yaml` & `easyllm-0.2.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/.github/workflows/test.yaml` & `easyllm-0.2.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/docs/index.md` & `easyllm-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/docs/prompt_utils.md` & `easyllm-0.2.0/docs/prompt_utils.md`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/docs/examples/chat-completion-api.ipynb` & `easyllm-0.2.0/notebooks/chat-completion-api.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9848403495718463%*

 * *Differences: {"'cells'": "{1: {'source': ['### 1. Import the easyllm library']}, 3: {'execution_count': 6}, 5: "*

 * *            "{'execution_count': 1, 'outputs': [OrderedDict([('data', OrderedDict([('text/plain', "*

 * *            '["{\'id\': \'hf-VH-mBO0hVT\',\\n", " \'object\': \'chat.completion\',\\n", " '*

 * *            '\'created\': 1690987326,\\n", " \'model\': \'meta-llama/Llama-2-70b-chat-hf\',\\n", " '*

 * *            '\'choices\': [{\'index\': 0,\\n", "   \'message\': {\'role\': \'assistant\', '*

 * *            '\'content\': \ […]*

```diff
@@ -17,30 +17,30 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### 1. Import the openai library"
+                "### 1. Import the easyllm library"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# if needed, install and/or upgrade to the latest version of the OpenAI Python library\n",
                 "%pip install --upgrade easyllm "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# import the EasyLLM Python library for calling the EasyLLM API\n",
                 "import easyllm"
             ]
         },
@@ -60,41 +60,58 @@
                 "Compared to OpenAI api is the `huggingface` module also exposing a `prompt_builder` and `stop_sequences` parameter you can use to customize the prompt and stop sequences. The EasyLLM package comes with build in popular methods for both of these parameters, e.g. `llama2_prompt_builder` and `llama2_stop_sequences`. \n",
                 "\n",
                 "Let's look at an example chat API calls to see how the chat format works in practice."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'id': 'hf-VH-mBO0hVT',\n",
+                            " 'object': 'chat.completion',\n",
+                            " 'created': 1690987326,\n",
+                            " 'model': 'meta-llama/Llama-2-70b-chat-hf',\n",
+                            " 'choices': [{'index': 0,\n",
+                            "   'message': {'role': 'assistant', 'content': ' Apple who?'},\n",
+                            "   'finish_reason': 'eos_token'}],\n",
+                            " 'usage': {'prompt_tokens': 149, 'completion_tokens': 5, 'total_tokens': 154}}"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "\n",
                 "from easyllm.clients import huggingface\n",
                 "from easyllm.prompt_utils import llama2_stop_sequences, build_llama2_prompt\n",
+                "# Example EasyLLM Python library request\n",
+                "MODEL = \"meta-llama/Llama-2-70b-chat-hf\"\n",
+                "huggingface.prompt_builder = build_llama2_prompt\n",
                 "\n",
                 "# The module automatically loads the HuggingFace API key from the environment variable HUGGINGFACE_TOKEN or from the HuggingFace CLI configuration file.\n",
                 "# huggingface.api_key=\"hf_xxx\"\n",
                 "\n",
-                "MODEL = \"meta-llama/Llama-2-70b-chat-hf\"\n",
-                "huggingface.prompt_builder = build_llama2_prompt\n",
-                "\n",
                 "response = huggingface.ChatCompletion.create(\n",
                 "    model=MODEL,\n",
                 "    messages=[\n",
                 "        {\"role\": \"system\", \"content\": \"\\nYou are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\\n\\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information.\"},\n",
                 "        {\"role\": \"user\", \"content\": \"Knock knock.\"},\n",
                 "        {\"role\": \"assistant\", \"content\": \"Who's there?\"},\n",
-                "        {\"role\": \"user\", \"content\": \"Orange.\"},\n",
+                "        {\"role\": \"user\", \"content\": \"Apple.\"},\n",
                 "    ],\n",
                 "      temperature=0.9,\n",
                 "      top_p=0.6,\n",
                 "      max_tokens=1024,\n",
                 ")\n",
-                "\n",
                 "response"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -117,22 +134,22 @@
             "metadata": {},
             "source": [
                 "Extract just the reply with:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        " Orange who?\n"
+                        " Apple who?\n"
                     ]
                 }
             ],
             "source": [
                 "print(response['choices'][0]['message']['content'])"
             ]
         },
@@ -144,97 +161,102 @@
                 "Even non-conversation-based tasks can fit into the chat format, by placing the instruction in the first user message.\n",
                 "\n",
                 "For example, to ask the model to explain asynchronous programming in the style of the pirate Blackbeard, we can structure conversation as follows:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "07/29/2023 21:13:43 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
-                        "<s>[INST] <<SYS>>\n",
-                        "You are a helpful assistant.\n",
-                        "<</SYS>>\n",
+                        " Hello, my dear students! Today, we're going to learn about a fascinating topic that will help us understand how to make our programs more efficient and responsive: asynchronous programming.\n",
                         "\n",
-                        "Explain asynchronous programming in the style of the pirate Blackbeard. [/INST]\n",
-                        "07/29/2023 21:13:43 - DEBUG - easyllm.utils - Url:\n",
-                        "https://api-inference.huggingface.co/models/meta-llama/Llama-2-70b-chat-hf\n",
-                        "07/29/2023 21:13:43 - DEBUG - easyllm.utils - Stop sequences:\n",
-                        "[]\n",
-                        "07/29/2023 21:13:43 - DEBUG - easyllm.utils - Generation parameters:\n",
-                        "{'do_sample': True, 'return_full_text': False, 'max_new_tokens': 1024, 'top_p': 0.6, 'temperature': 0.2, 'stop_sequences': [], 'repetition_penalty': 1.0, 'top_k': 10, 'seed': 42}\n",
-                        "07/29/2023 21:13:43 - DEBUG - easyllm.utils - Response at index 0:\n",
-                        "index=0 message=ChatMessage(role='assistant', content=' Ahoy matey! Ol\\' Blackbeard here be explainin\\' asynchronous programming, arrr!\\n\\nAsynchronous programming be like sailin\\' a ship, ye see. Ye got yer crew, and each member be doin\\' their own task, like hoistin\\' the sails, swabbin\\' the deck, or mannin\\' the cannons. But, ye don\\'t be tellin\\' them what to do, they be doin\\' it on their own, in their own time, savvy?\\n\\nNow, imagine ye be the captain, and ye want to make sure the ship be sailin\\' smoothly. Ye give orders, but ye don\\'t be tellin\\' each crew member exactly when to do their task. Instead, ye be sayin\\', \"Alright me hearties, we need to hoist the sails, swab the deck, and man the cannons, but ye can do it in yer own time, just make sure it be done before we reach the next port!\"\\n\\nThat be asynchronous programming, me hearty! Ye be tellin\\' the crew what needs to be done, but not when to do it. They be figure out the best time to do their task, and they be doin\\' it on their own, without ye tellin\\' \\'em what to do every step o\\' the way.\\n\\nBut, arrr, there be a catch, me matey! If ye not careful, the crew might be doin\\' their tasks at the wrong time, and the ship might not sail smoothly. That be why ye need to be careful when ye be writin\\' yer code, and make sure that each task be done in the right order, and that they be done before the next task can be started.\\n\\nSo, hoist the sails, me hearties, and set sail fer asynchronous programming! It be a powerful tool, but ye need to use it wisely, or ye might find yerself walkin\\' the plank! Arrr!') finish_reason=None\n",
-                        " Ahoy matey! Ol' Blackbeard here be explainin' asynchronous programming, arrr!\n",
+                        "Imagine you're working on a project with your classmates, and you need to finish a task, but you're waiting for someone else to finish their part first. You can't start your work until they're done, but you don't want to just sit there twiddling your thumbs. That's where asynchronous programming comes in!\n",
+                        "\n",
+                        "Asynchronous programming is like working on a project with your classmates, but instead of waiting for them to finish, you can start working on something else in the meantime. You can think of it like this:\n",
+                        "\n",
+                        "1. You give a task to your classmate, and they start working on it.\n",
+                        "2. While they're working, you start working on another task that doesn't depend on their work.\n",
+                        "3. When your classmate finishes their task, they give it back to you, and you can continue working on your task.\n",
                         "\n",
-                        "Asynchronous programming be like sailin' a ship, ye see. Ye got yer crew, and each member be doin' their own task, like hoistin' the sails, swabbin' the deck, or mannin' the cannons. But, ye don't be tellin' them what to do, they be doin' it on their own, in their own time, savvy?\n",
+                        "This way, you can work on multiple tasks simultaneously, and you don't have to wait for each other to finish before moving on to the next step. It's like having multiple people working on a project at the same time, but they're all working on different parts of it.\n",
                         "\n",
-                        "Now, imagine ye be the captain, and ye want to make sure the ship be sailin' smoothly. Ye give orders, but ye don't be tellin' each crew member exactly when to do their task. Instead, ye be sayin', \"Alright me hearties, we need to hoist the sails, swab the deck, and man the cannons, but ye can do it in yer own time, just make sure it be done before we reach the next port!\"\n",
+                        "Now, let's see how this works in programming. Imagine you're building a website, and you want to load some data from an API. You can't start building the website until the data is loaded, but you don't want to wait for the data to be loaded before you start building the website. That's where asynchronous programming comes in!\n",
                         "\n",
-                        "That be asynchronous programming, me hearty! Ye be tellin' the crew what needs to be done, but not when to do it. They be figure out the best time to do their task, and they be doin' it on their own, without ye tellin' 'em what to do every step o' the way.\n",
+                        "You can use a special function called a \"callback\" to handle this situation. A callback is like a homework assignment that you give to a classmate. You give them the assignment, and they work on it. When they're done, they give it back to you, and you can continue working on your project.\n",
                         "\n",
-                        "But, arrr, there be a catch, me matey! If ye not careful, the crew might be doin' their tasks at the wrong time, and the ship might not sail smoothly. That be why ye need to be careful when ye be writin' yer code, and make sure that each task be done in the right order, and that they be done before the next task can be started.\n",
+                        "Here's an example of how this might look in code:\n",
+                        "```\n",
+                        "// Give the homework assignment (callback) to the API\n",
+                        "fetchDataFromApi(callback);\n",
                         "\n",
-                        "So, hoist the sails, me hearties, and set sail fer asynchronous programming! It be a powerful tool, but ye need to use it wisely, or ye might find yerself walkin' the plank! Arrr!\n"
+                        "// Start working on the website while waiting for the data to be loaded\n",
+                        "buildWebsite();\n",
+                        "\n",
+                        "// When the data is loaded, continue working on the website\n",
+                        "function callback(data) {\n",
+                        "  // Use the data to finish building the website\n",
+                        "  buildWebsiteWithData(data);\n",
+                        "}\n",
+                        "```\n",
+                        "Asynchronous programming can be a bit tricky to wrap your head around at first, but once you understand the concept, it's a powerful tool for building efficient and responsive programs. So, keep practicing, and soon you'll be a master of asynchronous programming!\n"
                     ]
                 }
             ],
             "source": [
                 "# example with a system message\n",
                 "response = huggingface.ChatCompletion.create(\n",
                 "    model=MODEL,\n",
                 "    messages=[\n",
                 "        {\"role\": \"system\", \"content\": \"You are a helpful assistant.\"},\n",
-                "        {\"role\": \"user\", \"content\": \"Explain asynchronous programming in the style of the pirate Blackbeard.\"},\n",
+                "        {\"role\": \"user\", \"content\": \"Explain asynchronous programming in the style of math teacher.\"},\n",
                 "    ],\n",
-                "    temperature=0.2,\n",
                 ")\n",
                 "\n",
                 "print(response['choices'][0]['message']['content'])\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "07/29/2023 21:11:56 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
+                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
                         "<s>[INST] Explain asynchronous programming in the style of the pirate Blackbeard. [/INST]\n",
-                        "07/29/2023 21:11:56 - DEBUG - easyllm.utils - Url:\n",
+                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Url:\n",
                         "https://api-inference.huggingface.co/models/meta-llama/Llama-2-70b-chat-hf\n",
-                        "07/29/2023 21:11:56 - DEBUG - easyllm.utils - Stop sequences:\n",
+                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Stop sequences:\n",
                         "[]\n",
-                        "07/29/2023 21:11:56 - DEBUG - easyllm.utils - Generation parameters:\n",
+                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Generation parameters:\n",
                         "{'do_sample': True, 'return_full_text': False, 'max_new_tokens': 1024, 'top_p': 0.6, 'temperature': 0.9, 'stop_sequences': [], 'repetition_penalty': 1.0, 'top_k': 10, 'seed': 42}\n",
-                        "07/29/2023 21:11:56 - DEBUG - easyllm.utils - Response at index 0:\n",
-                        "index=0 message=ChatMessage(role='assistant', content=' Ahoy matey! Yer lookin\\' fer a tale of asynchronous programming, eh? Well, settle yerself down with a pint o\\' grog and listen close, for Blackbeard\\'s got a story fer ye.\\n\\nAsynchronous programming, me hearties, be like sailin\\' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the hidden dangers that lie beneath the surface.\\n\\nImagine ye\\'re sailin\\' along, and suddenly, out o\\' the blue, a great storm brews up. The winds howl, the waves crash, and yer ship takes on water. Now, ye gotta act fast, or ye\\'ll be sent to Davy Jones\\' locker!\\n\\nBut, me hearties, ye can\\'t just abandon ship. Ye gotta batten down the hatches, and ride out the storm. And that\\'s where asynchronous programming comes in.\\n\\nAsynchronous programming be like haulin\\' up the sails, and lettin\\' the wind do the work fer ye. Ye don\\'t have to worry about the details o\\' how the wind\\'s blowin\\', or the waves crashin\\', ye just gotta keep yer ship pointed in the right direction, and let nature take its course.\\n\\nNow, I know what ye\\'re thinkin\\', \"Blackbeard, how do I know when me ship\\'s gonna make it through the storm?\" And that, me hearties, be the beauty o\\' asynchronous programming. Ye don\\'t have to know! Ye just have to trust that the winds o\\' change will carry ye through, and ye\\'ll make it to the other side, all in one piece.\\n\\nBut, me hearties, don\\'t ye be thinkin\\' this be easy. Asynchronous programming be like navigatin\\' through treacherous waters, with a crew o\\' mutinous code, and a hull full o\\' bugs. Ye gotta be prepared fer the unexpected, and have a stout heart, or ye\\'ll be walkin\\' the plank!\\n\\nSo, me hearties, there ye have it. Asynchronous programming in the style o\\' Blackbeard. May the winds o\\' change blow in yer favor, and may yer code always be free o\\' bugs! Arrr!') finish_reason=None\n",
+                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Response at index 0:\n",
+                        "index=0 message=ChatMessage(role='assistant', content=\" Ahoy matey! Yer lookin' fer a tale of asynchronous programming, eh? Well, settle yerself down with a pint o' grog and listen close, for Blackbeard's got a story fer ye.\\n\\nAsynchronous programming, me hearty, be like sailin' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the rocks and shoals that'll sink ye ship if ye ain't careful.\\n\\nImagine ye're sailin' along, and ye need to send a message to another ship, say, to arrange a meetin' at the next port o' call. Now, ye could just shout out the message and hope the other ship hears ye, but that be a risky business. The wind and the waves might carry yer words away, and the other ship might not hear ye at all.\\n\\nOr, ye could use a bit o' magic, like a bottle with a message inside, and throw it into the sea. The currents and the tides'll carry it to the other ship, and they'll find it when they least expect it. That be asynchronous programming, me hearty!\\n\\nYe see, when ye send a message, ye don't know when it'll arrive, or even if it'll arrive at all. It's like sendin' a ship's boy up the riggin' to fetch a sail that's stuck. Ye don't know when he'll get there, but ye trust that he'll do his best to fetch it down.\\n\\nAnd that's where the magic comes in, me hearty. Ye gotta have faith that the message'll get there, and that the other ship'll receive it in good time. And while ye wait, ye can keep sailin' on, doin' other tasks, like fixin' the riggin' or swabbin' the decks.\\n\\nNow, there be times when the message don't arrive at all, or it arrives too late. That be like a storm blowin' in, and ye gotta adjust yer sails to keep the ship afloat. But that's the way o' the sea, me hearty. Ye gotta be ready fer anythin', and keep yer wits about ye at all times.\\n\\nSo there ye have it, me hearty. Asynchronous programming be like sailin' the high seas, with a bit o' magic and a lot o' faith. Keep yer wits about ye, and ye'll navigate the treacherous waters like a seasoned pirate! Arrr!\") finish_reason='eos_token'\n",
                         " Ahoy matey! Yer lookin' fer a tale of asynchronous programming, eh? Well, settle yerself down with a pint o' grog and listen close, for Blackbeard's got a story fer ye.\n",
                         "\n",
-                        "Asynchronous programming, me hearties, be like sailin' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the hidden dangers that lie beneath the surface.\n",
+                        "Asynchronous programming, me hearty, be like sailin' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the rocks and shoals that'll sink ye ship if ye ain't careful.\n",
                         "\n",
-                        "Imagine ye're sailin' along, and suddenly, out o' the blue, a great storm brews up. The winds howl, the waves crash, and yer ship takes on water. Now, ye gotta act fast, or ye'll be sent to Davy Jones' locker!\n",
+                        "Imagine ye're sailin' along, and ye need to send a message to another ship, say, to arrange a meetin' at the next port o' call. Now, ye could just shout out the message and hope the other ship hears ye, but that be a risky business. The wind and the waves might carry yer words away, and the other ship might not hear ye at all.\n",
                         "\n",
-                        "But, me hearties, ye can't just abandon ship. Ye gotta batten down the hatches, and ride out the storm. And that's where asynchronous programming comes in.\n",
+                        "Or, ye could use a bit o' magic, like a bottle with a message inside, and throw it into the sea. The currents and the tides'll carry it to the other ship, and they'll find it when they least expect it. That be asynchronous programming, me hearty!\n",
                         "\n",
-                        "Asynchronous programming be like haulin' up the sails, and lettin' the wind do the work fer ye. Ye don't have to worry about the details o' how the wind's blowin', or the waves crashin', ye just gotta keep yer ship pointed in the right direction, and let nature take its course.\n",
+                        "Ye see, when ye send a message, ye don't know when it'll arrive, or even if it'll arrive at all. It's like sendin' a ship's boy up the riggin' to fetch a sail that's stuck. Ye don't know when he'll get there, but ye trust that he'll do his best to fetch it down.\n",
                         "\n",
-                        "Now, I know what ye're thinkin', \"Blackbeard, how do I know when me ship's gonna make it through the storm?\" And that, me hearties, be the beauty o' asynchronous programming. Ye don't have to know! Ye just have to trust that the winds o' change will carry ye through, and ye'll make it to the other side, all in one piece.\n",
+                        "And that's where the magic comes in, me hearty. Ye gotta have faith that the message'll get there, and that the other ship'll receive it in good time. And while ye wait, ye can keep sailin' on, doin' other tasks, like fixin' the riggin' or swabbin' the decks.\n",
                         "\n",
-                        "But, me hearties, don't ye be thinkin' this be easy. Asynchronous programming be like navigatin' through treacherous waters, with a crew o' mutinous code, and a hull full o' bugs. Ye gotta be prepared fer the unexpected, and have a stout heart, or ye'll be walkin' the plank!\n",
+                        "Now, there be times when the message don't arrive at all, or it arrives too late. That be like a storm blowin' in, and ye gotta adjust yer sails to keep the ship afloat. But that's the way o' the sea, me hearty. Ye gotta be ready fer anythin', and keep yer wits about ye at all times.\n",
                         "\n",
-                        "So, me hearties, there ye have it. Asynchronous programming in the style o' Blackbeard. May the winds o' change blow in yer favor, and may yer code always be free o' bugs! Arrr!\n"
+                        "So there ye have it, me hearty. Asynchronous programming be like sailin' the high seas, with a bit o' magic and a lot o' faith. Keep yer wits about ye, and ye'll navigate the treacherous waters like a seasoned pirate! Arrr!\n"
                     ]
                 }
             ],
             "source": [
                 "# example without a system message and debug flag on:\n",
                 "response = huggingface.ChatCompletion.create(\n",
                 "    model=MODEL,\n",
@@ -259,21 +281,35 @@
                 "One way to show the model what you want is with faked example messages.\n",
                 "\n",
                 "For example:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
+                        "<s>[INST] <<SYS>>\n",
+                        "You are a helpful, pattern-following assistant.\n",
+                        "<</SYS>>\n",
+                        "\n",
+                        "Help me translate the following corporate jargon into plain English. [/INST] Sure, I'd be happy to!</s><s>[INST] New synergies will help drive top-line growth. [/INST] Things working well together will increase revenue.</s><s>[INST] Let's circle back when we have more bandwidth to touch base on opportunities for increased leverage. [/INST] Let's talk later when we're less busy about how to do better.</s><s>[INST] This late pivot means we don't have time to boil the ocean for the client deliverable. [/INST]\n",
+                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Url:\n",
+                        "https://api-inference.huggingface.co/models/meta-llama/Llama-2-70b-chat-hf\n",
+                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Stop sequences:\n",
+                        "[]\n",
+                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Generation parameters:\n",
+                        "{'do_sample': True, 'return_full_text': False, 'max_new_tokens': 1024, 'top_p': 0.6, 'temperature': 0.9, 'stop_sequences': [], 'repetition_penalty': 1.0, 'top_k': 10, 'seed': 42}\n",
+                        "08/02/2023 16:42:59 - DEBUG - easyllm.utils - Response at index 0:\n",
+                        "index=0 message=ChatMessage(role='assistant', content=\" We've changed direction too late to do a complete job for the client.\") finish_reason='eos_token'\n",
                         " We've changed direction too late to do a complete job for the client.\n"
                     ]
                 }
             ],
             "source": [
                 "# An example of a faked few-shot conversation to prime the model into translating business jargon to simpler speech\n",
                 "response = huggingface.ChatCompletion.create(\n",
@@ -302,14 +338,19 @@
                 "\n",
                 "If your first attempts fail, don't be afraid to experiment with different ways of priming or conditioning the model.\n",
                 "\n",
                 "As an example, one developer discovered an increase in accuracy when they inserted a user message that said \"Great job so far, these have been perfect\" to help condition the model into providing higher quality responses.\n",
                 "\n",
                 "For more ideas on how to lift the reliability of the models, consider reading our guide on [techniques to increase reliability](../techniques_to_improve_reliability.md). It was written for non-chat models, but many of its principles still apply."
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "openai",
             "language": "python",
             "name": "python3"
```

### Comparing `easyllm-0.1.0/docs/examples/stream-chat-completions.ipynb` & `easyllm-0.2.0/notebooks/stream-chat-completions.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997169384057971%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(12, 'Note that using `stream=True` in a production "*

 * *            'application makes it more difficult to moderate the content of the completions, as '*

 * *            "partial completions may be more difficult to evaluate. \\n')], delete: [14, 13, 12, "*

 * *            '11]}}}'}*

```diff
@@ -13,18 +13,15 @@
                 "\n",
                 "To get responses sooner, you can 'stream' the completion as it's being generated. This allows you to start printing or processing the beginning of the completion before the full completion is finished.\n",
                 "\n",
                 "To stream completions, set `stream=True` when calling the chat completions or completions endpoints. This will return an object that streams back the response as [data-only server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format). Extract chunks from the `delta` field rather than the `message` field.\n",
                 "\n",
                 "## Downsides\n",
                 "\n",
-                "Note that using `stream=True` in a production application makes it more difficult to moderate the content of the completions, as partial completions may be more difficult to evaluate. which has implications for [approved usage](https://beta.openai.com/docs/usage-guidelines).\n",
-                "\n",
-                "Another small drawback of streaming responses is that the response no longer includes the `usage` field to tell you how many tokens were consumed.\n",
-                "\n",
+                "Note that using `stream=True` in a production application makes it more difficult to moderate the content of the completions, as partial completions may be more difficult to evaluate. \n",
                 "## Example code\n",
                 "\n",
                 "Below, this notebook shows:\n",
                 "1. What a typical chat completion response looks like\n",
                 "2. What a streaming chat completion response looks like\n",
                 "3. How much time is saved by streaming a chat completion"
             ]
```

### Comparing `easyllm-0.1.0/easyllm/utils.py` & `easyllm-0.2.0/easyllm/utils.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/easyllm/prompt_utils/base.py` & `easyllm-0.2.0/easyllm/prompt_utils/base.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/easyllm/prompt_utils/llama2.py` & `easyllm-0.2.0/easyllm/prompt_utils/llama2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import List
+from typing import List, Union
 
 from easyllm.schema.base import ChatMessage
 
 llama2_stop_sequences = ["</s>"]
 
 
-def build_llama2_prompt(messages: List[ChatMessage]) -> str:
+def build_llama2_prompt(messages: Union[List[ChatMessage], str]) -> str:
     """
     Uses LLama 2 chat tokens (`[INST]`) to create a prompt, learn more in the [Hugging Face Blog on how to prompt Llama 2](https://huggingface.co/blog/llama2#how-to-prompt-llama-2). If a `Message` with an unsupported `role` is passed, an error will be thrown.
     Args:
         messages (:obj:`List[ChatMessage]`): The messages to use for the completion.
     """
 
     startPrompt = "<s>[INST] "
     endPrompt = " [/INST]"
     conversation = []
 
+    if isinstance(messages, str):
+        messages = [ChatMessage(content=messages, role="user")]
+
     for index, message in enumerate(messages):
         if message.role == "user":
             conversation.append(message.content.strip())
         elif message.role == "assistant":
             conversation.append(f" [/INST] {message.content}</s><s>[INST] ")
         elif message.role == "function":
             raise ValueError("Llama 2 does not support function calls.")
```

### Comparing `easyllm-0.1.0/easyllm/schema/openai.py` & `easyllm-0.2.0/easyllm/schema/openai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from typing import Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
 from nanoid import generate
 from pydantic import BaseModel, Field
 
 from easyllm.schema.base import ChatMessage, Usage
 
 
@@ -19,44 +19,107 @@
     max_tokens: Optional[int] = 1024
     stop: Optional[List[str]] = None
     stream: Optional[bool] = False
     frequency_penalty: Optional[float] = 1.0
     user: Optional[str] = None
 
 
-# adapted from https://github.com/lm-sys/FastChat/blob/main/fastchat/protocol/openai_api_protocol.py
 class ChatCompletionResponseChoice(BaseModel):
     index: int
     message: ChatMessage
-    finish_reason: Optional[Literal["stop", "length"]] = None
+    finish_reason: Optional[Literal["stop_sequence", "length", "eos_token"]] = None
 
 
-# adapted from https://github.com/lm-sys/FastChat/blob/main/fastchat/protocol/openai_api_protocol.py
 class ChatCompletionResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
     object: str = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
     choices: List[ChatCompletionResponseChoice]
     usage: Usage
 
 
-# adapted from https://github.com/lm-sys/FastChat/blob/main/fastchat/protocol/openai_api_protocol.py
 class DeltaMessage(BaseModel):
     role: Optional[str] = None
     content: Optional[str] = None
 
 
-# adapted from https://github.com/lm-sys/FastChat/blob/main/fastchat/protocol/openai_api_protocol.py
 class ChatCompletionResponseStreamChoice(BaseModel):
     index: int
     delta: Union[DeltaMessage, Dict[str, str]]
     finish_reason: Optional[Literal["stop", "length"]] = None
 
 
-# adapted from https://github.com/lm-sys/FastChat/blob/main/fastchat/protocol/openai_api_protocol.py
 class ChatCompletionStreamResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
     object: str = "chat.completion.chunk"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
     choices: List[ChatCompletionResponseStreamChoice]
+
+
+class CompletionRequest(BaseModel):
+    model: str
+    prompt: Union[str, List[Any]]
+    suffix: Optional[str] = None
+    temperature: Optional[float] = 0.9
+    top_p: Optional[float] = 0.6
+    top_k: Optional[int] = 10
+    n: Optional[int] = 1
+    max_tokens: Optional[int] = 1024
+    stop: Optional[List[str]] = None
+    stream: Optional[bool] = False
+    frequency_penalty: Optional[float] = 1.0
+    user: Optional[str] = None
+    logprobs: Optional[bool] = None
+    echo: Optional[bool] = False
+    user: Optional[str] = None
+
+
+class CompletionResponseChoice(BaseModel):
+    index: int
+    text: str
+    logprobs: Union[Optional[List[Dict[str, Any]]], float] = None
+    finish_reason: Optional[Literal["stop_sequence", "length", "eos_token"]] = None
+
+
+class CompletionResponse(BaseModel):
+    id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
+    object: str = "text.completion"
+    created: int = Field(default_factory=lambda: int(time.time()))
+    model: str
+    choices: List[CompletionResponseChoice]
+    usage: Usage
+
+
+class CompletionResponseStreamChoice(BaseModel):
+    index: int
+    text: str
+    logprobs: Optional[float] = None
+    finish_reason: Optional[Literal["stop_sequence", "length", "eos_token"]] = None
+
+
+class CompletionStreamResponse(BaseModel):
+    id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
+    object: str = "text.completion"
+    created: int = Field(default_factory=lambda: int(time.time()))
+    model: str
+    choices: List[CompletionResponseStreamChoice]
+
+
+class EmbeddingsRequest(BaseModel):
+    model: Optional[str] = None
+    input: Union[str, List[Any]]
+    user: Optional[str] = None
+
+
+class EmbeddingsObjectResponse(BaseModel):
+    index: int
+    object: str = "embedding"
+    embedding: List[float]
+
+
+class EmbeddingsResponse(BaseModel):
+    object: str = "list"
+    data: List[EmbeddingsObjectResponse]
+    model: str
+    usage: Usage
```

### Comparing `easyllm-0.1.0/.gitignore` & `easyllm-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/LICENSE` & `easyllm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyllm-0.1.0/README.md` & `easyllm-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # EasyLLM - 
 
-EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. 
+EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. Get immediataly started or check out the [documentation](https://philschmid.github.io/easyllm/).
 
-EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion` with, for example, `huggingface.ChatCompletion`.
+EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion`, `openai.Completion` with, for example, `huggingface.ChatCompletion` or `huggingface.Completion`.
 
 ## 🚀 Getting Started
 
 Install EasyLLM via pip:
 
 ```bash
 pip install easyllm
@@ -59,17 +59,19 @@
     "total_tokens": 410
   }
 }
 ```
 
 Check out other examples:
 * [Detailed ChatCompletion Example](examples/chat-completion-api)
-* [Example how to stream requests](examples/stream-chat-completion-api)
+* [Example how to stream chat requests](examples/stream-chat-completion-api)
+* [Example how to stream text requests](examples/stream-text-completion-api)
+* [Detailed Completion Example](examples/text-completion-api)
 
-See the [documentation](docs/README.md) for more detailed usage and examples.
+See the [documentation](https://philschmid.github.io/easyllm/) for more detailed usage and examples.
 
 ## 💪🏻 Migration from OpenAI to HuggingFace
 
 Migrating from OpenAI to HuggingFace is easy. Just change the import statement and the client you want to use and optionally the prompt builder.
 
 ```diff
 -import openai
@@ -90,15 +92,15 @@
 
 Make sure when you switch your client that your hyperparameters are still valid. For example, `temperature` of GPT-3 might be different than `temperature` of `Llama-2`.
 
 ## ☑️ Key Features
 
 ### 🤝 Compatible Clients
 
-- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`.
+- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`, `openai.Completion`.
 - Easily switch between different LLMs like `openai.ChatCompletion` and `huggingface.ChatCompletion` by changing one line of code. 
 - Support for streaming of completions, checkout example [How to stream completions](./notebooks/stream-chat-completions.ipynb).
 
 ### ⚙️ Helper Modules ⚙️
 
 - `evol_instruct` (work in progress) - Use evolutionary algorithms create instructions for LLMs.
 
@@ -114,8 +116,8 @@
 author = {Philipp Schmid},
 license = {Apache-2.0},
 month = juj,
 title = {EasyLLM: Streamlined Tools for LLMs},
 url = {https://github.com/philschmid/easyllm},
 year = {2023}
 }
-```
+```
```

### Comparing `easyllm-0.1.0/pyproject.toml` & `easyllm-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 authors = [{ name = "Philipp Schmid", email = "schmidphilipp1995@gmail.com" }]
 classifiers = [
   "Topic :: Internet",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development",
-  "Framework :: FastAPI",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
 scripts = { easyllm = "easyllm.cli:main" }
 dependencies = ["pydantic==2.1.1", "nanoid==2.0.0", "huggingface-hub==0.16.4"]
```

### Comparing `easyllm-0.1.0/PKG-INFO` & `easyllm-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: easyllm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Description
 Project-URL: Documentation, https://github.com/unknown/hatch-demo#readme
 Project-URL: Issues, https://github.com/unknown/hatch-demo/issues
 Project-URL: Source, https://github.com/unknown/hatch-demo
 Author-email: Philipp Schmid <schmidphilipp1995@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
-Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -43,17 +43,17 @@
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 # EasyLLM - 
 
-EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. 
+EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. Get immediataly started or check out the [documentation](https://philschmid.github.io/easyllm/).
 
-EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion` with, for example, `huggingface.ChatCompletion`.
+EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion`, `openai.Completion` with, for example, `huggingface.ChatCompletion` or `huggingface.Completion`.
 
 ## 🚀 Getting Started
 
 Install EasyLLM via pip:
 
 ```bash
 pip install easyllm
@@ -106,17 +106,19 @@
     "total_tokens": 410
   }
 }
 ```
 
 Check out other examples:
 * [Detailed ChatCompletion Example](examples/chat-completion-api)
-* [Example how to stream requests](examples/stream-chat-completion-api)
+* [Example how to stream chat requests](examples/stream-chat-completion-api)
+* [Example how to stream text requests](examples/stream-text-completion-api)
+* [Detailed Completion Example](examples/text-completion-api)
 
-See the [documentation](docs/README.md) for more detailed usage and examples.
+See the [documentation](https://philschmid.github.io/easyllm/) for more detailed usage and examples.
 
 ## 💪🏻 Migration from OpenAI to HuggingFace
 
 Migrating from OpenAI to HuggingFace is easy. Just change the import statement and the client you want to use and optionally the prompt builder.
 
 ```diff
 -import openai
@@ -137,15 +139,15 @@
 
 Make sure when you switch your client that your hyperparameters are still valid. For example, `temperature` of GPT-3 might be different than `temperature` of `Llama-2`.
 
 ## ☑️ Key Features
 
 ### 🤝 Compatible Clients
 
-- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`.
+- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`, `openai.Completion`.
 - Easily switch between different LLMs like `openai.ChatCompletion` and `huggingface.ChatCompletion` by changing one line of code. 
 - Support for streaming of completions, checkout example [How to stream completions](./notebooks/stream-chat-completions.ipynb).
 
 ### ⚙️ Helper Modules ⚙️
 
 - `evol_instruct` (work in progress) - Use evolutionary algorithms create instructions for LLMs.
 
@@ -161,8 +163,8 @@
 author = {Philipp Schmid},
 license = {Apache-2.0},
 month = juj,
 title = {EasyLLM: Streamlined Tools for LLMs},
 url = {https://github.com/philschmid/easyllm},
 year = {2023}
 }
-```
+```
```

