# Comparing `tmp/fastllm-0.1.4.tar.gz` & `tmp/fastllm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastllm-0.1.4.tar", max compression
+gzip compressed data, was "fastllm-0.1.5.tar", max compression
```

## Comparing `fastllm-0.1.4.tar` & `fastllm-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-07-16 18:54:36.878631 fastllm-0.1.4/LICENSE
--rw-r--r--   0        0        0     5353 2023-07-30 20:01:21.676030 fastllm-0.1.4/README.md
--rw-r--r--   0        0        0      137 2023-07-23 15:51:19.906944 fastllm-0.1.4/fastllm/__init__.py
--rw-r--r--   0        0        0    22275 2023-07-30 20:05:18.654169 fastllm-0.1.4/fastllm/base.py
--rw-r--r--   0        0        0     1173 2023-07-30 20:00:28.975555 fastllm-0.1.4/fastllm/utils.py
--rw-r--r--   0        0        0     1577 2023-07-30 20:01:57.104350 fastllm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 fastllm-0.1.4/setup.py
--rw-r--r--   0        0        0     6470 1970-01-01 00:00:00.000000 fastllm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 18:01:27.056723 fastllm-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6517 2023-08-02 19:08:08.771877 fastllm-0.1.5/README.md
+-rw-r--r--   0        0        0      137 2023-07-24 18:01:27.056723 fastllm-0.1.5/fastllm/__init__.py
+-rw-r--r--   0        0        0    22384 2023-08-02 19:08:03.641878 fastllm-0.1.5/fastllm/base.py
+-rw-r--r--   0        0        0     1275 2023-08-02 19:07:58.561880 fastllm-0.1.5/fastllm/utils.py
+-rw-r--r--   0        0        0     1577 2023-08-02 19:08:53.601862 fastllm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7484 1970-01-01 00:00:00.000000 fastllm-0.1.5/PKG-INFO
```

### Comparing `fastllm-0.1.4/LICENSE` & `fastllm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastllm-0.1.4/README.md` & `fastllm-0.1.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -100,59 +100,107 @@
 print(another_result)
 ```
 
 ```bash
 38
 ```
 
-#### Avoid and Prefer
+#### Avoid words/phrases 
 
-Guide completion by prefer or avoid certain words or phrases. Supports regex patterns. For avoiding/banning words typically it is advised to put a [blank space](https://community.openai.com/t/reproducible-gpt-3-5-turbo-logit-bias-100-not-functioning/88293/8) in front of the word.
+Avoid/ban word and phrases - supports patterns. Patterns follow regex syntax but do not support all features. If the number of possible strings matching the pattern is too large, the pattern is ignored. 
+
+For avoiding/banning words typically it is advised to put a [blank space](https://community.openai.com/t/reproducible-gpt-3-5-turbo-logit-bias-100-not-functioning/88293/8) in front of the word.
 
 ```python
 cat = Agent(
     Prompt("Say Cat!"),
 )
 
 print(cat())
 ```
 
 ```bash
 Cat!
 ```
 
+No we avoid/ban the regex pattern `r"[ ]?Cat"` (e.g. " Cat" or "Cat") from the response.
+
 ```python
 not_cat = Agent(
     Prompt("Say Cat!", avoid=r"[ ]?Cat"),
 )
 
 print(not_cat())
 ```
 
-OpenAI is making fun of us (that really happened!) and writes "Cat" with a lower case "c". 
+OpenAI is making fun of us (that really happened!) - obviously we need to be more specific (e.g. ban lowercase and uppercase)
 
 ```bash
 Dog! Just kidding, cat!
 ```
 
 Ok let's try again.
 
 ```python
 seriously_not_a_cat = Agent(
     Prompt("Say Cat!, PLEEASSEE", avoid=r"[ ]?[Cc][aA][tT]]"),
 )
+
+print(seriously_not_a_cat())
 ```
 
 Well no cat but kudos for the effort.
 
 ```bash
 Sure, here you go: "Meow! "
 ```
 
+#### Prefer words/phrases
+
+Prefer words/phrases - supports patterns. Patterns follow regex syntax but do not support all features. Only supports pattern matching a limited number of strings. The max token length is set to the longest possible string in the pattern. Also the order of token can not be guaranteed. 
+
+```python
+meow = Agent(
+    Prompt("Say Hi!", prefer="Meow!"),
+)
+
+print(meow())
+```
+
+```bash
+Meow!
+```
+
+```python
+austria_wins = Agent(
+    Prompt("Predict the score for Austria against Germany.", prefer=r"Austria: [3-4], Germany: [0-1]"),
+)
 
+print(austria_wins())
+```
+
+Order of tokens is not guaranteed (and this is obviously false ;))
+
+```bash
+Austria, 1: Germany, 3
+```
+
+```python
+meow = Agent(
+    Prompt("Say Hi!", prefer="Meow!", max_tokens=10),
+)
+
+print(meow())
+```
+
+Our model can only say "Meow" or "!" up to 10 tokens.
+
+```bash
+Meow!!!!Meow!Meow!Meow!Meow!Meow
+```
 
 ## Roadmap
 
 ### Features
 
 - [x] Prompts using jinja2 templates
 - [x] LLM calling with backoff and retry
```

### Comparing `fastllm-0.1.4/fastllm/base.py` & `fastllm-0.1.5/fastllm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,19 +617,22 @@
     ) -> Generator[dict, None, None]:
         """Calls the model, retries on RateLimitError."""
 
         name = kwargs.pop("name", self.name)
         logit_bias = kwargs.get("logit_bias", {})
 
         if prefer:
-            _logit_bias, _ = get_logit_bias(name, prefer)
+            _logit_bias, _, max_tokens = get_logit_bias(name, prefer)
+
+            if "max_tokens" not in kwargs:
+                kwargs["max_tokens"] = max_tokens
 
             logit_bias.update(_logit_bias)
         if avoid:
-            _logit_bias, _ = get_logit_bias(name, avoid, bias=-100)
+            _logit_bias, _, _ = get_logit_bias(name, avoid, bias=-100)
 
             logit_bias.update(_logit_bias)
 
         if logit_bias:
             kwargs["logit_bias"] = logit_bias
 
             # this is a hard limit by OpenAI for tokens with a logit bias
```

### Comparing `fastllm-0.1.4/fastllm/utils.py` & `fastllm-0.1.5/fastllm/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import exrex
 import tiktoken
 
 
 def get_logit_bias(
     model_name: str, pattern: list[str] | str, bias: int = 100, limit: int = 10000
-) -> tuple[dict[str, int], list[str]]:
+) -> tuple[dict[str, int], list[str], int]:
     """Given a model name, a pattern and a bias, returns a logit bias dict."""
 
     tokenizer = tiktoken.encoding_for_model(model_name)
 
     encoded_strings = []
     for p in [pattern] if isinstance(pattern, str) else pattern:
         try:
@@ -33,10 +33,15 @@
 
             strings = exrex.generate(p, limit=limit)
         else:
             strings = [p]
 
         encoded_strings += tokenizer.encode_batch(strings)
 
+    max_tokens = len(max(encoded_strings, key=len))
     tokens = set(chain.from_iterable(encoded_strings))
 
-    return {f"{t}": bias for t in tokens}, [tokenizer.decode([t]) for t in tokens]
+    return (
+        {f"{t}": bias for t in tokens},
+        [tokenizer.decode([t]) for t in tokens],
+        max_tokens,
+    )
```

### Comparing `fastllm-0.1.4/pyproject.toml` & `fastllm-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastllm"
-version = "0.1.4"
+version = "0.1.5"
 description = "Fast and easy wrapper around LLMs."
 authors = ["Clemens Kriechbaumer <clemens.kriechbaumer@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/clemens33/fastllm"
 repository = "https://github.com/clemens33/fastllm"
 keywords = ["agents", "chatbots", "openai", "llm", "ai"]
```

