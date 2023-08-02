# Comparing `tmp/dfv-0.7.0.tar.gz` & `tmp/dfv-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfv-0.7.0.tar", max compression
+gzip compressed data, was "dfv-0.8.0.tar", max compression
```

## Comparing `dfv-0.7.0.tar` & `dfv-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    17371 2023-08-02 19:53:41.847374 dfv-0.7.0/dfv/__init__.py
--rw-r--r--   0        0        0    28620 2023-08-02 19:53:44.291403 dfv-0.7.0/dfv/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10456 2023-07-31 19:21:19.730323 dfv-0.7.0/dfv/__pycache__/test_element.cpython-311.pyc
--rw-r--r--   0        0        0     8642 2023-07-29 08:01:02.515193 dfv-0.7.0/dfv/__pycache__/test_form.cpython-311.pyc
--rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.7.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
--rw-r--r--   0        0        0     4496 2023-08-02 19:49:36.096341 dfv-0.7.0/dfv/__pycache__/test_view.cpython-311.pyc
--rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.7.0/dfv/static/dfv.js
--rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.7.0/dfv/templates/dfv/tests/TemplateResponse.html
--rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.7.0/dfv/templatetags/__init__.py
--rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.7.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.7.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
--rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.7.0/dfv/templatetags/dfv.py
--rw-r--r--   0        0        0     4328 2023-07-31 19:19:29.401041 dfv-0.7.0/dfv/test_element.py
--rw-r--r--   0        0        0     3340 2023-07-29 08:01:00.971175 dfv-0.7.0/dfv/test_form.py
--rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.7.0/dfv/test_params_to_args.py
--rw-r--r--   0        0        0     1646 2023-08-02 19:49:35.828337 dfv-0.7.0/dfv/test_view.py
--rw-r--r--   0        0        0     1438 2023-08-01 20:43:58.184518 dfv-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.7.0/setup.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    17876 2023-08-02 20:07:26.193267 dfv-0.8.0/dfv/__init__.py
+-rw-r--r--   0        0        0    29012 2023-08-02 20:07:54.981616 dfv-0.8.0/dfv/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10456 2023-07-31 19:21:19.730323 dfv-0.8.0/dfv/__pycache__/test_element.cpython-311.pyc
+-rw-r--r--   0        0        0     8642 2023-07-29 08:01:02.515193 dfv-0.8.0/dfv/__pycache__/test_form.cpython-311.pyc
+-rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.8.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
+-rw-r--r--   0        0        0     4496 2023-08-02 19:49:36.096341 dfv-0.8.0/dfv/__pycache__/test_view.cpython-311.pyc
+-rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.8.0/dfv/static/dfv.js
+-rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.8.0/dfv/templates/dfv/tests/TemplateResponse.html
+-rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.8.0/dfv/templatetags/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.8.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.8.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
+-rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.8.0/dfv/templatetags/dfv.py
+-rw-r--r--   0        0        0     4328 2023-07-31 19:19:29.401041 dfv-0.8.0/dfv/test_element.py
+-rw-r--r--   0        0        0     3340 2023-07-29 08:01:00.971175 dfv-0.8.0/dfv/test_form.py
+-rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.8.0/dfv/test_params_to_args.py
+-rw-r--r--   0        0        0     1646 2023-08-02 19:49:35.828337 dfv-0.8.0/dfv/test_view.py
+-rw-r--r--   0        0        0     1438 2023-08-02 20:07:31.369330 dfv-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.8.0/setup.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.8.0/PKG-INFO
```

### Comparing `dfv-0.7.0/dfv/__init__.py` & `dfv-0.8.0/dfv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,22 +70,27 @@
     element_id: Optional[str] = None,
     *,
     tag="div",
     hx_target="this",
     hx_swap="outerHTML",
     classes: Optional[str] = None,
     handle_args=True,
+    decorators: Optional[list[Callable]] = None,
     login_required=False,
 ) -> Callable[[Callable[P, R]], Callable[P, R]]:
     def decorator(f: Callable[P, HttpResponse]) -> Callable[P, HttpResponse]:
         id = element_id if isinstance(element_id, str) else f.__name__
-        f = view(handle_args)(f)
+        f = view(
+            handle_args=handle_args,
+            decorators=decorators,
+            login_required=login_required,
+        )(f)
 
-        if login_required:
-            f = auth_decorators.login_required()(f)
+        # if login_required:
+        #     f = auth_decorators.login_required()(f)
 
         @functools.wraps(f)
         def inner(*args: P.args, **kwargs: P.kwargs) -> HttpResponse:
             response = f(*args, **kwargs)
             if not response["Content-Type"].startswith("text/html"):
                 return response
 
@@ -144,19 +149,33 @@
 ) -> Optional[list[Callable]]:
     call_stack = getattr(request, "__dfv_view_fn_call_stack", None)
     call_stack = [] if call_stack is None and create else call_stack
     setattr(request, "__dfv_view_fn_call_stack", call_stack)
     return call_stack
 
 
-def view(handle_args=True) -> Callable[[Callable[P, R]], Callable[P, R]]:
+def view(
+    *,
+    decorators: Optional[list[Callable]] = None,
+    login_required=False,
+    handle_args=True,
+) -> Callable[[Callable[P, R]], Callable[P, R]]:
+    if decorators is None:
+        decorators = []
+    if login_required:
+        decorators = [auth_decorators.login_required(), *decorators]
+
     def decorator(fn: Callable[P, R]) -> Callable[P, R]:
         if handle_args:
             fn = _inject_args()(fn)
 
+        if decorators is not None:
+            for d in reversed(decorators):
+                fn = d(fn)
+
         @functools.wraps(fn)
         def inner(*args: P.args, **kwargs: P.kwargs) -> R:
             view_request: HttpRequest = args[0]
             stack = get_view_fn_call_stack_from_request(view_request)
             try:
                 stack.append(fn)
                 return fn(*args, **kwargs)
```

### Comparing `dfv-0.7.0/dfv/__pycache__/__init__.cpython-311.pyc` & `dfv-0.8.0/dfv/__pycache__/__init__.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,66 +1,69 @@
 magic:    0xa70d0d0a
-moddate:  0x45b4ca64 (Wed Aug  2 19:53:41 2023 UTC)
-files sz: 17371
+moddate:  0x7eb7ca64 (Wed Aug  2 20:07:26 2023 UTC)
+files sz: 17876
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 13
+   stacksize : 14
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       016c035a03640064016c045a04640064016c055a05640064026c066d075a
       070100640064036c046d085a086d095a096d0a5a0a6d0b5a0b6d0c5a0c6d
       0d5a0d0100640064016c0e5a0f640064016c105a10640064046c116d125a
       120100640064056c136d145a150100640064066c166d175a176d185a186d
       195a196d1a5a1a0100640064076c1b6d1c5a1c0100640064086c1d6d1e5a
       1e6d1f5a1f01000200650c6409a6010000ab0100000000000000005a2002
       00650d640aa6010000ab0100000000000000005a210200650d640ba60100
       00ab0100000000000000005a2202004700640c8400640d65106a23000000
       0000000000a6030000ab0300000000000000005a24640e6518651c7a0700
-      00640f651f6604641084045a250900644d64116412641364016414641564
-      169c066417650b6526190000000000000000006418650b65261900000000
+      00640f651f6604641084045a250900644f64116412641364016414640164
+      1564169c076417650b6526190000000000000000006418650b6526190000
+      000000000000006419650b65276509190000000000000000001900000000
       0000000000640f6509650965206521660219000000000000000000670165
       096520652166021900000000000000000066021900000000000000000066
-      06641984075a270900644e640e6518641a6518640f65186606641b84055a
-      2865046a290000000000000000641c6517640f652a650919000000000000
-      0000006604641d8404a6000000ab0000000000000000005a2b65046a2900
-      00000000000000641c6517641e652c640f650b652a650919000000000000
-      000000190000000000000000006606641f8404a6000000ab000000000000
-      0000005a2b0900644f641c6517640f650b652a6509190000000000000000
-      00190000000000000000006604642084055a2b644f640f65096509652065
-      216602190000000000000000006701650965206521660219000000000000
-      0000006602190000000000000000006602642184055a2d641c6517660264
-      2284045a2e641c65176602642384045a2f641c65176602642484045a3064
-      1c65176602642584045a31641c65176602642684045a32641c6517660264
-      2784045a33641c65176602642884045a346415641464299c02642a652c65
-      0a642b190000000000000000007a070000642c650b652c65267a07000019
-      000000000000000000640f65096509652065216602190000000000000000
-      006701650965206521660219000000000000000000660219000000000000
-      0000006606642d84065a3565355a3665006a370000000000000000020047
-      00642e8400642fa6020000ab020000000000000000a6000000ab00000000
-      00000000005a386430650965086701650866021900000000000000000064
-      31653864326526643365026a3900000000000000006608643484045a3a09
-      00644f643065096508670165086602190000000000000000006435652a65
-      026a39000000000000000019000000000000000000642a652c650a643619
-      0000000000000000007a070000650a6437190000000000000000007a0700
-      00642c650b652c65267a07000019000000000000000000640f653b652665
-      38660219000000000000000000660a643884055a3c65006a370000000000
-      0000000200470064398400643a6538a6030000ab030000000000000000a6
-      000000ab0000000000000000005a3d65006a370000000000000000020047
-      00643b8400643c653da6030000ab030000000000000000a6000000ab0000
-      000000000000005a3e65006a37000000000000000002004700643d840064
-      3e653da6030000ab030000000000000000a6000000ab0000000000000000
-      005a3f6450640f65086602643f84055a406450640f65086602644084055a
-      41020065046a42000000000000000065086401a6020000ab020000000000
-      0000006414660264416522640f65226604644284055a436443652a65046a
-      08000000000000000019000000000000000000644465446604644584045a
-      45020047006446840064476538a6030000ab0300000000000000005a4664
-      0f65086602644884045a476449653b640f651a6604644a84045a48644b65
-      2a650819000000000000000000640f65176604644c84045a4964015300
+      08641a84075a2809006450640e6518641b6518640f65186606641c84055a
+      2965046a2a0000000000000000641d6517640f6527650919000000000000
+      0000006604641e8404a6000000ab0000000000000000005a2b65046a2a00
+      00000000000000641d6517641f652c640f650b6527650919000000000000
+      00000019000000000000000000660664208404a6000000ab000000000000
+      0000005a2b09006451641d6517640f650b65276509190000000000000000
+      00190000000000000000006604642184055a2b64016415641464229c0364
+      19650b652765091900000000000000000019000000000000000000640f65
+      096509652065216602190000000000000000006701650965206521660219
+      0000000000000000006602190000000000000000006604642384065a2d64
+      1d65176602642484045a2e641d65176602642584045a2f641d6517660264
+      2684045a30641d65176602642784045a31641d65176602642884045a3264
+      1d65176602642984045a33641d65176602642a84045a3464156414642b9c
+      02642c652c650a642d190000000000000000007a070000642e650b652c65
+      267a07000019000000000000000000640f65096509652065216602190000
+      000000000000006701650965206521660219000000000000000000660219
+      0000000000000000006606642f84065a3565355a3665006a370000000000
+      00000002004700643084006431a6020000ab020000000000000000a60000
+      00ab0000000000000000005a386432650965086701650866021900000000
+      00000000006433653864346526643565026a390000000000000000660864
+      3684045a3a09006451643265096508670165086602190000000000000000
+      006437652765026a39000000000000000019000000000000000000642c65
+      2c650a6438190000000000000000007a070000650a643919000000000000
+      0000007a070000642e650b652c65267a0700001900000000000000000064
+      0f653b65266538660219000000000000000000660a643a84055a3c65006a
+      37000000000000000002004700643b8400643c6538a6030000ab03000000
+      0000000000a6000000ab0000000000000000005a3d65006a370000000000
+      00000002004700643d8400643e653da6030000ab030000000000000000a6
+      000000ab0000000000000000005a3e65006a370000000000000000020047
+      00643f84006440653da6030000ab030000000000000000a6000000ab0000
+      000000000000005a3f6452640f65086602644184055a406452640f650866
+      02644284055a41020065046a42000000000000000065086401a6020000ab
+      0200000000000000006414660264436522640f65226604644484055a4364
+      45652765046a080000000000000000190000000000000000006446654466
+      04644784045a45020047006448840064496538a6030000ab030000000000
+      0000005a46640f65086602644a84045a47644b653b640f651a6604644c84
+      045a48644d6527650819000000000000000000640f65176604644e84045a
+      4964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (dataclasses)
                  8 STORE_NAME               0 (dataclasses)
    
@@ -207,497 +210,524 @@
                304 BUILD_TUPLE              4
                306 LOAD_CONST              16 (<code object response_to_str, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 61>)
                308 MAKE_FUNCTION            4 (annotations)
                310 STORE_NAME              37 (response_to_str)
    
     70         312 NOP
    
-    69         314 LOAD_CONST              77 ((None,))
+    69         314 LOAD_CONST              79 ((None,))
    
     72         316 LOAD_CONST              17 ('div')
    
     73         318 LOAD_CONST              18 ('this')
    
     74         320 LOAD_CONST              19 ('outerHTML')
    
     75         322 LOAD_CONST               1 (None)
    
     76         324 LOAD_CONST              20 (True)
    
-    77         326 LOAD_CONST              21 (False)
+    77         326 LOAD_CONST               1 (None)
    
-    69         328 LOAD_CONST              22 (('tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required'))
-               330 BUILD_CONST_KEY_MAP      6
-               332 LOAD_CONST              23 ('element_id')
-   
-    70         334 LOAD_NAME               11 (Optional)
-               336 LOAD_NAME               38 (str)
-               338 BINARY_SUBSCR
-   
-    69         348 LOAD_CONST              24 ('classes')
-   
-    75         350 LOAD_NAME               11 (Optional)
-               352 LOAD_NAME               38 (str)
-               354 BINARY_SUBSCR
-   
-    69         364 LOAD_CONST              15 ('return')
-   
-    78         366 LOAD_NAME                9 (Callable)
-               368 LOAD_NAME                9 (Callable)
-               370 LOAD_NAME               32 (P)
-               372 LOAD_NAME               33 (R)
-               374 BUILD_TUPLE              2
-               376 BINARY_SUBSCR
-               386 BUILD_LIST               1
-               388 LOAD_NAME                9 (Callable)
-               390 LOAD_NAME               32 (P)
-               392 LOAD_NAME               33 (R)
-               394 BUILD_TUPLE              2
-               396 BINARY_SUBSCR
-               406 BUILD_TUPLE              2
-               408 BINARY_SUBSCR
-   
-    69         418 BUILD_TUPLE              6
-               420 LOAD_CONST              25 (<code object element, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 69>)
-               422 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
-               424 STORE_NAME              39 (element)
-   
-   110         426 NOP
-   
-   109         428 LOAD_CONST              78 (('outerHTML',))
-               430 LOAD_CONST              14 ('response')
-   
-   110         432 LOAD_NAME               24 (HttpResponse)
-   
-   109         434 LOAD_CONST              26 ('additional')
-   
-   110         436 LOAD_NAME               24 (HttpResponse)
-   
-   109         438 LOAD_CONST              15 ('return')
-   
-   111         440 LOAD_NAME               24 (HttpResponse)
-   
-   109         442 BUILD_TUPLE              6
-               444 LOAD_CONST              27 (<code object swap_oob, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 109>)
-               446 MAKE_FUNCTION            5 (defaults, annotations)
-               448 STORE_NAME              40 (swap_oob)
-   
-   130         450 LOAD_NAME                4 (typing)
-               452 LOAD_ATTR               41 (overload)
-   
-   131         462 LOAD_CONST              28 ('request')
-               464 LOAD_NAME               23 (HttpRequest)
-               466 LOAD_CONST              15 ('return')
-               468 LOAD_NAME               42 (list)
-               470 LOAD_NAME                9 (Callable)
-               472 BINARY_SUBSCR
-               482 BUILD_TUPLE              4
-               484 LOAD_CONST              29 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 130>)
-               486 MAKE_FUNCTION            4 (annotations)
-   
-   130         488 PRECALL                  0
-               492 CALL                     0
-   
-   131         502 STORE_NAME              43 (get_view_fn_call_stack_from_request)
-   
-   135         504 LOAD_NAME                4 (typing)
-               506 LOAD_ATTR               41 (overload)
-   
-   136         516 LOAD_CONST              28 ('request')
-   
-   137         518 LOAD_NAME               23 (HttpRequest)
-   
-   136         520 LOAD_CONST              30 ('create')
-   
-   137         522 LOAD_NAME               44 (bool)
-   
-   136         524 LOAD_CONST              15 ('return')
-   
-   138         526 LOAD_NAME               11 (Optional)
-               528 LOAD_NAME               42 (list)
-               530 LOAD_NAME                9 (Callable)
-               532 BINARY_SUBSCR
-               542 BINARY_SUBSCR
-   
-   136         552 BUILD_TUPLE              6
-               554 LOAD_CONST              31 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 135>)
-               556 MAKE_FUNCTION            4 (annotations)
-   
-   135         558 PRECALL                  0
-               562 CALL                     0
-   
-   136         572 STORE_NAME              43 (get_view_fn_call_stack_from_request)
-   
-   143         574 NOP
-   
-   142         576 LOAD_CONST              79 ((True,))
-               578 LOAD_CONST              28 ('request')
-   
-   143         580 LOAD_NAME               23 (HttpRequest)
-   
-   142         582 LOAD_CONST              15 ('return')
-   
-   144         584 LOAD_NAME               11 (Optional)
-               586 LOAD_NAME               42 (list)
-               588 LOAD_NAME                9 (Callable)
-               590 BINARY_SUBSCR
-               600 BINARY_SUBSCR
-   
-   142         610 BUILD_TUPLE              4
-               612 LOAD_CONST              32 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 142>)
-               614 MAKE_FUNCTION            5 (defaults, annotations)
-               616 STORE_NAME              43 (get_view_fn_call_stack_from_request)
-   
-   151         618 LOAD_CONST              79 ((True,))
-               620 LOAD_CONST              15 ('return')
-               622 LOAD_NAME                9 (Callable)
-               624 LOAD_NAME                9 (Callable)
-               626 LOAD_NAME               32 (P)
-               628 LOAD_NAME               33 (R)
-               630 BUILD_TUPLE              2
-               632 BINARY_SUBSCR
-               642 BUILD_LIST               1
-               644 LOAD_NAME                9 (Callable)
-               646 LOAD_NAME               32 (P)
-               648 LOAD_NAME               33 (R)
-               650 BUILD_TUPLE              2
-               652 BINARY_SUBSCR
-               662 BUILD_TUPLE              2
-               664 BINARY_SUBSCR
-               674 BUILD_TUPLE              2
-               676 LOAD_CONST              33 (<code object view, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 151>)
-               678 MAKE_FUNCTION            5 (defaults, annotations)
-               680 STORE_NAME              45 (view)
-   
-   171         682 LOAD_CONST              28 ('request')
-               684 LOAD_NAME               23 (HttpRequest)
-               686 BUILD_TUPLE              2
-               688 LOAD_CONST              34 (<code object is_view_fn_request_target, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 171>)
-               690 MAKE_FUNCTION            4 (annotations)
-               692 STORE_NAME              46 (is_view_fn_request_target)
-   
-   176         694 LOAD_CONST              28 ('request')
-               696 LOAD_NAME               23 (HttpRequest)
-               698 BUILD_TUPLE              2
-               700 LOAD_CONST              35 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 176>)
-               702 MAKE_FUNCTION            4 (annotations)
-               704 STORE_NAME              47 (is_head)
-   
-   180         706 LOAD_CONST              28 ('request')
-               708 LOAD_NAME               23 (HttpRequest)
-               710 BUILD_TUPLE              2
-               712 LOAD_CONST              36 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 180>)
-               714 MAKE_FUNCTION            4 (annotations)
-               716 STORE_NAME              48 (is_get)
-   
-   184         718 LOAD_CONST              28 ('request')
-               720 LOAD_NAME               23 (HttpRequest)
-               722 BUILD_TUPLE              2
-               724 LOAD_CONST              37 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 184>)
-               726 MAKE_FUNCTION            4 (annotations)
-               728 STORE_NAME              49 (is_post)
-   
-   188         730 LOAD_CONST              28 ('request')
-               732 LOAD_NAME               23 (HttpRequest)
-               734 BUILD_TUPLE              2
-               736 LOAD_CONST              38 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 188>)
-               738 MAKE_FUNCTION            4 (annotations)
-               740 STORE_NAME              50 (is_put)
-   
-   192         742 LOAD_CONST              28 ('request')
-               744 LOAD_NAME               23 (HttpRequest)
-               746 BUILD_TUPLE              2
-               748 LOAD_CONST              39 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 192>)
-               750 MAKE_FUNCTION            4 (annotations)
-               752 STORE_NAME              51 (is_patch)
-   
-   196         754 LOAD_CONST              28 ('request')
-               756 LOAD_NAME               23 (HttpRequest)
-               758 BUILD_TUPLE              2
-               760 LOAD_CONST              40 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 196>)
-               762 MAKE_FUNCTION            4 (annotations)
-               764 STORE_NAME              52 (is_delete)
-   
-   207         766 LOAD_CONST              21 (False)
-   
-   208         768 LOAD_CONST              20 (True)
-   
-   205         770 LOAD_CONST              41 (('auto_param', 'auto_form'))
-               772 BUILD_CONST_KEY_MAP      2
-               774 LOAD_CONST              42 ('auto_param')
-   
-   207         776 LOAD_NAME               44 (bool)
-               778 LOAD_NAME               10 (Literal)
-               780 LOAD_CONST              43 (('get', 'post'))
-               782 BINARY_SUBSCR
-               792 BINARY_OP                7 (|)
-   
-   205         796 LOAD_CONST              44 ('auto_form')
-   
-   208         798 LOAD_NAME               11 (Optional)
-               800 LOAD_NAME               44 (bool)
-               802 LOAD_NAME               38 (str)
-               804 BINARY_OP                7 (|)
-               808 BINARY_SUBSCR
-   
-   205         818 LOAD_CONST              15 ('return')
-   
-   209         820 LOAD_NAME                9 (Callable)
-               822 LOAD_NAME                9 (Callable)
-               824 LOAD_NAME               32 (P)
-               826 LOAD_NAME               33 (R)
-               828 BUILD_TUPLE              2
-               830 BINARY_SUBSCR
-               840 BUILD_LIST               1
-               842 LOAD_NAME                9 (Callable)
-               844 LOAD_NAME               32 (P)
-               846 LOAD_NAME               33 (R)
-               848 BUILD_TUPLE              2
-               850 BINARY_SUBSCR
-               860 BUILD_TUPLE              2
-               862 BINARY_SUBSCR
-   
-   205         872 BUILD_TUPLE              6
-               874 LOAD_CONST              45 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 205>)
-               876 MAKE_FUNCTION            6 (kwdefaults, annotations)
-               878 STORE_NAME              53 (inject_args)
-   
-   239         880 LOAD_NAME               53 (inject_args)
-               882 STORE_NAME              54 (_inject_args)
-   
-   242         884 LOAD_NAME                0 (dataclasses)
-               886 LOAD_ATTR               55 (dataclass)
-   
-   243         896 PUSH_NULL
-               898 LOAD_BUILD_CLASS
-               900 LOAD_CONST              46 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 242>)
-               902 MAKE_FUNCTION            0
-               904 LOAD_CONST              47 ('InjectedParam')
-               906 PRECALL                  2
-               910 CALL                     2
-   
-   242         920 PRECALL                  0
-               924 CALL                     0
-   
-   243         934 STORE_NAME              56 (InjectedParam)
-   
-   260         936 LOAD_CONST              48 ('view_fn')
-   
-   261         938 LOAD_NAME                9 (Callable)
-               940 LOAD_NAME                8 (Any)
-               942 BUILD_LIST               1
-               944 LOAD_NAME                8 (Any)
-               946 BUILD_TUPLE              2
-               948 BINARY_SUBSCR
-   
-   260         958 LOAD_CONST              49 ('ip')
-   
-   262         960 LOAD_NAME               56 (InjectedParam)
-   
-   260         962 LOAD_CONST              50 ('name')
-   
-   263         964 LOAD_NAME               38 (str)
-   
-   260         966 LOAD_CONST              51 ('parameter')
-   
-   264         968 LOAD_NAME                2 (inspect)
-               970 LOAD_ATTR               57 (Parameter)
-   
-   260         980 BUILD_TUPLE              8
-               982 LOAD_CONST              52 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 260>)
-               984 MAKE_FUNCTION            4 (annotations)
-               986 STORE_NAME              58 (_setup_injected_param)
-   
-   287         988 NOP
-   
-   283         990 LOAD_CONST              79 ((True,))
-               992 LOAD_CONST              48 ('view_fn')
-   
-   284         994 LOAD_NAME                9 (Callable)
-               996 LOAD_NAME                8 (Any)
-               998 BUILD_LIST               1
-              1000 LOAD_NAME                8 (Any)
-              1002 BUILD_TUPLE              2
-              1004 BINARY_SUBSCR
-   
-   283        1014 LOAD_CONST              53 ('parameters')
-   
-   285        1016 LOAD_NAME               42 (list)
-              1018 LOAD_NAME                2 (inspect)
-              1020 LOAD_ATTR               57 (Parameter)
-              1030 BINARY_SUBSCR
-   
-   283        1040 LOAD_CONST              42 ('auto_param')
-   
-   286        1042 LOAD_NAME               44 (bool)
-              1044 LOAD_NAME               10 (Literal)
-              1046 LOAD_CONST              54 ('get')
-              1048 BINARY_SUBSCR
-              1058 BINARY_OP                7 (|)
-              1062 LOAD_NAME               10 (Literal)
-              1064 LOAD_CONST              55 ('post')
-              1066 BINARY_SUBSCR
-              1076 BINARY_OP                7 (|)
-   
-   283        1080 LOAD_CONST              44 ('auto_form')
-   
-   287        1082 LOAD_NAME               11 (Optional)
-              1084 LOAD_NAME               44 (bool)
-              1086 LOAD_NAME               38 (str)
-              1088 BINARY_OP                7 (|)
-              1092 BINARY_SUBSCR
-   
-   283        1102 LOAD_CONST              15 ('return')
-   
-   288        1104 LOAD_NAME               59 (dict)
-              1106 LOAD_NAME               38 (str)
-              1108 LOAD_NAME               56 (InjectedParam)
-              1110 BUILD_TUPLE              2
-              1112 BINARY_SUBSCR
-   
-   283        1122 BUILD_TUPLE             10
-              1124 LOAD_CONST              56 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 283>)
-              1126 MAKE_FUNCTION            5 (defaults, annotations)
-              1128 STORE_NAME              60 (_extract_injected_params)
-   
-   347        1130 LOAD_NAME                0 (dataclasses)
-              1132 LOAD_ATTR               55 (dataclass)
-   
-   348        1142 PUSH_NULL
-              1144 LOAD_BUILD_CLASS
-              1146 LOAD_CONST              57 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 347>)
-              1148 MAKE_FUNCTION            0
-              1150 LOAD_CONST              58 ('InjectedParamQuery')
-              1152 LOAD_NAME               56 (InjectedParam)
-              1154 PRECALL                  3
-              1158 CALL                     3
-   
-   347        1168 PRECALL                  0
-              1172 CALL                     0
-   
-   348        1182 STORE_NAME              61 (InjectedParamQuery)
-   
-   395        1184 LOAD_NAME                0 (dataclasses)
-              1186 LOAD_ATTR               55 (dataclass)
-   
-   396        1196 PUSH_NULL
-              1198 LOAD_BUILD_CLASS
-              1200 LOAD_CONST              59 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 395>)
-              1202 MAKE_FUNCTION            0
-              1204 LOAD_CONST              60 ('InjectedParamQueryGet')
-              1206 LOAD_NAME               61 (InjectedParamQuery)
-              1208 PRECALL                  3
-              1212 CALL                     3
-   
-   395        1222 PRECALL                  0
-              1226 CALL                     0
-   
-   396        1236 STORE_NAME              62 (InjectedParamQueryGet)
-   
-   408        1238 LOAD_NAME                0 (dataclasses)
-              1240 LOAD_ATTR               55 (dataclass)
-   
-   409        1250 PUSH_NULL
-              1252 LOAD_BUILD_CLASS
-              1254 LOAD_CONST              61 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 408>)
-              1256 MAKE_FUNCTION            0
-              1258 LOAD_CONST              62 ('InjectedParamQueryPost')
-              1260 LOAD_NAME               61 (InjectedParamQuery)
-              1262 PRECALL                  3
-              1266 CALL                     3
-   
-   408        1276 PRECALL                  0
-              1280 CALL                     0
-   
-   409        1290 STORE_NAME              63 (InjectedParamQueryPost)
-   
-   421        1292 LOAD_CONST              80 ((None, True))
-              1294 LOAD_CONST              15 ('return')
-              1296 LOAD_NAME                8 (Any)
-              1298 BUILD_TUPLE              2
-              1300 LOAD_CONST              63 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 421>)
-              1302 MAKE_FUNCTION            5 (defaults, annotations)
-              1304 STORE_NAME              64 (param_get)
-   
-   425        1306 LOAD_CONST              80 ((None, True))
-              1308 LOAD_CONST              15 ('return')
-              1310 LOAD_NAME                8 (Any)
-              1312 BUILD_TUPLE              2
-              1314 LOAD_CONST              64 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 425>)
-              1316 MAKE_FUNCTION            5 (defaults, annotations)
-              1318 STORE_NAME              65 (param_post)
-   
-   429        1320 PUSH_NULL
-              1322 LOAD_NAME                4 (typing)
-              1324 LOAD_ATTR               66 (cast)
-              1334 LOAD_NAME                8 (Any)
-              1336 LOAD_CONST               1 (None)
-              1338 PRECALL                  2
-              1342 CALL                     2
-              1352 LOAD_CONST              20 (True)
-              1354 BUILD_TUPLE              2
-              1356 LOAD_CONST              65 ('default')
-              1358 LOAD_NAME               34 (T)
+    78         328 LOAD_CONST              21 (False)
+   
+    69         330 LOAD_CONST              22 (('tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'decorators', 'login_required'))
+               332 BUILD_CONST_KEY_MAP      7
+               334 LOAD_CONST              23 ('element_id')
+   
+    70         336 LOAD_NAME               11 (Optional)
+               338 LOAD_NAME               38 (str)
+               340 BINARY_SUBSCR
+   
+    69         350 LOAD_CONST              24 ('classes')
+   
+    75         352 LOAD_NAME               11 (Optional)
+               354 LOAD_NAME               38 (str)
+               356 BINARY_SUBSCR
+   
+    69         366 LOAD_CONST              25 ('decorators')
+   
+    77         368 LOAD_NAME               11 (Optional)
+               370 LOAD_NAME               39 (list)
+               372 LOAD_NAME                9 (Callable)
+               374 BINARY_SUBSCR
+               384 BINARY_SUBSCR
+   
+    69         394 LOAD_CONST              15 ('return')
+   
+    79         396 LOAD_NAME                9 (Callable)
+               398 LOAD_NAME                9 (Callable)
+               400 LOAD_NAME               32 (P)
+               402 LOAD_NAME               33 (R)
+               404 BUILD_TUPLE              2
+               406 BINARY_SUBSCR
+               416 BUILD_LIST               1
+               418 LOAD_NAME                9 (Callable)
+               420 LOAD_NAME               32 (P)
+               422 LOAD_NAME               33 (R)
+               424 BUILD_TUPLE              2
+               426 BINARY_SUBSCR
+               436 BUILD_TUPLE              2
+               438 BINARY_SUBSCR
+   
+    69         448 BUILD_TUPLE              8
+               450 LOAD_CONST              26 (<code object element, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 69>)
+               452 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
+               454 STORE_NAME              40 (element)
+   
+   115         456 NOP
+   
+   114         458 LOAD_CONST              80 (('outerHTML',))
+               460 LOAD_CONST              14 ('response')
+   
+   115         462 LOAD_NAME               24 (HttpResponse)
+   
+   114         464 LOAD_CONST              27 ('additional')
+   
+   115         466 LOAD_NAME               24 (HttpResponse)
+   
+   114         468 LOAD_CONST              15 ('return')
+   
+   116         470 LOAD_NAME               24 (HttpResponse)
+   
+   114         472 BUILD_TUPLE              6
+               474 LOAD_CONST              28 (<code object swap_oob, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 114>)
+               476 MAKE_FUNCTION            5 (defaults, annotations)
+               478 STORE_NAME              41 (swap_oob)
+   
+   135         480 LOAD_NAME                4 (typing)
+               482 LOAD_ATTR               42 (overload)
+   
+   136         492 LOAD_CONST              29 ('request')
+               494 LOAD_NAME               23 (HttpRequest)
+               496 LOAD_CONST              15 ('return')
+               498 LOAD_NAME               39 (list)
+               500 LOAD_NAME                9 (Callable)
+               502 BINARY_SUBSCR
+               512 BUILD_TUPLE              4
+               514 LOAD_CONST              30 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 135>)
+               516 MAKE_FUNCTION            4 (annotations)
+   
+   135         518 PRECALL                  0
+               522 CALL                     0
+   
+   136         532 STORE_NAME              43 (get_view_fn_call_stack_from_request)
+   
+   140         534 LOAD_NAME                4 (typing)
+               536 LOAD_ATTR               42 (overload)
+   
+   141         546 LOAD_CONST              29 ('request')
+   
+   142         548 LOAD_NAME               23 (HttpRequest)
+   
+   141         550 LOAD_CONST              31 ('create')
+   
+   142         552 LOAD_NAME               44 (bool)
+   
+   141         554 LOAD_CONST              15 ('return')
+   
+   143         556 LOAD_NAME               11 (Optional)
+               558 LOAD_NAME               39 (list)
+               560 LOAD_NAME                9 (Callable)
+               562 BINARY_SUBSCR
+               572 BINARY_SUBSCR
+   
+   141         582 BUILD_TUPLE              6
+               584 LOAD_CONST              32 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 140>)
+               586 MAKE_FUNCTION            4 (annotations)
+   
+   140         588 PRECALL                  0
+               592 CALL                     0
+   
+   141         602 STORE_NAME              43 (get_view_fn_call_stack_from_request)
+   
+   148         604 NOP
+   
+   147         606 LOAD_CONST              81 ((True,))
+               608 LOAD_CONST              29 ('request')
+   
+   148         610 LOAD_NAME               23 (HttpRequest)
+   
+   147         612 LOAD_CONST              15 ('return')
+   
+   149         614 LOAD_NAME               11 (Optional)
+               616 LOAD_NAME               39 (list)
+               618 LOAD_NAME                9 (Callable)
+               620 BINARY_SUBSCR
+               630 BINARY_SUBSCR
+   
+   147         640 BUILD_TUPLE              4
+               642 LOAD_CONST              33 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 147>)
+               644 MAKE_FUNCTION            5 (defaults, annotations)
+               646 STORE_NAME              43 (get_view_fn_call_stack_from_request)
+   
+   158         648 LOAD_CONST               1 (None)
+   
+   159         650 LOAD_CONST              21 (False)
+   
+   160         652 LOAD_CONST              20 (True)
+   
+   156         654 LOAD_CONST              34 (('decorators', 'login_required', 'handle_args'))
+               656 BUILD_CONST_KEY_MAP      3
+               658 LOAD_CONST              25 ('decorators')
+   
+   158         660 LOAD_NAME               11 (Optional)
+               662 LOAD_NAME               39 (list)
+               664 LOAD_NAME                9 (Callable)
+               666 BINARY_SUBSCR
+               676 BINARY_SUBSCR
+   
+   156         686 LOAD_CONST              15 ('return')
+   
+   161         688 LOAD_NAME                9 (Callable)
+               690 LOAD_NAME                9 (Callable)
+               692 LOAD_NAME               32 (P)
+               694 LOAD_NAME               33 (R)
+               696 BUILD_TUPLE              2
+               698 BINARY_SUBSCR
+               708 BUILD_LIST               1
+               710 LOAD_NAME                9 (Callable)
+               712 LOAD_NAME               32 (P)
+               714 LOAD_NAME               33 (R)
+               716 BUILD_TUPLE              2
+               718 BINARY_SUBSCR
+               728 BUILD_TUPLE              2
+               730 BINARY_SUBSCR
+   
+   156         740 BUILD_TUPLE              4
+               742 LOAD_CONST              35 (<code object view, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 156>)
+               744 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               746 STORE_NAME              45 (view)
+   
+   190         748 LOAD_CONST              29 ('request')
+               750 LOAD_NAME               23 (HttpRequest)
+               752 BUILD_TUPLE              2
+               754 LOAD_CONST              36 (<code object is_view_fn_request_target, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 190>)
+               756 MAKE_FUNCTION            4 (annotations)
+               758 STORE_NAME              46 (is_view_fn_request_target)
+   
+   195         760 LOAD_CONST              29 ('request')
+               762 LOAD_NAME               23 (HttpRequest)
+               764 BUILD_TUPLE              2
+               766 LOAD_CONST              37 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 195>)
+               768 MAKE_FUNCTION            4 (annotations)
+               770 STORE_NAME              47 (is_head)
+   
+   199         772 LOAD_CONST              29 ('request')
+               774 LOAD_NAME               23 (HttpRequest)
+               776 BUILD_TUPLE              2
+               778 LOAD_CONST              38 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 199>)
+               780 MAKE_FUNCTION            4 (annotations)
+               782 STORE_NAME              48 (is_get)
+   
+   203         784 LOAD_CONST              29 ('request')
+               786 LOAD_NAME               23 (HttpRequest)
+               788 BUILD_TUPLE              2
+               790 LOAD_CONST              39 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 203>)
+               792 MAKE_FUNCTION            4 (annotations)
+               794 STORE_NAME              49 (is_post)
+   
+   207         796 LOAD_CONST              29 ('request')
+               798 LOAD_NAME               23 (HttpRequest)
+               800 BUILD_TUPLE              2
+               802 LOAD_CONST              40 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 207>)
+               804 MAKE_FUNCTION            4 (annotations)
+               806 STORE_NAME              50 (is_put)
+   
+   211         808 LOAD_CONST              29 ('request')
+               810 LOAD_NAME               23 (HttpRequest)
+               812 BUILD_TUPLE              2
+               814 LOAD_CONST              41 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 211>)
+               816 MAKE_FUNCTION            4 (annotations)
+               818 STORE_NAME              51 (is_patch)
+   
+   215         820 LOAD_CONST              29 ('request')
+               822 LOAD_NAME               23 (HttpRequest)
+               824 BUILD_TUPLE              2
+               826 LOAD_CONST              42 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 215>)
+               828 MAKE_FUNCTION            4 (annotations)
+               830 STORE_NAME              52 (is_delete)
+   
+   226         832 LOAD_CONST              21 (False)
+   
+   227         834 LOAD_CONST              20 (True)
+   
+   224         836 LOAD_CONST              43 (('auto_param', 'auto_form'))
+               838 BUILD_CONST_KEY_MAP      2
+               840 LOAD_CONST              44 ('auto_param')
+   
+   226         842 LOAD_NAME               44 (bool)
+               844 LOAD_NAME               10 (Literal)
+               846 LOAD_CONST              45 (('get', 'post'))
+               848 BINARY_SUBSCR
+               858 BINARY_OP                7 (|)
+   
+   224         862 LOAD_CONST              46 ('auto_form')
+   
+   227         864 LOAD_NAME               11 (Optional)
+               866 LOAD_NAME               44 (bool)
+               868 LOAD_NAME               38 (str)
+               870 BINARY_OP                7 (|)
+               874 BINARY_SUBSCR
+   
+   224         884 LOAD_CONST              15 ('return')
+   
+   228         886 LOAD_NAME                9 (Callable)
+               888 LOAD_NAME                9 (Callable)
+               890 LOAD_NAME               32 (P)
+               892 LOAD_NAME               33 (R)
+               894 BUILD_TUPLE              2
+               896 BINARY_SUBSCR
+               906 BUILD_LIST               1
+               908 LOAD_NAME                9 (Callable)
+               910 LOAD_NAME               32 (P)
+               912 LOAD_NAME               33 (R)
+               914 BUILD_TUPLE              2
+               916 BINARY_SUBSCR
+               926 BUILD_TUPLE              2
+               928 BINARY_SUBSCR
+   
+   224         938 BUILD_TUPLE              6
+               940 LOAD_CONST              47 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 224>)
+               942 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               944 STORE_NAME              53 (inject_args)
+   
+   258         946 LOAD_NAME               53 (inject_args)
+               948 STORE_NAME              54 (_inject_args)
+   
+   261         950 LOAD_NAME                0 (dataclasses)
+               952 LOAD_ATTR               55 (dataclass)
+   
+   262         962 PUSH_NULL
+               964 LOAD_BUILD_CLASS
+               966 LOAD_CONST              48 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 261>)
+               968 MAKE_FUNCTION            0
+               970 LOAD_CONST              49 ('InjectedParam')
+               972 PRECALL                  2
+               976 CALL                     2
+   
+   261         986 PRECALL                  0
+               990 CALL                     0
+   
+   262        1000 STORE_NAME              56 (InjectedParam)
+   
+   279        1002 LOAD_CONST              50 ('view_fn')
+   
+   280        1004 LOAD_NAME                9 (Callable)
+              1006 LOAD_NAME                8 (Any)
+              1008 BUILD_LIST               1
+              1010 LOAD_NAME                8 (Any)
+              1012 BUILD_TUPLE              2
+              1014 BINARY_SUBSCR
+   
+   279        1024 LOAD_CONST              51 ('ip')
+   
+   281        1026 LOAD_NAME               56 (InjectedParam)
+   
+   279        1028 LOAD_CONST              52 ('name')
+   
+   282        1030 LOAD_NAME               38 (str)
+   
+   279        1032 LOAD_CONST              53 ('parameter')
+   
+   283        1034 LOAD_NAME                2 (inspect)
+              1036 LOAD_ATTR               57 (Parameter)
+   
+   279        1046 BUILD_TUPLE              8
+              1048 LOAD_CONST              54 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 279>)
+              1050 MAKE_FUNCTION            4 (annotations)
+              1052 STORE_NAME              58 (_setup_injected_param)
+   
+   306        1054 NOP
+   
+   302        1056 LOAD_CONST              81 ((True,))
+              1058 LOAD_CONST              50 ('view_fn')
+   
+   303        1060 LOAD_NAME                9 (Callable)
+              1062 LOAD_NAME                8 (Any)
+              1064 BUILD_LIST               1
+              1066 LOAD_NAME                8 (Any)
+              1068 BUILD_TUPLE              2
+              1070 BINARY_SUBSCR
+   
+   302        1080 LOAD_CONST              55 ('parameters')
+   
+   304        1082 LOAD_NAME               39 (list)
+              1084 LOAD_NAME                2 (inspect)
+              1086 LOAD_ATTR               57 (Parameter)
+              1096 BINARY_SUBSCR
+   
+   302        1106 LOAD_CONST              44 ('auto_param')
+   
+   305        1108 LOAD_NAME               44 (bool)
+              1110 LOAD_NAME               10 (Literal)
+              1112 LOAD_CONST              56 ('get')
+              1114 BINARY_SUBSCR
+              1124 BINARY_OP                7 (|)
+              1128 LOAD_NAME               10 (Literal)
+              1130 LOAD_CONST              57 ('post')
+              1132 BINARY_SUBSCR
+              1142 BINARY_OP                7 (|)
+   
+   302        1146 LOAD_CONST              46 ('auto_form')
+   
+   306        1148 LOAD_NAME               11 (Optional)
+              1150 LOAD_NAME               44 (bool)
+              1152 LOAD_NAME               38 (str)
+              1154 BINARY_OP                7 (|)
+              1158 BINARY_SUBSCR
+   
+   302        1168 LOAD_CONST              15 ('return')
+   
+   307        1170 LOAD_NAME               59 (dict)
+              1172 LOAD_NAME               38 (str)
+              1174 LOAD_NAME               56 (InjectedParam)
+              1176 BUILD_TUPLE              2
+              1178 BINARY_SUBSCR
+   
+   302        1188 BUILD_TUPLE             10
+              1190 LOAD_CONST              58 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 302>)
+              1192 MAKE_FUNCTION            5 (defaults, annotations)
+              1194 STORE_NAME              60 (_extract_injected_params)
+   
+   366        1196 LOAD_NAME                0 (dataclasses)
+              1198 LOAD_ATTR               55 (dataclass)
+   
+   367        1208 PUSH_NULL
+              1210 LOAD_BUILD_CLASS
+              1212 LOAD_CONST              59 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 366>)
+              1214 MAKE_FUNCTION            0
+              1216 LOAD_CONST              60 ('InjectedParamQuery')
+              1218 LOAD_NAME               56 (InjectedParam)
+              1220 PRECALL                  3
+              1224 CALL                     3
+   
+   366        1234 PRECALL                  0
+              1238 CALL                     0
+   
+   367        1248 STORE_NAME              61 (InjectedParamQuery)
+   
+   414        1250 LOAD_NAME                0 (dataclasses)
+              1252 LOAD_ATTR               55 (dataclass)
+   
+   415        1262 PUSH_NULL
+              1264 LOAD_BUILD_CLASS
+              1266 LOAD_CONST              61 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 414>)
+              1268 MAKE_FUNCTION            0
+              1270 LOAD_CONST              62 ('InjectedParamQueryGet')
+              1272 LOAD_NAME               61 (InjectedParamQuery)
+              1274 PRECALL                  3
+              1278 CALL                     3
+   
+   414        1288 PRECALL                  0
+              1292 CALL                     0
+   
+   415        1302 STORE_NAME              62 (InjectedParamQueryGet)
+   
+   427        1304 LOAD_NAME                0 (dataclasses)
+              1306 LOAD_ATTR               55 (dataclass)
+   
+   428        1316 PUSH_NULL
+              1318 LOAD_BUILD_CLASS
+              1320 LOAD_CONST              63 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 427>)
+              1322 MAKE_FUNCTION            0
+              1324 LOAD_CONST              64 ('InjectedParamQueryPost')
+              1326 LOAD_NAME               61 (InjectedParamQuery)
+              1328 PRECALL                  3
+              1332 CALL                     3
+   
+   427        1342 PRECALL                  0
+              1346 CALL                     0
+   
+   428        1356 STORE_NAME              63 (InjectedParamQueryPost)
+   
+   440        1358 LOAD_CONST              82 ((None, True))
               1360 LOAD_CONST              15 ('return')
-              1362 LOAD_NAME               34 (T)
-              1364 BUILD_TUPLE              4
-              1366 LOAD_CONST              66 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 429>)
+              1362 LOAD_NAME                8 (Any)
+              1364 BUILD_TUPLE              2
+              1366 LOAD_CONST              65 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 440>)
               1368 MAKE_FUNCTION            5 (defaults, annotations)
-              1370 STORE_NAME              67 (param)
+              1370 STORE_NAME              64 (param_get)
    
-   433        1372 LOAD_CONST              67 ('values')
-              1374 LOAD_NAME               42 (list)
-              1376 LOAD_NAME                4 (typing)
-              1378 LOAD_ATTR                8 (Any)
-              1388 BINARY_SUBSCR
-              1398 LOAD_CONST              68 ('target_type')
-              1400 LOAD_NAME               68 (type)
-              1402 BUILD_TUPLE              4
-              1404 LOAD_CONST              69 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 433>)
-              1406 MAKE_FUNCTION            4 (annotations)
-              1408 STORE_NAME              69 (_convert_value_to_type)
-   
-   468        1410 PUSH_NULL
-              1412 LOAD_BUILD_CLASS
-              1414 LOAD_CONST              70 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 468>)
-              1416 MAKE_FUNCTION            0
-              1418 LOAD_CONST              71 ('InjectedParamForm')
-              1420 LOAD_NAME               56 (InjectedParam)
-              1422 PRECALL                  3
-              1426 CALL                     3
-              1436 STORE_NAME              70 (InjectedParamForm)
-   
-   514        1438 LOAD_CONST              15 ('return')
-              1440 LOAD_NAME                8 (Any)
-              1442 BUILD_TUPLE              2
-              1444 LOAD_CONST              72 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 514>)
-              1446 MAKE_FUNCTION            4 (annotations)
-              1448 STORE_NAME              71 (handle_form)
-   
-   523        1450 LOAD_CONST              73 ('querydict')
-              1452 LOAD_NAME               59 (dict)
-              1454 LOAD_CONST              15 ('return')
-              1456 LOAD_NAME               26 (QueryDict)
-              1458 BUILD_TUPLE              4
-              1460 LOAD_CONST              74 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 523>)
-              1462 MAKE_FUNCTION            4 (annotations)
-              1464 STORE_NAME              72 (querydict_key_removed)
-   
-   530        1466 LOAD_CONST              75 ('args')
-              1468 LOAD_NAME               42 (list)
-              1470 LOAD_NAME                8 (Any)
-              1472 BINARY_SUBSCR
-              1482 LOAD_CONST              15 ('return')
-              1484 LOAD_NAME               23 (HttpRequest)
-              1486 BUILD_TUPLE              4
-              1488 LOAD_CONST              76 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 530>)
-              1490 MAKE_FUNCTION            4 (annotations)
-              1492 STORE_NAME              73 (_get_request_from_args)
-              1494 LOAD_CONST               1 (None)
-              1496 RETURN_VALUE
+   444        1372 LOAD_CONST              82 ((None, True))
+              1374 LOAD_CONST              15 ('return')
+              1376 LOAD_NAME                8 (Any)
+              1378 BUILD_TUPLE              2
+              1380 LOAD_CONST              66 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 444>)
+              1382 MAKE_FUNCTION            5 (defaults, annotations)
+              1384 STORE_NAME              65 (param_post)
+   
+   448        1386 PUSH_NULL
+              1388 LOAD_NAME                4 (typing)
+              1390 LOAD_ATTR               66 (cast)
+              1400 LOAD_NAME                8 (Any)
+              1402 LOAD_CONST               1 (None)
+              1404 PRECALL                  2
+              1408 CALL                     2
+              1418 LOAD_CONST              20 (True)
+              1420 BUILD_TUPLE              2
+              1422 LOAD_CONST              67 ('default')
+              1424 LOAD_NAME               34 (T)
+              1426 LOAD_CONST              15 ('return')
+              1428 LOAD_NAME               34 (T)
+              1430 BUILD_TUPLE              4
+              1432 LOAD_CONST              68 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 448>)
+              1434 MAKE_FUNCTION            5 (defaults, annotations)
+              1436 STORE_NAME              67 (param)
+   
+   452        1438 LOAD_CONST              69 ('values')
+              1440 LOAD_NAME               39 (list)
+              1442 LOAD_NAME                4 (typing)
+              1444 LOAD_ATTR                8 (Any)
+              1454 BINARY_SUBSCR
+              1464 LOAD_CONST              70 ('target_type')
+              1466 LOAD_NAME               68 (type)
+              1468 BUILD_TUPLE              4
+              1470 LOAD_CONST              71 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 452>)
+              1472 MAKE_FUNCTION            4 (annotations)
+              1474 STORE_NAME              69 (_convert_value_to_type)
+   
+   487        1476 PUSH_NULL
+              1478 LOAD_BUILD_CLASS
+              1480 LOAD_CONST              72 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 487>)
+              1482 MAKE_FUNCTION            0
+              1484 LOAD_CONST              73 ('InjectedParamForm')
+              1486 LOAD_NAME               56 (InjectedParam)
+              1488 PRECALL                  3
+              1492 CALL                     3
+              1502 STORE_NAME              70 (InjectedParamForm)
+   
+   533        1504 LOAD_CONST              15 ('return')
+              1506 LOAD_NAME                8 (Any)
+              1508 BUILD_TUPLE              2
+              1510 LOAD_CONST              74 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 533>)
+              1512 MAKE_FUNCTION            4 (annotations)
+              1514 STORE_NAME              71 (handle_form)
+   
+   542        1516 LOAD_CONST              75 ('querydict')
+              1518 LOAD_NAME               59 (dict)
+              1520 LOAD_CONST              15 ('return')
+              1522 LOAD_NAME               26 (QueryDict)
+              1524 BUILD_TUPLE              4
+              1526 LOAD_CONST              76 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 542>)
+              1528 MAKE_FUNCTION            4 (annotations)
+              1530 STORE_NAME              72 (querydict_key_removed)
+   
+   549        1532 LOAD_CONST              77 ('args')
+              1534 LOAD_NAME               39 (list)
+              1536 LOAD_NAME                8 (Any)
+              1538 BINARY_SUBSCR
+              1548 LOAD_CONST              15 ('return')
+              1550 LOAD_NAME               23 (HttpRequest)
+              1552 BUILD_TUPLE              4
+              1554 LOAD_CONST              78 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 549>)
+              1556 MAKE_FUNCTION            4 (annotations)
+              1558 STORE_NAME              73 (_get_request_from_args)
+              1560 LOAD_CONST               1 (None)
+              1562 RETURN_VALUE
    consts
       0
       None
       ('NoneType',)
       ('Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar')
       ('forms',)
       ('decorators',)
@@ -1050,161 +1080,159 @@
          firstlineno 61
          lnotab 0x02012a012802
       'div'
       'this'
       'outerHTML'
       True
       False
-      ('tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required')
+      ('tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'decorators', 'login_required')
       'element_id'
       'classes'
+      'decorators'
       code
          argcount  : 1
-         nlocals   : 8
-         stacksize : 8
+         nlocals   : 9
+         stacksize : 9
          flags     : 3
          code
-            0x8700870187028703870487058706970064017400000000000000000000
-            007402000000000000000000007404000000000000000000006602190000
-            000000000000006402740000000000000000000000740200000000000000
-            000000740400000000000000000000660219000000000000000000660488
-            0488008805880388028806880166076403840c7d077c075300
+            0x8700870187028703870487058706870797006401740000000000000000
+            000000740200000000000000000000740400000000000000000000660219
+            000000000000000000640274000000000000000000000074020000000000
+            000000000074040000000000000000000066021900000000000000000066
+            048804880688008805880388028807880166086403840c7d087c085300
                        0 MAKE_CELL                0 (element_id)
                        2 MAKE_CELL                1 (tag)
                        4 MAKE_CELL                2 (hx_target)
                        6 MAKE_CELL                3 (hx_swap)
                        8 MAKE_CELL                4 (classes)
                       10 MAKE_CELL                5 (handle_args)
-                      12 MAKE_CELL                6 (login_required)
+                      12 MAKE_CELL                6 (decorators)
+                      14 MAKE_CELL                7 (login_required)
          
-          69          14 RESUME                   0
+          69          16 RESUME                   0
          
-          79          16 LOAD_CONST               1 ('f')
-                      18 LOAD_GLOBAL              0 (Callable)
-                      30 LOAD_GLOBAL              2 (P)
-                      42 LOAD_GLOBAL              4 (HttpResponse)
-                      54 BUILD_TUPLE              2
-                      56 BINARY_SUBSCR
-                      66 LOAD_CONST               2 ('return')
-                      68 LOAD_GLOBAL              0 (Callable)
-                      80 LOAD_GLOBAL              2 (P)
-                      92 LOAD_GLOBAL              4 (HttpResponse)
-                     104 BUILD_TUPLE              2
-                     106 BINARY_SUBSCR
-                     116 BUILD_TUPLE              4
-                     118 LOAD_CLOSURE             4 (classes)
-                     120 LOAD_CLOSURE             0 (element_id)
-                     122 LOAD_CLOSURE             5 (handle_args)
-                     124 LOAD_CLOSURE             3 (hx_swap)
-                     126 LOAD_CLOSURE             2 (hx_target)
-                     128 LOAD_CLOSURE             6 (login_required)
-                     130 LOAD_CLOSURE             1 (tag)
-                     132 BUILD_TUPLE              7
-                     134 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 79>)
-                     136 MAKE_FUNCTION           12 (annotations, closure)
-                     138 STORE_FAST               7 (decorator)
+          80          18 LOAD_CONST               1 ('f')
+                      20 LOAD_GLOBAL              0 (Callable)
+                      32 LOAD_GLOBAL              2 (P)
+                      44 LOAD_GLOBAL              4 (HttpResponse)
+                      56 BUILD_TUPLE              2
+                      58 BINARY_SUBSCR
+                      68 LOAD_CONST               2 ('return')
+                      70 LOAD_GLOBAL              0 (Callable)
+                      82 LOAD_GLOBAL              2 (P)
+                      94 LOAD_GLOBAL              4 (HttpResponse)
+                     106 BUILD_TUPLE              2
+                     108 BINARY_SUBSCR
+                     118 BUILD_TUPLE              4
+                     120 LOAD_CLOSURE             4 (classes)
+                     122 LOAD_CLOSURE             6 (decorators)
+                     124 LOAD_CLOSURE             0 (element_id)
+                     126 LOAD_CLOSURE             5 (handle_args)
+                     128 LOAD_CLOSURE             3 (hx_swap)
+                     130 LOAD_CLOSURE             2 (hx_target)
+                     132 LOAD_CLOSURE             7 (login_required)
+                     134 LOAD_CLOSURE             1 (tag)
+                     136 BUILD_TUPLE              8
+                     138 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 80>)
+                     140 MAKE_FUNCTION           12 (annotations, closure)
+                     142 STORE_FAST               8 (decorator)
          
-         106         140 LOAD_FAST                7 (decorator)
-                     142 RETURN_VALUE
+         111         144 LOAD_FAST                8 (decorator)
+                     146 RETURN_VALUE
          consts
             None
             'f'
             'return'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 19
                code
-                  0x9507870087029700740100000000000000000000890474020000000000
-                  0000000000a6020000ab020000000000000000720289046e0689006a0200
-                  000000000000008a0202007407000000000000000000008905a6010000ab
-                  0100000000000000008900a6010000ab0100000000000000008a00890872
-                  1c02007409000000000000000000006a050000000000000000a6000000ab
-                  0000000000000000008900a6010000ab0100000000000000008a00740d00
-                  0000000000000000006a0700000000000000008900a6010000ab01000000
-                  000000000064017410000000000000000000006a09000000000000000064
-                  027410000000000000000000006a0a000000000000000064037416000000
-                  00000000000000660688038800880688078802880966066404840ca60000
-                  00ab0000000000000000007d017c015300
-                             0 COPY_FREE_VARS           7
+                  0x9508870087029700740100000000000000000000890574020000000000
+                  0000000000a6020000ab020000000000000000720289056e0689006a0200
+                  000000000000008a020200740700000000000000000000890689048909ac
+                  01a6030000ab0300000000000000008900a6010000ab0100000000000000
+                  008a007409000000000000000000006a0500000000000000008900a60100
+                  00ab0100000000000000006402740c000000000000000000006a07000000
+                  00000000006403740c000000000000000000006a08000000000000000064
+                  04741200000000000000000000660688038800880788088802880a660664
+                  05840ca6000000ab0000000000000000007d017c015300
+                             0 COPY_FREE_VARS           8
                              2 MAKE_CELL                0 (f)
                              4 MAKE_CELL                2 (id)
                
-                79           6 RESUME                   0
+                80           6 RESUME                   0
                
-                80           8 LOAD_GLOBAL              1 (NULL + isinstance)
-                            20 LOAD_DEREF               4 (element_id)
+                81           8 LOAD_GLOBAL              1 (NULL + isinstance)
+                            20 LOAD_DEREF               5 (element_id)
                             22 LOAD_GLOBAL              2 (str)
                             34 PRECALL                  2
                             38 CALL                     2
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
-                            50 LOAD_DEREF               4 (element_id)
+                            50 LOAD_DEREF               5 (element_id)
                             52 JUMP_FORWARD             6 (to 66)
                        >>   54 LOAD_DEREF               0 (f)
                             56 LOAD_ATTR                2 (__name__)
                        >>   66 STORE_DEREF              2 (id)
                
-                81          68 PUSH_NULL
+                82          68 PUSH_NULL
                             70 LOAD_GLOBAL              7 (NULL + view)
-                            82 LOAD_DEREF               5 (handle_args)
-                            84 PRECALL                  1
-                            88 CALL                     1
-                            98 LOAD_DEREF               0 (f)
-                           100 PRECALL                  1
-                           104 CALL                     1
-                           114 STORE_DEREF              0 (f)
                
-                83         116 LOAD_DEREF               8 (login_required)
-                           118 POP_JUMP_FORWARD_IF_FALSE    28 (to 176)
+                83          82 LOAD_DEREF               6 (handle_args)
                
-                84         120 PUSH_NULL
-                           122 LOAD_GLOBAL              9 (NULL + auth_decorators)
-                           134 LOAD_ATTR                5 (login_required)
-                           144 PRECALL                  0
-                           148 CALL                     0
-                           158 LOAD_DEREF               0 (f)
-                           160 PRECALL                  1
-                           164 CALL                     1
-                           174 STORE_DEREF              0 (f)
-               
-                86     >>  176 LOAD_GLOBAL             13 (NULL + functools)
-                           188 LOAD_ATTR                7 (wraps)
-                           198 LOAD_DEREF               0 (f)
-                           200 PRECALL                  1
-                           204 CALL                     1
-               
-                87         214 LOAD_CONST               1 ('args')
-                           216 LOAD_GLOBAL             16 (P)
-                           228 LOAD_ATTR                9 (args)
-                           238 LOAD_CONST               2 ('kwargs')
-                           240 LOAD_GLOBAL             16 (P)
-                           252 LOAD_ATTR               10 (kwargs)
-                           262 LOAD_CONST               3 ('return')
-                           264 LOAD_GLOBAL             22 (HttpResponse)
-                           276 BUILD_TUPLE              6
-                           278 LOAD_CLOSURE             3 (classes)
-                           280 LOAD_CLOSURE             0 (f)
-                           282 LOAD_CLOSURE             6 (hx_swap)
-                           284 LOAD_CLOSURE             7 (hx_target)
-                           286 LOAD_CLOSURE             2 (id)
-                           288 LOAD_CLOSURE             9 (tag)
-                           290 BUILD_TUPLE              6
-                           292 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 86>)
-                           294 MAKE_FUNCTION           12 (annotations, closure)
+                84          84 LOAD_DEREF               4 (decorators)
                
-                86         296 PRECALL                  0
-                           300 CALL                     0
+                85          86 LOAD_DEREF               9 (login_required)
                
-                87         310 STORE_FAST               1 (inner)
+                82          88 KW_NAMES                 1
+                            90 PRECALL                  3
+                            94 CALL                     3
                
-               104         312 LOAD_FAST                1 (inner)
-                           314 RETURN_VALUE
+                86         104 LOAD_DEREF               0 (f)
+               
+                82         106 PRECALL                  1
+                           110 CALL                     1
+                           120 STORE_DEREF              0 (f)
+               
+                91         122 LOAD_GLOBAL              9 (NULL + functools)
+                           134 LOAD_ATTR                5 (wraps)
+                           144 LOAD_DEREF               0 (f)
+                           146 PRECALL                  1
+                           150 CALL                     1
+               
+                92         160 LOAD_CONST               2 ('args')
+                           162 LOAD_GLOBAL             12 (P)
+                           174 LOAD_ATTR                7 (args)
+                           184 LOAD_CONST               3 ('kwargs')
+                           186 LOAD_GLOBAL             12 (P)
+                           198 LOAD_ATTR                8 (kwargs)
+                           208 LOAD_CONST               4 ('return')
+                           210 LOAD_GLOBAL             18 (HttpResponse)
+                           222 BUILD_TUPLE              6
+                           224 LOAD_CLOSURE             3 (classes)
+                           226 LOAD_CLOSURE             0 (f)
+                           228 LOAD_CLOSURE             7 (hx_swap)
+                           230 LOAD_CLOSURE             8 (hx_target)
+                           232 LOAD_CLOSURE             2 (id)
+                           234 LOAD_CLOSURE            10 (tag)
+                           236 BUILD_TUPLE              6
+                           238 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 91>)
+                           240 MAKE_FUNCTION           12 (annotations, closure)
+               
+                91         242 PRECALL                  0
+                           246 CALL                     0
+               
+                92         256 STORE_FAST               1 (inner)
+               
+               109         258 LOAD_FAST                1 (inner)
+                           260 RETURN_VALUE
                consts
                   None
+                  ('handle_args', 'decorators', 'login_required')
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
                      nlocals   : 3
                      stacksize : 8
@@ -1214,94 +1242,94 @@
                         0000000000a00000000000000000000000000000000000000000006402a6
                         010000ab01000000000000000073027c0253007403000000000000000000
                         007c02740400000000000000000000a6020000ab02000000000000000072
                         027c0253007405000000000000000000007c0289078908890689058903ac
                         03a6060000ab0600000000000000005300
                                    0 COPY_FREE_VARS           6
                      
-                      86           2 RESUME                   0
+                      91           2 RESUME                   0
                      
-                      88           4 PUSH_NULL
+                      93           4 PUSH_NULL
                                    6 LOAD_DEREF               4 (f)
                                    8 LOAD_FAST                0 (args)
                                   10 BUILD_MAP                0
                                   12 LOAD_FAST                1 (kwargs)
                                   14 DICT_MERGE               1
                                   16 CALL_FUNCTION_EX         1
                                   18 STORE_FAST               2 (response)
                      
-                      89          20 LOAD_FAST                2 (response)
+                      94          20 LOAD_FAST                2 (response)
                                   22 LOAD_CONST               1 ('Content-Type')
                                   24 BINARY_SUBSCR
                                   34 LOAD_METHOD              0 (startswith)
                                   56 LOAD_CONST               2 ('text/html')
                                   58 PRECALL                  1
                                   62 CALL                     1
                                   72 POP_JUMP_FORWARD_IF_TRUE     2 (to 78)
                      
-                      90          74 LOAD_FAST                2 (response)
+                      95          74 LOAD_FAST                2 (response)
                                   76 RETURN_VALUE
                      
-                      92     >>   78 LOAD_GLOBAL              3 (NULL + isinstance)
+                      97     >>   78 LOAD_GLOBAL              3 (NULL + isinstance)
                                   90 LOAD_FAST                2 (response)
                                   92 LOAD_GLOBAL              4 (ElementResponse)
                                  104 PRECALL                  2
                                  108 CALL                     2
                                  118 POP_JUMP_FORWARD_IF_FALSE     2 (to 124)
                      
-                      93         120 LOAD_FAST                2 (response)
+                      98         120 LOAD_FAST                2 (response)
                                  122 RETURN_VALUE
                      
-                      95     >>  124 LOAD_GLOBAL              5 (NULL + ElementResponse)
+                     100     >>  124 LOAD_GLOBAL              5 (NULL + ElementResponse)
                      
-                      96         136 LOAD_FAST                2 (response)
+                     101         136 LOAD_FAST                2 (response)
                      
-                      97         138 LOAD_DEREF               7 (id)
+                     102         138 LOAD_DEREF               7 (id)
                      
-                      98         140 LOAD_DEREF               8 (tag)
+                     103         140 LOAD_DEREF               8 (tag)
                      
-                      99         142 LOAD_DEREF               6 (hx_target)
+                     104         142 LOAD_DEREF               6 (hx_target)
                      
-                     100         144 LOAD_DEREF               5 (hx_swap)
+                     105         144 LOAD_DEREF               5 (hx_swap)
                      
-                     101         146 LOAD_DEREF               3 (classes)
+                     106         146 LOAD_DEREF               3 (classes)
                      
-                      95         148 KW_NAMES                 3
+                     100         148 KW_NAMES                 3
                                  150 PRECALL                  6
                                  154 CALL                     6
                                  164 RETURN_VALUE
                      consts
                         None
                         'Content-Type'
                         'text/html'
                         ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes')
                      names      ('startswith', 'isinstance', 'ElementResponse')
                      varnames   ('args', 'kwargs', 'response')
                      freevars   ('classes', 'f', 'hx_swap', 'hx_target', 'id', 'tag')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 86
+                     firstlineno 91
                      lnotab 0x04021001360104022a0104020c010201020102010201020102fa
-               names      ('isinstance', 'str', '__name__', 'view', 'auth_decorators', 'login_required', 'functools', 'wraps', 'P', 'args', 'kwargs', 'HttpResponse')
+               names      ('isinstance', 'str', '__name__', 'view', 'functools', 'wraps', 'P', 'args', 'kwargs', 'HttpResponse')
                varnames   ('f', 'inner')
-               freevars   ('classes', 'element_id', 'handle_args', 'hx_swap', 'hx_target', 'login_required', 'tag')
+               freevars   ('classes', 'decorators', 'element_id', 'handle_args', 'hx_swap', 'hx_target', 'login_required', 'tag')
                cellvars   ('f', 'id')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 79
-               lnotab 0x08013c01300204013802260152ff0e010211
+               firstlineno 80
+               lnotab 0x08013c010e010201020102fd100402fc1009260152ff0e010211
          names      ('Callable', 'P', 'HttpResponse')
-         varnames   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required', 'decorator')
+         varnames   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'decorators', 'login_required', 'decorator')
          freevars   ()
-         cellvars   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required')
+         cellvars   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'decorators', 'login_required')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'element'
          firstlineno 69
-         lnotab 0x100a7c1b
+         lnotab 0x120b7e1f
       'additional'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1313,281 +1341,325 @@
             0000000000000000000000000000006401a6010000ab0100000000000000
             007d057c05800f740f000000000000000000006402a6010000ab01000000
             000000000082017c029b0064037c059b009d037c046a0500000000000000
             0064043c0000007c0078016a080000000000000000740400000000000000
             0000006a030000000000000000a009000000000000000000000000000000
             00000000007c04a6010000ab0100000000000000007a0d000063025f0800
             000000000000007c005300
-         109           0 RESUME                   0
+         114           0 RESUME                   0
          
-         112           2 LOAD_GLOBAL              1 (NULL + response_to_str)
+         117           2 LOAD_GLOBAL              1 (NULL + response_to_str)
                       14 LOAD_FAST                1 (additional)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_METHOD              1 (strip)
                       52 PRECALL                  0
                       56 CALL                     0
                       66 STORE_FAST               3 (oob_content)
          
-         113          68 LOAD_GLOBAL              4 (lxml)
+         118          68 LOAD_GLOBAL              4 (lxml)
                       80 LOAD_ATTR                3 (html)
                       90 LOAD_METHOD              4 (fromstring)
                      112 LOAD_FAST                3 (oob_content)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 STORE_FAST               4 (parsed)
          
-         114         130 LOAD_FAST                4 (parsed)
+         119         130 LOAD_FAST                4 (parsed)
                      132 LOAD_ATTR                5 (attrib)
                      142 LOAD_METHOD              6 (get)
                      164 LOAD_CONST               1 ('id')
                      166 PRECALL                  1
                      170 CALL                     1
                      180 STORE_FAST               5 (id)
          
-         115         182 LOAD_FAST                5 (id)
+         120         182 LOAD_FAST                5 (id)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 216)
          
-         116         186 LOAD_GLOBAL             15 (NULL + Exception)
+         121         186 LOAD_GLOBAL             15 (NULL + Exception)
          
-         117         198 LOAD_CONST               2 ('The additional response does not contain exactly one element with an id attribute.')
+         122         198 LOAD_CONST               2 ('The additional response does not contain exactly one element with an id attribute.')
          
-         116         200 PRECALL                  1
+         121         200 PRECALL                  1
                      204 CALL                     1
                      214 RAISE_VARARGS            1
          
-         120     >>  216 LOAD_FAST                2 (hx_swap_oob_method)
+         125     >>  216 LOAD_FAST                2 (hx_swap_oob_method)
                      218 FORMAT_VALUE             0
                      220 LOAD_CONST               3 (':#')
                      222 LOAD_FAST                5 (id)
                      224 FORMAT_VALUE             0
                      226 BUILD_STRING             3
                      228 LOAD_FAST                4 (parsed)
                      230 LOAD_ATTR                5 (attrib)
                      240 LOAD_CONST               4 ('hx-swap-oob')
                      242 STORE_SUBSCR
          
-         121         246 LOAD_FAST                0 (response)
+         126         246 LOAD_FAST                0 (response)
                      248 COPY                     1
                      250 LOAD_ATTR                8 (content)
                      260 LOAD_GLOBAL              4 (lxml)
                      272 LOAD_ATTR                3 (html)
                      282 LOAD_METHOD              9 (tostring)
                      304 LOAD_FAST                4 (parsed)
                      306 PRECALL                  1
                      310 CALL                     1
                      320 BINARY_OP               13 (+=)
                      324 SWAP                     2
                      326 STORE_ATTR               8 (content)
          
-         122         336 LOAD_FAST                0 (response)
+         127         336 LOAD_FAST                0 (response)
                      338 RETURN_VALUE
          consts
             None
             'id'
             'The additional response does not contain exactly one element with an id attribute.'
             ':#'
             'hx-swap-oob'
          names      ('response_to_str', 'strip', 'lxml', 'html', 'fromstring', 'attrib', 'get', 'Exception', 'content', 'tostring')
          varnames   ('response', 'additional', 'hx_swap_oob_method', 'oob_content', 'parsed', 'id')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'swap_oob'
-         firstlineno 109
+         firstlineno 114
          lnotab 0x020342013e01340104010c0102ff10041e015a01
       'request'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 1
          flags     : 3
          code 0x970064005300
-         130           0 RESUME                   0
+         135           0 RESUME                   0
          
-         132           2 LOAD_CONST               0 (None)
+         137           2 LOAD_CONST               0 (None)
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'get_view_fn_call_stack_from_request'
-         firstlineno 130
+         firstlineno 135
          lnotab 0x0202
       'create'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 1
          flags     : 3
          code 0x970064005300
-         135           0 RESUME                   0
+         140           0 RESUME                   0
          
-         139           2 LOAD_CONST               0 (None)
+         144           2 LOAD_CONST               0 (None)
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('request', 'create')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'get_view_fn_call_stack_from_request'
-         firstlineno 135
+         firstlineno 140
          lnotab 0x0204
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007c0064016400a6030000ab03000000
             00000000007d027c0280047c01720267006e017c027d0274030000000000
             00000000007c0064017c02a6030000ab03000000000000000001007c0253
             00
-         142           0 RESUME                   0
+         147           0 RESUME                   0
          
-         145           2 LOAD_GLOBAL              1 (NULL + getattr)
+         150           2 LOAD_GLOBAL              1 (NULL + getattr)
                       14 LOAD_FAST                0 (request)
                       16 LOAD_CONST               1 ('__dfv_view_fn_call_stack')
                       18 LOAD_CONST               0 (None)
                       20 PRECALL                  3
                       24 CALL                     3
                       34 STORE_FAST               2 (call_stack)
          
-         146          36 LOAD_FAST                2 (call_stack)
+         151          36 LOAD_FAST                2 (call_stack)
                       38 POP_JUMP_FORWARD_IF_NOT_NONE     4 (to 48)
                       40 LOAD_FAST                1 (create)
                       42 POP_JUMP_FORWARD_IF_FALSE     2 (to 48)
                       44 BUILD_LIST               0
                       46 JUMP_FORWARD             1 (to 50)
                  >>   48 LOAD_FAST                2 (call_stack)
                  >>   50 STORE_FAST               2 (call_stack)
          
-         147          52 LOAD_GLOBAL              3 (NULL + setattr)
+         152          52 LOAD_GLOBAL              3 (NULL + setattr)
                       64 LOAD_FAST                0 (request)
                       66 LOAD_CONST               1 ('__dfv_view_fn_call_stack')
                       68 LOAD_FAST                2 (call_stack)
                       70 PRECALL                  3
                       74 CALL                     3
                       84 POP_TOP
          
-         148          86 LOAD_FAST                2 (call_stack)
+         153          86 LOAD_FAST                2 (call_stack)
                       88 RETURN_VALUE
          consts
             None
             '__dfv_view_fn_call_stack'
          names      ('getattr', 'setattr')
          varnames   ('request', 'create', 'call_stack')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'get_view_fn_call_stack_from_request'
-         firstlineno 142
+         firstlineno 147
          lnotab 0x0203220110012201
+      ('decorators', 'login_required', 'handle_args')
       code
-         argcount  : 1
-         nlocals   : 2
+         argcount  : 0
+         nlocals   : 4
          stacksize : 6
          flags     : 3
          code
-            0x8700970064017400000000000000000000007402000000000000000000
-            007404000000000000000000006602190000000000000000006402740000
-            000000000000000000740200000000000000000000740400000000000000
-            0000006602190000000000000000006604880066016403840c7d017c0153
+            0x8700870297008900800267008a007c0172167401000000000000000000
+            006a010000000000000000a6000000ab00000000000000000067018900a2
+            018a00640174040000000000000000000074060000000000000000000074
+            080000000000000000000066021900000000000000000064027404000000
+            000000000000007406000000000000000000007408000000000000000000
+            0066021900000000000000000066048800880266026403840c7d037c0353
             00
-                       0 MAKE_CELL                0 (handle_args)
+                       0 MAKE_CELL                0 (decorators)
+                       2 MAKE_CELL                2 (handle_args)
+         
+         156           4 RESUME                   0
          
-         151           2 RESUME                   0
+         162           6 LOAD_DEREF               0 (decorators)
+                       8 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 14)
          
-         152           4 LOAD_CONST               1 ('fn')
-                       6 LOAD_GLOBAL              0 (Callable)
-                      18 LOAD_GLOBAL              2 (P)
-                      30 LOAD_GLOBAL              4 (R)
-                      42 BUILD_TUPLE              2
-                      44 BINARY_SUBSCR
-                      54 LOAD_CONST               2 ('return')
-                      56 LOAD_GLOBAL              0 (Callable)
-                      68 LOAD_GLOBAL              2 (P)
-                      80 LOAD_GLOBAL              4 (R)
-                      92 BUILD_TUPLE              2
-                      94 BINARY_SUBSCR
-                     104 BUILD_TUPLE              4
-                     106 LOAD_CLOSURE             0 (handle_args)
-                     108 BUILD_TUPLE              1
-                     110 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 152>)
-                     112 MAKE_FUNCTION           12 (annotations, closure)
-                     114 STORE_FAST               1 (decorator)
+         163          10 BUILD_LIST               0
+                      12 STORE_DEREF              0 (decorators)
+         
+         164     >>   14 LOAD_FAST                1 (login_required)
+                      16 POP_JUMP_FORWARD_IF_FALSE    22 (to 62)
+         
+         165          18 LOAD_GLOBAL              1 (NULL + auth_decorators)
+                      30 LOAD_ATTR                1 (login_required)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 BUILD_LIST               1
+                      56 LOAD_DEREF               0 (decorators)
+                      58 LIST_EXTEND              1
+                      60 STORE_DEREF              0 (decorators)
+         
+         167     >>   62 LOAD_CONST               1 ('fn')
+                      64 LOAD_GLOBAL              4 (Callable)
+                      76 LOAD_GLOBAL              6 (P)
+                      88 LOAD_GLOBAL              8 (R)
+                     100 BUILD_TUPLE              2
+                     102 BINARY_SUBSCR
+                     112 LOAD_CONST               2 ('return')
+                     114 LOAD_GLOBAL              4 (Callable)
+                     126 LOAD_GLOBAL              6 (P)
+                     138 LOAD_GLOBAL              8 (R)
+                     150 BUILD_TUPLE              2
+                     152 BINARY_SUBSCR
+                     162 BUILD_TUPLE              4
+                     164 LOAD_CLOSURE             0 (decorators)
+                     166 LOAD_CLOSURE             2 (handle_args)
+                     168 BUILD_TUPLE              2
+                     170 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 167>)
+                     172 MAKE_FUNCTION           12 (annotations, closure)
+                     174 STORE_FAST               3 (decorator)
          
-         168         116 LOAD_FAST                1 (decorator)
-                     118 RETURN_VALUE
+         187         176 LOAD_FAST                3 (decorator)
+                     178 RETURN_VALUE
          consts
             None
             'fn'
             'return'
             code
                argcount  : 1
-               nlocals   : 2
+               nlocals   : 3
                stacksize : 7
                flags     : 19
                code
-                  0x950187009700890272170200740100000000000000000000a6000000ab
-                  0000000000000000008900a6010000ab0100000000000000008a00740300
-                  0000000000000000006a0200000000000000008900a6010000ab01000000
-                  000000000064017406000000000000000000006a04000000000000000064
-                  027406000000000000000000006a0500000000000000006403740c000000
-                  000000000000006606880066016404840ca6000000ab0000000000000000
-                  007d017c015300
-                             0 COPY_FREE_VARS           1
+                  0x950287009700890472170200740100000000000000000000a6000000ab
+                  0000000000000000008900a6010000ab0100000000000000008a00890381
+                  1d7403000000000000000000008903a6010000ab01000000000000000044
+                  005d0d7d0102007c018900a6010000ab0100000000000000008a008c0e74
+                  05000000000000000000006a0300000000000000008900a6010000ab0100
+                  0000000000000064017408000000000000000000006a0500000000000000
+                  0064027408000000000000000000006a0600000000000000006403740e00
+                  0000000000000000006606880066016404840ca6000000ab000000000000
+                  0000007d027c025300
+                             0 COPY_FREE_VARS           2
                              2 MAKE_CELL                0 (fn)
                
-               152           4 RESUME                   0
+               167           4 RESUME                   0
                
-               153           6 LOAD_DEREF               2 (handle_args)
+               168           6 LOAD_DEREF               4 (handle_args)
                              8 POP_JUMP_FORWARD_IF_FALSE    23 (to 56)
                
-               154          10 PUSH_NULL
+               169          10 PUSH_NULL
                             12 LOAD_GLOBAL              1 (NULL + _inject_args)
                             24 PRECALL                  0
                             28 CALL                     0
                             38 LOAD_DEREF               0 (fn)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_DEREF              0 (fn)
                
-               156     >>   56 LOAD_GLOBAL              3 (NULL + functools)
-                            68 LOAD_ATTR                2 (wraps)
-                            78 LOAD_DEREF               0 (fn)
-                            80 PRECALL                  1
-                            84 CALL                     1
-               
-               157          94 LOAD_CONST               1 ('args')
-                            96 LOAD_GLOBAL              6 (P)
-                           108 LOAD_ATTR                4 (args)
-                           118 LOAD_CONST               2 ('kwargs')
-                           120 LOAD_GLOBAL              6 (P)
-                           132 LOAD_ATTR                5 (kwargs)
-                           142 LOAD_CONST               3 ('return')
-                           144 LOAD_GLOBAL             12 (R)
-                           156 BUILD_TUPLE              6
-                           158 LOAD_CLOSURE             0 (fn)
-                           160 BUILD_TUPLE              1
-                           162 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 156>)
-                           164 MAKE_FUNCTION           12 (annotations, closure)
+               171     >>   56 LOAD_DEREF               3 (decorators)
+                            58 POP_JUMP_FORWARD_IF_NONE    29 (to 118)
                
-               156         166 PRECALL                  0
-                           170 CALL                     0
+               172          60 LOAD_GLOBAL              3 (NULL + reversed)
+                            72 LOAD_DEREF               3 (decorators)
+                            74 PRECALL                  1
+                            78 CALL                     1
+                            88 GET_ITER
+                       >>   90 FOR_ITER                13 (to 118)
+                            92 STORE_FAST               1 (d)
+               
+               173          94 PUSH_NULL
+                            96 LOAD_FAST                1 (d)
+                            98 LOAD_DEREF               0 (fn)
+                           100 PRECALL                  1
+                           104 CALL                     1
+                           114 STORE_DEREF              0 (fn)
+                           116 JUMP_BACKWARD           14 (to 90)
+               
+               175     >>  118 LOAD_GLOBAL              5 (NULL + functools)
+                           130 LOAD_ATTR                3 (wraps)
+                           140 LOAD_DEREF               0 (fn)
+                           142 PRECALL                  1
+                           146 CALL                     1
+               
+               176         156 LOAD_CONST               1 ('args')
+                           158 LOAD_GLOBAL              8 (P)
+                           170 LOAD_ATTR                5 (args)
+                           180 LOAD_CONST               2 ('kwargs')
+                           182 LOAD_GLOBAL              8 (P)
+                           194 LOAD_ATTR                6 (kwargs)
+                           204 LOAD_CONST               3 ('return')
+                           206 LOAD_GLOBAL             14 (R)
+                           218 BUILD_TUPLE              6
+                           220 LOAD_CLOSURE             0 (fn)
+                           222 BUILD_TUPLE              1
+                           224 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 175>)
+                           226 MAKE_FUNCTION           12 (annotations, closure)
                
-               157         180 STORE_FAST               1 (inner)
+               175         228 PRECALL                  0
+                           232 CALL                     0
                
-               166         182 LOAD_FAST                1 (inner)
-                           184 RETURN_VALUE
+               176         242 STORE_FAST               2 (inner)
+               
+               185         244 LOAD_FAST                2 (inner)
+                           246 RETURN_VALUE
                consts
                   None
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
@@ -1600,45 +1672,45 @@
                         00000000000000000000000000000000008904a6010000ab010000000000
                         0000000100020089047c0069007c01a4018e017c03a00200000000000000
                         00000000000000000000000000a6000000ab000000000000000000010053
                         0023007c03a0020000000000000000000000000000000000000000a60000
                         00ab00000000000000000001007700780359007701
                                    0 COPY_FREE_VARS           1
                      
-                     156           2 RESUME                   0
+                     175           2 RESUME                   0
                      
-                     158           4 LOAD_FAST                0 (args)
+                     177           4 LOAD_FAST                0 (args)
                                    6 LOAD_CONST               1 (0)
                                    8 BINARY_SUBSCR
                                   18 STORE_FAST               2 (view_request)
                      
-                     159          20 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
+                     178          20 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
                                   32 LOAD_FAST                2 (view_request)
                                   34 PRECALL                  1
                                   38 CALL                     1
                                   48 STORE_FAST               3 (stack)
                      
-                     160          50 NOP
+                     179          50 NOP
                      
-                     161          52 LOAD_FAST                3 (stack)
+                     180          52 LOAD_FAST                3 (stack)
                                   54 LOAD_METHOD              1 (append)
                                   76 LOAD_DEREF               4 (fn)
                                   78 PRECALL                  1
                                   82 CALL                     1
                                   92 POP_TOP
                      
-                     162          94 PUSH_NULL
+                     181          94 PUSH_NULL
                                   96 LOAD_DEREF               4 (fn)
                                   98 LOAD_FAST                0 (args)
                                  100 BUILD_MAP                0
                                  102 LOAD_FAST                1 (kwargs)
                                  104 DICT_MERGE               1
                                  106 CALL_FUNCTION_EX         1
                      
-                     164         108 LOAD_FAST                3 (stack)
+                     183         108 LOAD_FAST                3 (stack)
                                  110 LOAD_METHOD              2 (pop)
                                  132 PRECALL                  0
                                  136 CALL                     0
                                  146 POP_TOP
                                  148 RETURN_VALUE
                              >>  150 PUSH_EXC_INFO
                                  152 LOAD_FAST                3 (stack)
@@ -1658,52 +1730,52 @@
                         0
                      names      ('get_view_fn_call_stack_from_request', 'append', 'pop')
                      varnames   ('args', 'kwargs', 'view_request', 'stack')
                      freevars   ('fn',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 156
+                     firstlineno 175
                      lnotab 0x040210011e0102012a010e02
-               names      ('_inject_args', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
-               varnames   ('fn', 'inner')
-               freevars   ('handle_args',)
+               names      ('_inject_args', 'reversed', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
+               varnames   ('fn', 'd', 'inner')
+               freevars   ('decorators', 'handle_args')
                cellvars   ('fn',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 152
-               lnotab 0x060104012e02260148ff0e010209
-         names      ('Callable', 'P', 'R')
-         varnames   ('handle_args', 'decorator')
+               firstlineno 167
+               lnotab 0x060104012e02040122011802260148ff0e010209
+         names      ('auth_decorators', 'login_required', 'Callable', 'P', 'R')
+         varnames   ('decorators', 'login_required', 'handle_args', 'decorator')
          freevars   ()
-         cellvars   ('handle_args',)
+         cellvars   ('decorators', 'handle_args')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'view'
-         firstlineno 151
-         lnotab 0x04017010
+         firstlineno 156
+         lnotab 0x06060401040104012c027214
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c006401ac02a6020000ab02000000
             00000000007d017c016400750070127403000000000000000000007c01a6
             010000ab01000000000000000064036b02000000005300
-         171           0 RESUME                   0
+         190           0 RESUME                   0
          
-         172           2 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
+         191           2 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
                       14 LOAD_FAST                0 (request)
                       16 LOAD_CONST               1 (False)
                       18 KW_NAMES                 2
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_FAST               1 (stack)
          
-         173          36 LOAD_FAST                1 (stack)
+         192          36 LOAD_FAST                1 (stack)
                       38 LOAD_CONST               0 (None)
                       40 IS_OP                    0
                       42 JUMP_IF_TRUE_OR_POP     18 (to 80)
                       44 LOAD_GLOBAL              3 (NULL + len)
                       56 LOAD_FAST                1 (stack)
                       58 PRECALL                  1
                       62 CALL                     1
@@ -1717,27 +1789,27 @@
             1
          names      ('get_view_fn_call_stack_from_request', 'len')
          varnames   ('request', 'stack')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_view_fn_request_target'
-         firstlineno 171
+         firstlineno 190
          lnotab 0x02012201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         176           0 RESUME                   0
+         195           0 RESUME                   0
          
-         177           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         196           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('HEAD')
@@ -1748,51 +1820,51 @@
             'HEAD'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_head'
-         firstlineno 176
+         firstlineno 195
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         180           0 RESUME                   0
+         199           0 RESUME                   0
          
-         181           2 LOAD_FAST                0 (request)
+         200           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('GET')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'GET'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_get'
-         firstlineno 180
+         firstlineno 199
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         184           0 RESUME                   0
+         203           0 RESUME                   0
          
-         185           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         204           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('POST')
@@ -1803,27 +1875,27 @@
             'POST'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_post'
-         firstlineno 184
+         firstlineno 203
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         188           0 RESUME                   0
+         207           0 RESUME                   0
          
-         189           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         208           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('PUT')
@@ -1834,27 +1906,27 @@
             'PUT'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_put'
-         firstlineno 188
+         firstlineno 207
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         192           0 RESUME                   0
+         211           0 RESUME                   0
          
-         193           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         212           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('PATCH')
@@ -1865,27 +1937,27 @@
             'PATCH'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_patch'
-         firstlineno 192
+         firstlineno 211
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         196           0 RESUME                   0
+         215           0 RESUME                   0
          
-         197           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         216           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('DELETE')
@@ -1896,15 +1968,15 @@
             'DELETE'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_delete'
-         firstlineno 196
+         firstlineno 215
          lnotab 0x0201
       ('auto_param', 'auto_form')
       'auto_param'
       ('get', 'post')
       'auto_form'
       code
          argcount  : 0
@@ -1916,17 +1988,17 @@
             000000740400000000000000000000660219000000000000000000640274
             000000000000000000000074020000000000000000000074040000000000
             000000000066021900000000000000000066048801880066026403840c7d
             027c025300
                        0 MAKE_CELL                0 (auto_param)
                        2 MAKE_CELL                1 (auto_form)
          
-         205           4 RESUME                   0
+         224           4 RESUME                   0
          
-         210           6 LOAD_CONST               1 ('fn')
+         229           6 LOAD_CONST               1 ('fn')
                        8 LOAD_GLOBAL              0 (Callable)
                       20 LOAD_GLOBAL              2 (P)
                       32 LOAD_GLOBAL              4 (R)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('return')
                       58 LOAD_GLOBAL              0 (Callable)
@@ -1934,19 +2006,19 @@
                       82 LOAD_GLOBAL              4 (R)
                       94 BUILD_TUPLE              2
                       96 BINARY_SUBSCR
                      106 BUILD_TUPLE              4
                      108 LOAD_CLOSURE             1 (auto_form)
                      110 LOAD_CLOSURE             0 (auto_param)
                      112 BUILD_TUPLE              2
-                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 210>)
+                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 229>)
                      116 MAKE_FUNCTION           12 (annotations, closure)
                      118 STORE_FAST               2 (decorator)
          
-         235         120 LOAD_FAST                2 (decorator)
+         254         120 LOAD_FAST                2 (decorator)
                      122 RETURN_VALUE
          consts
             None
             'fn'
             'return'
             code
                argcount  : 1
@@ -1966,89 +2038,89 @@
                   04741600000000000000000000660688038800880466036405840ca60000
                   00ab0000000000000000007d027c025300
                              0 COPY_FREE_VARS           2
                              2 MAKE_CELL                0 (fn)
                              4 MAKE_CELL                3 (arg_names)
                              6 MAKE_CELL                4 (injected_params)
                
-               210           8 RESUME                   0
+               229           8 RESUME                   0
                
-               211          10 LOAD_GLOBAL              1 (NULL + list)
+               230          10 LOAD_GLOBAL              1 (NULL + list)
                
-               212          22 LOAD_GLOBAL              3 (NULL + inspect)
+               231          22 LOAD_GLOBAL              3 (NULL + inspect)
                             34 LOAD_ATTR                2 (signature)
                             44 LOAD_DEREF               0 (fn)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 LOAD_ATTR                3 (parameters)
                             70 LOAD_METHOD              4 (values)
                             92 PRECALL                  0
                             96 CALL                     0
                
-               211         106 PRECALL                  1
+               230         106 PRECALL                  1
                            110 CALL                     1
                            120 STORE_FAST               1 (parameters)
                
-               214         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
+               233         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
                
-               215         134 LOAD_DEREF               0 (fn)
+               234         134 LOAD_DEREF               0 (fn)
                            136 LOAD_FAST                1 (parameters)
                            138 LOAD_DEREF               6 (auto_param)
                            140 LOAD_DEREF               5 (auto_form)
                
-               214         142 PRECALL                  4
+               233         142 PRECALL                  4
                            146 CALL                     4
                            156 STORE_DEREF              4 (injected_params)
                
-               217         158 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 217>)
+               236         158 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 236>)
                            160 MAKE_FUNCTION            0
                            162 LOAD_FAST                1 (parameters)
                            164 GET_ITER
                            166 PRECALL                  0
                            170 CALL                     0
                            180 STORE_DEREF              3 (arg_names)
                
-               219         182 LOAD_GLOBAL             13 (NULL + functools)
+               238         182 LOAD_GLOBAL             13 (NULL + functools)
                            194 LOAD_ATTR                7 (wraps)
                            204 LOAD_DEREF               0 (fn)
                            206 PRECALL                  1
                            210 CALL                     1
                
-               220         220 LOAD_CONST               2 ('args')
+               239         220 LOAD_CONST               2 ('args')
                            222 LOAD_GLOBAL             16 (P)
                            234 LOAD_ATTR                9 (args)
                            244 LOAD_CONST               3 ('kwargs')
                            246 LOAD_GLOBAL             16 (P)
                            258 LOAD_ATTR               10 (kwargs)
                            268 LOAD_CONST               4 ('return')
                            270 LOAD_GLOBAL             22 (R)
                            282 BUILD_TUPLE              6
                            284 LOAD_CLOSURE             3 (arg_names)
                            286 LOAD_CLOSURE             0 (fn)
                            288 LOAD_CLOSURE             4 (injected_params)
                            290 BUILD_TUPLE              3
-                           292 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 219>)
+                           292 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 238>)
                            294 MAKE_FUNCTION           12 (annotations, closure)
                
-               219         296 PRECALL                  0
+               238         296 PRECALL                  0
                            300 CALL                     0
                
-               220         310 STORE_FAST               2 (inner)
+               239         310 STORE_FAST               2 (inner)
                
-               233         312 LOAD_FAST                2 (inner)
+               252         312 LOAD_FAST                2 (inner)
                            314 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     217           0 RESUME                   0
+                     236           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (p)
                                   10 LOAD_FAST                1 (p)
                                   12 LOAD_ATTR                0 (name)
                                   22 LIST_APPEND              2
@@ -2057,15 +2129,15 @@
                      consts
                      names      ('name',)
                      varnames   ('.0', 'p')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<listcomp>'
-                     firstlineno 217
+                     firstlineno 236
                      lnotab 0x
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
                      nlocals   : 6
@@ -2083,90 +2155,90 @@
                         020000ab020000000000000000a6010000ab0100000000000000007c017c
                         0319000000000000000000a6020000ab0200000000000000007d057c0581
                         1c740b000000000000000000006a06000000000000000074100000000000
                         00000000007c05a6020000ab0200000000000000006302010053008c8602
                         0089077c0069007c01a4018e015300
                                    0 COPY_FREE_VARS           3
                      
-                     219           2 RESUME                   0
+                     238           2 RESUME                   0
                      
-                     221           4 LOAD_DEREF               6 (arg_names)
+                     240           4 LOAD_DEREF               6 (arg_names)
                                    6 LOAD_CONST               0 (None)
                                    8 LOAD_GLOBAL              1 (NULL + len)
                                   20 LOAD_FAST                0 (args)
                                   22 PRECALL                  1
                                   26 CALL                     1
                                   36 BUILD_SLICE              2
                                   38 BINARY_SUBSCR
                                   48 STORE_FAST               2 (supplied_args)
                      
-                     222          50 LOAD_DEREF               8 (injected_params)
+                     241          50 LOAD_DEREF               8 (injected_params)
                                   52 LOAD_METHOD              1 (items)
                                   74 PRECALL                  0
                                   78 CALL                     0
                                   88 GET_ITER
                              >>   90 FOR_ITER               133 (to 358)
                                   92 UNPACK_SEQUENCE          2
                                   96 STORE_FAST               3 (name)
                                   98 STORE_FAST               4 (ip)
                      
-                     223         100 LOAD_FAST                3 (name)
+                     242         100 LOAD_FAST                3 (name)
                                  102 LOAD_FAST                1 (kwargs)
                                  104 CONTAINS_OP              1
                                  106 POP_JUMP_FORWARD_IF_FALSE   124 (to 356)
                                  108 LOAD_FAST                3 (name)
                                  110 LOAD_FAST                2 (supplied_args)
                                  112 CONTAINS_OP              1
                                  114 POP_JUMP_FORWARD_IF_FALSE   120 (to 356)
                      
-                     224         116 LOAD_FAST                4 (ip)
+                     243         116 LOAD_FAST                4 (ip)
                                  118 LOAD_METHOD              2 (get_value)
                                  140 LOAD_FAST                0 (args)
                                  142 LOAD_FAST                1 (kwargs)
                                  144 PRECALL                  2
                                  148 CALL                     2
                                  158 LOAD_FAST                1 (kwargs)
                                  160 LOAD_FAST                3 (name)
                                  162 STORE_SUBSCR
                      
-                     225         166 LOAD_FAST                4 (ip)
+                     244         166 LOAD_FAST                4 (ip)
                                  168 LOAD_METHOD              3 (replace_response)
                      
-                     226         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
+                     245         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
                                  202 LOAD_GLOBAL             11 (NULL + typing)
                                  214 LOAD_ATTR                6 (cast)
                                  224 LOAD_GLOBAL             14 (Any)
                                  236 LOAD_FAST                0 (args)
                                  238 PRECALL                  2
                                  242 CALL                     2
                                  252 PRECALL                  1
                                  256 CALL                     1
                                  266 LOAD_FAST                1 (kwargs)
                                  268 LOAD_FAST                3 (name)
                                  270 BINARY_SUBSCR
                      
-                     225         280 PRECALL                  2
+                     244         280 PRECALL                  2
                                  284 CALL                     2
                                  294 STORE_FAST               5 (replace_response)
                      
-                     228         296 LOAD_FAST                5 (replace_response)
+                     247         296 LOAD_FAST                5 (replace_response)
                                  298 POP_JUMP_FORWARD_IF_NONE    28 (to 356)
                      
-                     229         300 LOAD_GLOBAL             11 (NULL + typing)
+                     248         300 LOAD_GLOBAL             11 (NULL + typing)
                                  312 LOAD_ATTR                6 (cast)
                                  322 LOAD_GLOBAL             16 (R)
                                  334 LOAD_FAST                5 (replace_response)
                                  336 PRECALL                  2
                                  340 CALL                     2
                                  350 SWAP                     2
                                  352 POP_TOP
                                  354 RETURN_VALUE
                              >>  356 JUMP_BACKWARD          134 (to 90)
                      
-                     231     >>  358 PUSH_NULL
+                     250     >>  358 PUSH_NULL
                                  360 LOAD_DEREF               7 (fn)
                                  362 LOAD_FAST                0 (args)
                                  364 BUILD_MAP                0
                                  366 LOAD_FAST                1 (kwargs)
                                  368 DICT_MERGE               1
                                  370 CALL_FUNCTION_EX         1
                                  372 RETURN_VALUE
@@ -2174,31 +2246,31 @@
                         None
                      names      ('len', 'items', 'get_value', 'replace_response', '_get_request_from_args', 'typing', 'cast', 'Any', 'R')
                      varnames   ('args', 'kwargs', 'supplied_args', 'name', 'ip', 'replace_response')
                      freevars   ('arg_names', 'fn', 'injected_params')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 219
+                     firstlineno 238
                      lnotab 0x04022e0132011001320118015aff100304013a02
                names      ('list', 'inspect', 'signature', 'parameters', 'values', '_extract_injected_params', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
                varnames   ('fn', 'parameters', 'inner')
                freevars   ('auto_form', 'auto_param')
                cellvars   ('fn', 'arg_names', 'injected_params')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 210
+               firstlineno 229
                lnotab 0x0a010c0154ff10030c0108ff1003180226014cff0e01020d
          names      ('Callable', 'P', 'R')
          varnames   ('auto_param', 'auto_form', 'decorator')
          freevars   ()
          cellvars   ('auto_param', 'auto_form')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'inject_args'
-         firstlineno 205
+         firstlineno 224
          lnotab 0x06057219
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
@@ -2207,48 +2279,48 @@
             036a0400000000000000006401ac02a6010000ab0100000000000000005a
             086509650764043c000000020065036a0400000000000000006401ac02a6
             010000ab0100000000000000005a0a650b650c6701650c66021900000000
             0000000000650764053c000000640684005a0d6407650c6408650e650665
             0c6602190000000000000000006409650c6606640a84045a0f640b651064
             0c650c640965116512190000000000000000006606640d84045a13640e53
             00
-         242           0 RESUME                   0
+         261           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParam')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         244          12 PUSH_NULL
+         263          12 PUSH_NULL
                       14 LOAD_NAME                3 (dataclasses)
                       16 LOAD_ATTR                4 (field)
                       26 LOAD_CONST               1 (False)
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (name)
                       46 LOAD_NAME                6 (str)
                       48 LOAD_NAME                7 (__annotations__)
                       50 LOAD_CONST               3 ('name')
                       52 STORE_SUBSCR
          
-         245          56 PUSH_NULL
+         264          56 PUSH_NULL
                       58 LOAD_NAME                3 (dataclasses)
                       60 LOAD_ATTR                4 (field)
                       70 LOAD_CONST               1 (False)
                       72 KW_NAMES                 2
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME               8 (target_type)
                       90 LOAD_NAME                9 (type)
                       92 LOAD_NAME                7 (__annotations__)
                       94 LOAD_CONST               4 ('target_type')
                       96 STORE_SUBSCR
          
-         246         100 PUSH_NULL
+         265         100 PUSH_NULL
                      102 LOAD_NAME                3 (dataclasses)
                      104 LOAD_ATTR                4 (field)
                      114 LOAD_CONST               1 (False)
                      116 KW_NAMES                 2
                      118 PRECALL                  1
                      122 CALL                     1
                      132 STORE_NAME              10 (view_fn)
@@ -2258,49 +2330,49 @@
                      140 LOAD_NAME               12 (Any)
                      142 BUILD_TUPLE              2
                      144 BINARY_SUBSCR
                      154 LOAD_NAME                7 (__annotations__)
                      156 LOAD_CONST               5 ('view_fn')
                      158 STORE_SUBSCR
          
-         248         162 LOAD_CONST               6 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 248>)
+         267         162 LOAD_CONST               6 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 267>)
                      164 MAKE_FUNCTION            0
                      166 STORE_NAME              13 (check)
          
-         251         168 LOAD_CONST               7 ('args')
+         270         168 LOAD_CONST               7 ('args')
                      170 LOAD_NAME               12 (Any)
                      172 LOAD_CONST               8 ('kwargs')
                      174 LOAD_NAME               14 (dict)
                      176 LOAD_NAME                6 (str)
                      178 LOAD_NAME               12 (Any)
                      180 BUILD_TUPLE              2
                      182 BINARY_SUBSCR
                      192 LOAD_CONST               9 ('return')
                      194 LOAD_NAME               12 (Any)
                      196 BUILD_TUPLE              6
-                     198 LOAD_CONST              10 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 251>)
+                     198 LOAD_CONST              10 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 270>)
                      200 MAKE_FUNCTION            4 (annotations)
                      202 STORE_NAME              15 (get_value)
          
-         254         204 LOAD_CONST              11 ('request')
+         273         204 LOAD_CONST              11 ('request')
          
-         255         206 LOAD_NAME               16 (HttpRequest)
+         274         206 LOAD_NAME               16 (HttpRequest)
          
-         254         208 LOAD_CONST              12 ('value')
+         273         208 LOAD_CONST              12 ('value')
          
-         255         210 LOAD_NAME               12 (Any)
+         274         210 LOAD_NAME               12 (Any)
          
-         254         212 LOAD_CONST               9 ('return')
+         273         212 LOAD_CONST               9 ('return')
          
-         256         214 LOAD_NAME               17 (Optional)
+         275         214 LOAD_NAME               17 (Optional)
                      216 LOAD_NAME               18 (HttpResponse)
                      218 BINARY_SUBSCR
          
-         254         228 BUILD_TUPLE              6
-                     230 LOAD_CONST              13 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 254>)
+         273         228 BUILD_TUPLE              6
+                     230 LOAD_CONST              13 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 273>)
                      232 MAKE_FUNCTION            4 (annotations)
                      234 STORE_NAME              19 (replace_response)
                      236 LOAD_CONST              14 (None)
                      238 RETURN_VALUE
          consts
             'InjectedParam'
             False
@@ -2310,81 +2382,81 @@
             'view_fn'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               248           0 RESUME                   0
+               267           0 RESUME                   0
                
-               249           2 LOAD_CONST               0 (None)
+               268           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 248
+               firstlineno 267
                lnotab 0x0201
             'args'
             'kwargs'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               251           0 RESUME                   0
+               270           0 RESUME                   0
                
-               252           2 LOAD_CONST               0 (None)
+               271           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 251
+               firstlineno 270
                lnotab 0x0201
             'request'
             'value'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               254           0 RESUME                   0
+               273           0 RESUME                   0
                
-               257           2 LOAD_CONST               0 (None)
+               276           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'request', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 254
+               firstlineno 273
                lnotab 0x0203
             None
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'name', 'str', '__annotations__', 'target_type', 'type', 'view_fn', 'Callable', 'Any', 'check', 'dict', 'get_value', 'HttpRequest', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParam'
-         firstlineno 242
+         firstlineno 261
          lnotab 0x0c022c012c013e0206032403020102ff020102ff02020efe
       'InjectedParam'
       'view_fn'
       'ip'
       'name'
       'parameter'
       code
@@ -2404,104 +2476,104 @@
             000000741400000000000000000000a6020000ab02000000000000000072
             257c036a0500000000000000006a05000000000000000081197413000000
             000000000000007c036a0500000000000000006a050000000000000000a6
             010000ab0100000000000000006e067416000000000000000000007c015f
             0c00000000000000007c007c015f0d00000000000000007c01a00e000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0001007c015300
-         260           0 RESUME                   0
+         279           0 RESUME                   0
          
-         266           2 LOAD_FAST                2 (name)
+         285           2 LOAD_FAST                2 (name)
                        4 LOAD_FAST                1 (ip)
                        6 STORE_ATTR               0 (name)
          
-         269          16 LOAD_FAST                3 (parameter)
+         288          16 LOAD_FAST                3 (parameter)
                       18 LOAD_ATTR                1 (annotation)
                       28 LOAD_GLOBAL              4 (inspect)
                       40 LOAD_ATTR                3 (Signature)
                       50 LOAD_ATTR                4 (empty)
                       60 IS_OP                    1
                       62 POP_JUMP_FORWARD_IF_FALSE     7 (to 78)
          
-         268          64 LOAD_FAST                3 (parameter)
+         287          64 LOAD_FAST                3 (parameter)
                       66 LOAD_ATTR                1 (annotation)
                       76 JUMP_FORWARD           139 (to 356)
          
-         271     >>   78 LOAD_FAST                3 (parameter)
+         290     >>   78 LOAD_FAST                3 (parameter)
                       80 LOAD_ATTR                5 (default)
                       90 LOAD_GLOBAL              4 (inspect)
                      102 LOAD_ATTR                6 (Parameter)
                      112 LOAD_ATTR                4 (empty)
                      122 IS_OP                    1
                      124 POP_JUMP_FORWARD_IF_FALSE    46 (to 218)
          
-         272         126 LOAD_GLOBAL             15 (NULL + isinstance)
+         291         126 LOAD_GLOBAL             15 (NULL + isinstance)
                      138 LOAD_FAST                3 (parameter)
                      140 LOAD_ATTR                5 (default)
                      150 LOAD_GLOBAL             16 (InjectedParam)
                      162 PRECALL                  2
                      166 CALL                     2
          
-         271         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
+         290         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
          
-         270         178 LOAD_GLOBAL             19 (NULL + type)
+         289         178 LOAD_GLOBAL             19 (NULL + type)
                      190 LOAD_FAST                3 (parameter)
                      192 LOAD_ATTR                5 (default)
                      202 PRECALL                  1
                      206 CALL                     1
                      216 JUMP_FORWARD            69 (to 356)
          
-         274     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
+         293     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
                      230 LOAD_FAST                3 (parameter)
                      232 LOAD_ATTR                5 (default)
                      242 LOAD_GLOBAL             20 (InjectedParamQuery)
                      254 PRECALL                  2
                      258 CALL                     2
          
-         273         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
+         292         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
          
-         275         270 LOAD_FAST                3 (parameter)
+         294         270 LOAD_FAST                3 (parameter)
                      272 LOAD_ATTR                5 (default)
                      282 LOAD_ATTR                5 (default)
                      292 POP_JUMP_FORWARD_IF_NONE    25 (to 344)
          
-         273         294 LOAD_GLOBAL             19 (NULL + type)
+         292         294 LOAD_GLOBAL             19 (NULL + type)
                      306 LOAD_FAST                3 (parameter)
                      308 LOAD_ATTR                5 (default)
                      318 LOAD_ATTR                5 (default)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 JUMP_FORWARD             6 (to 356)
          
-         276     >>  344 LOAD_GLOBAL             22 (str)
+         295     >>  344 LOAD_GLOBAL             22 (str)
          
-         267     >>  356 LOAD_FAST                1 (ip)
+         286     >>  356 LOAD_FAST                1 (ip)
                      358 STORE_ATTR              12 (target_type)
          
-         278         368 LOAD_FAST                0 (view_fn)
+         297         368 LOAD_FAST                0 (view_fn)
                      370 LOAD_FAST                1 (ip)
                      372 STORE_ATTR              13 (view_fn)
          
-         279         382 LOAD_FAST                1 (ip)
+         298         382 LOAD_FAST                1 (ip)
                      384 LOAD_METHOD             14 (check)
                      406 PRECALL                  0
                      410 CALL                     0
                      420 POP_TOP
          
-         280         422 LOAD_FAST                1 (ip)
+         299         422 LOAD_FAST                1 (ip)
                      424 RETURN_VALUE
          consts
             None
          names      ('name', 'annotation', 'inspect', 'Signature', 'empty', 'default', 'Parameter', 'isinstance', 'InjectedParam', 'type', 'InjectedParamQuery', 'str', 'target_type', 'view_fn', 'check')
          varnames   ('view_fn', 'ip', 'name', 'parameter')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_setup_injected_param'
-         firstlineno 260
+         firstlineno 279
          lnotab
             0x02060e0330ff0e03300132ff02ff280432ff020218fe32030cf70c0b0e
             012801
       'parameters'
       'get'
       'post'
       code
@@ -2533,212 +2605,212 @@
             07000000000000000000007c007421000000000000000000007c08ac06a6
             010000ab0100000000000000007c066a0400000000000000007c06a60400
             00ab0400000000000000007c047c066a0400000000000000003c00000090
             018c497c0264086b0200000000722d7407000000000000000000007c0074
             23000000000000000000007c08ac06a6010000ab0100000000000000007c
             066a0400000000000000007c06a6040000ab0400000000000000007c047c
             066a0400000000000000003c00000090018c7e7c045300
-         283           0 RESUME                   0
+         302           0 RESUME                   0
          
-         292           2 BUILD_MAP                0
+         311           2 BUILD_MAP                0
                        4 STORE_FAST               4 (result)
          
-         295           6 LOAD_FAST                1 (parameters)
+         314           6 LOAD_FAST                1 (parameters)
                        8 LOAD_CONST               1 (1)
                       10 LOAD_CONST               2 (None)
                       12 BUILD_SLICE              2
                       14 BINARY_SUBSCR
                       24 STORE_FAST               1 (parameters)
          
-         297          26 LOAD_CONST               3 (False)
+         316          26 LOAD_CONST               3 (False)
                       28 STORE_FAST               5 (found_form_arg)
          
-         298          30 LOAD_FAST                1 (parameters)
+         317          30 LOAD_FAST                1 (parameters)
                       32 GET_ITER
                  >>   34 EXTENDED_ARG             1
                       36 FOR_ITER               380 (to 798)
                       38 STORE_FAST               6 (arg)
          
-         299          40 LOAD_GLOBAL              1 (NULL + isinstance)
+         318          40 LOAD_GLOBAL              1 (NULL + isinstance)
                       52 LOAD_FAST                6 (arg)
                       54 LOAD_ATTR                1 (default)
                       64 LOAD_GLOBAL              4 (InjectedParam)
                       76 PRECALL                  2
                       80 CALL                     2
                       90 POP_JUMP_FORWARD_IF_FALSE    39 (to 170)
          
-         300          92 LOAD_FAST                6 (arg)
+         319          92 LOAD_FAST                6 (arg)
                       94 LOAD_ATTR                1 (default)
                      104 STORE_FAST               7 (ip)
          
-         301         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         320         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
                      118 LOAD_FAST                0 (view_fn)
                      120 LOAD_FAST                7 (ip)
                      122 LOAD_FAST                6 (arg)
                      124 LOAD_ATTR                4 (name)
                      134 LOAD_FAST                6 (arg)
                      136 PRECALL                  4
                      140 CALL                     4
                      150 LOAD_FAST                4 (result)
                      152 LOAD_FAST                7 (ip)
                      154 LOAD_ATTR                4 (name)
                      164 STORE_SUBSCR
                      168 JUMP_BACKWARD           68 (to 34)
          
-         306     >>  170 LOAD_FAST                6 (arg)
+         325     >>  170 LOAD_FAST                6 (arg)
                      172 LOAD_ATTR                1 (default)
                      182 LOAD_GLOBAL             10 (inspect)
                      194 LOAD_ATTR                6 (Parameter)
                      204 LOAD_ATTR                7 (empty)
                      214 COMPARE_OP               3 (!=)
                      220 POP_JUMP_FORWARD_IF_FALSE     7 (to 236)
                      222 LOAD_FAST                6 (arg)
                      224 LOAD_ATTR                1 (default)
                      234 JUMP_FORWARD             1 (to 238)
                  >>  236 LOAD_CONST               2 (None)
          
-         305     >>  238 STORE_FAST               8 (default_value)
+         324     >>  238 STORE_FAST               8 (default_value)
          
-         310         240 LOAD_FAST                3 (auto_form)
+         329         240 LOAD_FAST                3 (auto_form)
          
-         309         242 POP_JUMP_FORWARD_IF_FALSE   120 (to 484)
+         328         242 POP_JUMP_FORWARD_IF_FALSE   120 (to 484)
          
-         311         244 LOAD_GLOBAL              1 (NULL + isinstance)
+         330         244 LOAD_GLOBAL              1 (NULL + isinstance)
                      256 LOAD_FAST                6 (arg)
                      258 LOAD_ATTR                8 (annotation)
                      268 LOAD_GLOBAL             18 (type)
                      280 PRECALL                  2
                      284 CALL                     2
          
-         309         294 POP_JUMP_FORWARD_IF_FALSE    94 (to 484)
+         328         294 POP_JUMP_FORWARD_IF_FALSE    94 (to 484)
          
-         312         296 LOAD_GLOBAL             21 (NULL + issubclass)
+         331         296 LOAD_GLOBAL             21 (NULL + issubclass)
                      308 LOAD_FAST                6 (arg)
                      310 LOAD_ATTR                8 (annotation)
                      320 LOAD_GLOBAL             22 (forms)
                      332 LOAD_ATTR               12 (BaseForm)
                      342 PRECALL                  2
                      346 CALL                     2
          
-         309         356 POP_JUMP_FORWARD_IF_FALSE    63 (to 484)
+         328         356 POP_JUMP_FORWARD_IF_FALSE    63 (to 484)
          
-         314         358 LOAD_FAST                5 (found_form_arg)
+         333         358 LOAD_FAST                5 (found_form_arg)
                      360 POP_JUMP_FORWARD_IF_FALSE    15 (to 392)
          
-         315         362 LOAD_GLOBAL             27 (NULL + Exception)
+         334         362 LOAD_GLOBAL             27 (NULL + Exception)
          
-         316         374 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
+         335         374 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
          
-         315         376 PRECALL                  1
+         334         376 PRECALL                  1
                      380 CALL                     1
                      390 RAISE_VARARGS            1
          
-         318     >>  392 LOAD_CONST               5 (True)
+         337     >>  392 LOAD_CONST               5 (True)
                      394 STORE_FAST               5 (found_form_arg)
          
-         319         396 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         338         396 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         320         408 LOAD_FAST                0 (view_fn)
+         339         408 LOAD_FAST                0 (view_fn)
                      410 LOAD_GLOBAL             29 (NULL + handle_form)
                      422 PRECALL                  0
                      426 CALL                     0
                      436 LOAD_FAST                6 (arg)
                      438 LOAD_ATTR                4 (name)
                      448 LOAD_FAST                6 (arg)
          
-         319         450 PRECALL                  4
+         338         450 PRECALL                  4
                      454 CALL                     4
                      464 LOAD_FAST                4 (result)
                      466 LOAD_FAST                6 (arg)
                      468 LOAD_ATTR                4 (name)
                      478 STORE_SUBSCR
                      482 JUMP_BACKWARD          225 (to 34)
          
-         323     >>  484 LOAD_FAST                2 (auto_param)
+         342     >>  484 LOAD_FAST                2 (auto_param)
                      486 LOAD_CONST               5 (True)
                      488 IS_OP                    0
                      490 POP_JUMP_FORWARD_IF_FALSE    47 (to 586)
          
-         324         492 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         343         492 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         325         504 LOAD_FAST                0 (view_fn)
+         344         504 LOAD_FAST                0 (view_fn)
                      506 LOAD_GLOBAL             31 (NULL + InjectedParamQuery)
                      518 LOAD_FAST                8 (default_value)
                      520 KW_NAMES                 6
                      522 PRECALL                  1
                      526 CALL                     1
                      536 LOAD_FAST                6 (arg)
                      538 LOAD_ATTR                4 (name)
                      548 LOAD_FAST                6 (arg)
          
-         324         550 PRECALL                  4
+         343         550 PRECALL                  4
                      554 CALL                     4
                      564 LOAD_FAST                4 (result)
                      566 LOAD_FAST                6 (arg)
                      568 LOAD_ATTR                4 (name)
                      578 STORE_SUBSCR
                      582 EXTENDED_ARG             1
                      584 JUMP_BACKWARD          276 (to 34)
          
-         327     >>  586 LOAD_FAST                2 (auto_param)
+         346     >>  586 LOAD_FAST                2 (auto_param)
                      588 LOAD_CONST               7 ('get')
                      590 COMPARE_OP               2 (==)
                      596 POP_JUMP_FORWARD_IF_FALSE    47 (to 692)
          
-         328         598 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         347         598 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         329         610 LOAD_FAST                0 (view_fn)
+         348         610 LOAD_FAST                0 (view_fn)
                      612 LOAD_GLOBAL             33 (NULL + InjectedParamQueryGet)
                      624 LOAD_FAST                8 (default_value)
                      626 KW_NAMES                 6
                      628 PRECALL                  1
                      632 CALL                     1
                      642 LOAD_FAST                6 (arg)
                      644 LOAD_ATTR                4 (name)
                      654 LOAD_FAST                6 (arg)
          
-         328         656 PRECALL                  4
+         347         656 PRECALL                  4
                      660 CALL                     4
                      670 LOAD_FAST                4 (result)
                      672 LOAD_FAST                6 (arg)
                      674 LOAD_ATTR                4 (name)
                      684 STORE_SUBSCR
                      688 EXTENDED_ARG             1
                      690 JUMP_BACKWARD          329 (to 34)
          
-         331     >>  692 LOAD_FAST                2 (auto_param)
+         350     >>  692 LOAD_FAST                2 (auto_param)
                      694 LOAD_CONST               8 ('post')
                      696 COMPARE_OP               2 (==)
                      702 POP_JUMP_FORWARD_IF_FALSE    45 (to 794)
          
-         332         704 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         351         704 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         333         716 LOAD_FAST                0 (view_fn)
+         352         716 LOAD_FAST                0 (view_fn)
          
-         334         718 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
+         353         718 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
                      730 LOAD_FAST                8 (default_value)
                      732 KW_NAMES                 6
                      734 PRECALL                  1
                      738 CALL                     1
          
-         335         748 LOAD_FAST                6 (arg)
+         354         748 LOAD_FAST                6 (arg)
                      750 LOAD_ATTR                4 (name)
          
-         336         760 LOAD_FAST                6 (arg)
+         355         760 LOAD_FAST                6 (arg)
          
-         332         762 PRECALL                  4
+         351         762 PRECALL                  4
                      766 CALL                     4
                      776 LOAD_FAST                4 (result)
                      778 LOAD_FAST                6 (arg)
                      780 LOAD_ATTR                4 (name)
                      790 STORE_SUBSCR
                  >>  794 EXTENDED_ARG             1
                      796 JUMP_BACKWARD          382 (to 34)
          
-         339     >>  798 LOAD_FAST                4 (result)
+         358     >>  798 LOAD_FAST                4 (result)
                      800 RETURN_VALUE
          consts
             '\n    Extracts all injected parameters from the given list of function arguments.\n    '
             1
             None
             False
             'You can only have one Form argument in a view function.'
@@ -2748,15 +2820,15 @@
             'post'
          names      ('isinstance', 'default', 'InjectedParam', '_setup_injected_param', 'name', 'inspect', 'Parameter', 'empty', 'annotation', 'type', 'issubclass', 'forms', 'BaseForm', 'Exception', 'handle_form', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost')
          varnames   ('view_fn', 'parameters', 'auto_param', 'auto_form', 'result', 'found_form_arg', 'arg', 'ip', 'default_value')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_extract_injected_params'
-         firstlineno 283
+         firstlineno 302
          lnotab
             0x02090403140204010a0134010e01400544ff020502ff020232fe02033c
             fd020504010c0102ff100304010c012aff220408010c012eff24030c010c
             012eff24030c010c0102011e010c0102fc2407
       code
          argcount  : 0
          nlocals   : 0
@@ -2767,90 +2839,90 @@
             02a6010000ab0100000000000000005a0565066507190000000000000000
             00650864033c000000020065036a0400000000000000006401ac02a60100
             00ab0100000000000000005a09650a650864043c000000020065036a0400
             000000000000006405ac02a6010000ab0100000000000000005a0b650c65
             0864063c000000640784005a0d6408650e6602640984045a0f6408650e66
             02640a84045a10640b650a640c65116507650a6602190000000000000000
             006604640d84045a1264015300
-         347           0 RESUME                   0
+         366           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQuery')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         349          12 PUSH_NULL
+         368          12 PUSH_NULL
                       14 LOAD_NAME                3 (dataclasses)
                       16 LOAD_ATTR                4 (field)
                       26 LOAD_CONST               1 (None)
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (query_param_name)
                       46 LOAD_NAME                6 (Optional)
                       48 LOAD_NAME                7 (str)
                       50 BINARY_SUBSCR
                       60 LOAD_NAME                8 (__annotations__)
                       62 LOAD_CONST               3 ('query_param_name')
                       64 STORE_SUBSCR
          
-         350          68 PUSH_NULL
+         369          68 PUSH_NULL
                       70 LOAD_NAME                3 (dataclasses)
                       72 LOAD_ATTR                4 (field)
                       82 LOAD_CONST               1 (None)
                       84 KW_NAMES                 2
                       86 PRECALL                  1
                       90 CALL                     1
                      100 STORE_NAME               9 (default)
                      102 LOAD_NAME               10 (Any)
                      104 LOAD_NAME                8 (__annotations__)
                      106 LOAD_CONST               4 ('default')
                      108 STORE_SUBSCR
          
-         351         112 PUSH_NULL
+         370         112 PUSH_NULL
                      114 LOAD_NAME                3 (dataclasses)
                      116 LOAD_ATTR                4 (field)
                      126 LOAD_CONST               5 (True)
                      128 KW_NAMES                 2
                      130 PRECALL                  1
                      134 CALL                     1
                      144 STORE_NAME              11 (consume)
                      146 LOAD_NAME               12 (bool)
                      148 LOAD_NAME                8 (__annotations__)
                      150 LOAD_CONST               6 ('consume')
                      152 STORE_SUBSCR
          
-         353         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 353>)
+         372         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 372>)
                      158 MAKE_FUNCTION            0
                      160 STORE_NAME              13 (check)
          
-         357         162 LOAD_CONST               8 ('request')
+         376         162 LOAD_CONST               8 ('request')
                      164 LOAD_NAME               14 (HttpRequest)
                      166 BUILD_TUPLE              2
-                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 357>)
+                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 376>)
                      170 MAKE_FUNCTION            4 (annotations)
                      172 STORE_NAME              15 (_create_lookup_dict)
          
-         364         174 LOAD_CONST               8 ('request')
+         383         174 LOAD_CONST               8 ('request')
                      176 LOAD_NAME               14 (HttpRequest)
                      178 BUILD_TUPLE              2
-                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 364>)
+                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 383>)
                      182 MAKE_FUNCTION            4 (annotations)
                      184 STORE_NAME              16 (_consume_param)
          
-         374         186 LOAD_CONST              11 ('args')
+         393         186 LOAD_CONST              11 ('args')
                      188 LOAD_NAME               10 (Any)
                      190 LOAD_CONST              12 ('kwargs')
                      192 LOAD_NAME               17 (dict)
                      194 LOAD_NAME                7 (str)
                      196 LOAD_NAME               10 (Any)
                      198 BUILD_TUPLE              2
                      200 BINARY_SUBSCR
                      210 BUILD_TUPLE              4
-                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 374>)
+                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 393>)
                      214 MAKE_FUNCTION            4 (annotations)
                      216 STORE_NAME              18 (get_value)
                      218 LOAD_CONST               1 (None)
                      220 RETURN_VALUE
          consts
             'InjectedParamQuery'
             None
@@ -2863,38 +2935,38 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000800e7c006a0100000000000000007c
                   005f0000000000000000006400530064005300
-               353           0 RESUME                   0
+               372           0 RESUME                   0
                
-               354           2 LOAD_FAST                0 (self)
+               373           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 44)
                
-               355          16 LOAD_FAST                0 (self)
+               374          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (name)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               0 (query_param_name)
                             40 LOAD_CONST               0 (None)
                             42 RETURN_VALUE
                
-               354     >>   44 LOAD_CONST               0 (None)
+               373     >>   44 LOAD_CONST               0 (None)
                             46 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 353
+               firstlineno 372
                lnotab 0x02010e011cff
             'request'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -2905,55 +2977,55 @@
                   00000000007d027401000000000000000000006a01000000000000000074
                   04000000000000000000007c016a040000000000000000a6020000ab0200
                   000000000000008a05880566016402840889054400a6000000ab00000000
                   00000000007d037c037c027a0700005300
                              0 MAKE_CELL                4 (getqd)
                              2 MAKE_CELL                5 (postqd)
                
-               357           4 RESUME                   0
+               376           4 RESUME                   0
                
-               358           6 LOAD_GLOBAL              1 (NULL + typing)
+               377           6 LOAD_GLOBAL              1 (NULL + typing)
                             18 LOAD_ATTR                1 (cast)
                             28 LOAD_GLOBAL              4 (QueryDict)
                             40 LOAD_FAST                1 (request)
                             42 LOAD_ATTR                3 (GET)
                             52 PRECALL                  2
                             56 CALL                     2
                             66 STORE_DEREF              4 (getqd)
                
-               359          68 LOAD_CLOSURE             4 (getqd)
+               378          68 LOAD_CLOSURE             4 (getqd)
                             70 BUILD_TUPLE              1
-                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 359>)
+                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 378>)
                             74 MAKE_FUNCTION            8 (closure)
                             76 LOAD_DEREF               4 (getqd)
                             78 GET_ITER
                             80 PRECALL                  0
                             84 CALL                     0
                             94 STORE_FAST               2 (getd)
                
-               360          96 LOAD_GLOBAL              1 (NULL + typing)
+               379          96 LOAD_GLOBAL              1 (NULL + typing)
                            108 LOAD_ATTR                1 (cast)
                            118 LOAD_GLOBAL              4 (QueryDict)
                            130 LOAD_FAST                1 (request)
                            132 LOAD_ATTR                4 (POST)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_DEREF              5 (postqd)
                
-               361         158 LOAD_CLOSURE             5 (postqd)
+               380         158 LOAD_CLOSURE             5 (postqd)
                            160 BUILD_TUPLE              1
-                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 361>)
+                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 380>)
                            164 MAKE_FUNCTION            8 (closure)
                            166 LOAD_DEREF               5 (postqd)
                            168 GET_ITER
                            170 PRECALL                  0
                            174 CALL                     0
                            184 STORE_FAST               3 (postd)
                
-               362         186 LOAD_FAST                3 (postd)
+               381         186 LOAD_FAST                3 (postd)
                            188 LOAD_FAST                2 (getd)
                            190 BINARY_OP                7 (|)
                            194 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
@@ -2962,15 +3034,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     359           2 RESUME                   0
+                     378           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (getqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2983,28 +3055,28 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('getqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 359
+                     firstlineno 378
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     361           2 RESUME                   0
+                     380           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (postqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3017,23 +3089,23 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('postqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 361
+                     firstlineno 380
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET', 'POST')
                varnames   ('self', 'request', 'getd', 'postd')
                freevars   ()
                cellvars   ('getqd', 'postqd')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 357
+               firstlineno 376
                lnotab 0x06013e011c013e011c01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -3043,79 +3115,79 @@
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f010000000000000000640053007c006a0000
                   000000000000007c016a0600000000000000007600723974050000000000
                   00000000007407000000000000000000006a040000000000000000740a00
                   0000000000000000007c016a060000000000000000a6020000ab02000000
                   00000000007c006a000000000000000000a6020000ab0200000000000000
                   007c015f0600000000000000006400530064005300
-               364           0 RESUME                   0
+               383           0 RESUME                   0
                
-               365           2 LOAD_FAST                0 (self)
+               384           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               366          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               385          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               367          42 LOAD_GLOBAL              7 (NULL + typing)
+               386          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               366         114 PRECALL                  2
+               385         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               369     >>  144 LOAD_FAST                0 (self)
+               388     >>  144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                0 (query_param_name)
                            156 LOAD_FAST                1 (request)
                            158 LOAD_ATTR                6 (POST)
                            168 CONTAINS_OP              0
                            170 POP_JUMP_FORWARD_IF_FALSE    57 (to 286)
                
-               370         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               389         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               371         184 LOAD_GLOBAL              7 (NULL + typing)
+               390         184 LOAD_GLOBAL              7 (NULL + typing)
                            196 LOAD_ATTR                4 (cast)
                            206 LOAD_GLOBAL             10 (Any)
                            218 LOAD_FAST                1 (request)
                            220 LOAD_ATTR                6 (POST)
                            230 PRECALL                  2
                            234 CALL                     2
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR                0 (query_param_name)
                
-               370         256 PRECALL                  2
+               389         256 PRECALL                  2
                            260 CALL                     2
                            270 LOAD_FAST                1 (request)
                            272 STORE_ATTR               6 (POST)
                            282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                
-               369     >>  286 LOAD_CONST               0 (None)
+               388     >>  286 LOAD_CONST               0 (None)
                            288 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 364
+               firstlineno 383
                lnotab 0x02011c010c0148ff1e031c010c0148ff1eff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -3130,87 +3202,87 @@
                   0000000000000000007c006a070000000000000000a6020000ab02000000
                   000000000072026400530074110000000000000000000064017c006a0300
                   000000000000009b0064029d03a6010000ab01000000000000000082017c
                   006a09000000000000000072157c00a00a00000000000000000000000000
                   000000000000007c03a6010000ab01000000000000000001007417000000
                   000000000000007c057c006a070000000000000000a6020000ab02000000
                   00000000005300
-               374           0 RESUME                   0
+               393           0 RESUME                   0
                
-               375           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               394           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               376          32 LOAD_FAST                0 (self)
+               395          32 LOAD_FAST                0 (self)
                             34 LOAD_METHOD              1 (_create_lookup_dict)
                             56 LOAD_FAST                3 (request)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               4 (lookup_dict)
                
-               377          74 LOAD_FAST                4 (lookup_dict)
+               396          74 LOAD_FAST                4 (lookup_dict)
                             76 LOAD_METHOD              2 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (query_param_name)
                            110 LOAD_CONST               0 (None)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               5 (values)
                
-               379         128 LOAD_FAST                5 (values)
+               398         128 LOAD_FAST                5 (values)
                            130 POP_JUMP_FORWARD_IF_NOT_NONE    68 (to 268)
                
-               380         132 LOAD_FAST                0 (self)
+               399         132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                4 (default)
                            144 POP_JUMP_FORWARD_IF_NONE     9 (to 164)
                
-               381         146 LOAD_FAST                0 (self)
+               400         146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                4 (default)
                            158 BUILD_LIST               1
                            160 STORE_FAST               5 (values)
                            162 JUMP_FORWARD            52 (to 268)
                
-               382     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
+               401     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
                            176 LOAD_GLOBAL             12 (NoneType)
                            188 LOAD_FAST                0 (self)
                            190 LOAD_ATTR                7 (target_type)
                            200 PRECALL                  2
                            204 CALL                     2
                            214 POP_JUMP_FORWARD_IF_FALSE     2 (to 220)
                
-               383         216 LOAD_CONST               0 (None)
+               402         216 LOAD_CONST               0 (None)
                            218 RETURN_VALUE
                
-               385     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
+               404     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
                
-               386         232 LOAD_CONST               1 ("No value found for request parameter '")
+               405         232 LOAD_CONST               1 ("No value found for request parameter '")
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (query_param_name)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               2 ("'")
                            250 BUILD_STRING             3
                
-               385         252 PRECALL                  1
+               404         252 PRECALL                  1
                            256 CALL                     1
                            266 RAISE_VARARGS            1
                
-               389     >>  268 LOAD_FAST                0 (self)
+               408     >>  268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                9 (consume)
                            280 POP_JUMP_FORWARD_IF_FALSE    21 (to 324)
                
-               390         282 LOAD_FAST                0 (self)
+               409         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD             10 (_consume_param)
                            306 LOAD_FAST                3 (request)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               392     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
+               411     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
                            336 LOAD_FAST                5 (values)
                            338 LOAD_FAST                0 (self)
                            340 LOAD_ATTR                7 (target_type)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 RETURN_VALUE
                consts
@@ -3219,50 +3291,50 @@
                   "'"
                names      ('_get_request_from_args', '_create_lookup_dict', 'get', 'query_param_name', 'default', 'issubclass', 'NoneType', 'target_type', 'Exception', 'consume', '_consume_param', '_convert_value_to_type')
                varnames   ('self', 'args', 'kwargs', 'request', 'lookup_dict', 'values')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 374
+               firstlineno 393
                lnotab 0x02011e012a01360204010e011201340104020c0114ff10040e012a02
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'query_param_name', 'Optional', 'str', '__annotations__', 'default', 'Any', 'consume', 'bool', 'check', 'HttpRequest', '_create_lookup_dict', '_consume_param', 'dict', 'get_value')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQuery'
-         firstlineno 347
+         firstlineno 366
          lnotab 0x0c0238012c012c0206040c070c0a
       'InjectedParamQuery'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640165036602640284045a0464016503660264
             0384045a0564045300
-         395           0 RESUME                   0
+         414           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryGet')
                        8 STORE_NAME               2 (__qualname__)
          
-         397          10 LOAD_CONST               1 ('request')
+         416          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 397>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 416>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         401          22 LOAD_CONST               1 ('request')
+         420          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 401>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 420>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryGet'
             'request'
@@ -3274,28 +3346,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               397           2 RESUME                   0
+               416           2 RESUME                   0
                
-               398           4 LOAD_GLOBAL              1 (NULL + typing)
+               417           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (GET)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               399          66 LOAD_CLOSURE             2 (qd)
+               418          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 399>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 418>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -3307,15 +3379,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     399           2 RESUME                   0
+                     418           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3328,110 +3400,110 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 399
+                     firstlineno 418
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 397
+               firstlineno 416
                lnotab 0x04013e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000760072
                   397405000000000000000000007407000000000000000000006a04000000
                   0000000000740a000000000000000000007c016a010000000000000000a6
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f0100000000000000006400530064005300
-               401           0 RESUME                   0
+               420           0 RESUME                   0
                
-               402           2 LOAD_FAST                0 (self)
+               421           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               403          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               422          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               404          42 LOAD_GLOBAL              7 (NULL + typing)
+               423          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               403         114 PRECALL                  2
+               422         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               402     >>  144 LOAD_CONST               0 (None)
+               421     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 401
+               firstlineno 420
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryGet'
-         firstlineno 395
+         firstlineno 414
          lnotab 0x0a020c04
       'InjectedParamQueryGet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640165036602640284045a0464016503660264
             0384045a0564045300
-         408           0 RESUME                   0
+         427           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryPost')
                        8 STORE_NAME               2 (__qualname__)
          
-         410          10 LOAD_CONST               1 ('request')
+         429          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 410>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 429>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         414          22 LOAD_CONST               1 ('request')
+         433          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 414>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 433>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryPost'
             'request'
@@ -3443,28 +3515,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               410           2 RESUME                   0
+               429           2 RESUME                   0
                
-               411           4 LOAD_GLOBAL              1 (NULL + typing)
+               430           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (POST)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               412          66 LOAD_CLOSURE             2 (qd)
+               431          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 412>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 431>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -3476,15 +3548,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     412           2 RESUME                   0
+                     431           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3497,96 +3569,96 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 412
+                     firstlineno 431
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 410
+               firstlineno 429
                lnotab 0x04013e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000760072
                   397405000000000000000000007407000000000000000000006a04000000
                   0000000000740a000000000000000000007c016a010000000000000000a6
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f0100000000000000006400530064005300
-               414           0 RESUME                   0
+               433           0 RESUME                   0
                
-               415           2 LOAD_FAST                0 (self)
+               434           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (POST)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               416          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               435          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               417          42 LOAD_GLOBAL              7 (NULL + typing)
+               436          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (POST)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               416         114 PRECALL                  2
+               435         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (POST)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               415     >>  144 LOAD_CONST               0 (None)
+               434     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'POST', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 414
+               firstlineno 433
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryPost'
-         firstlineno 408
+         firstlineno 427
          lnotab 0x0a020c04
       'InjectedParamQueryPost'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         421           0 RESUME                   0
+         440           0 RESUME                   0
          
-         422           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
+         441           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -3594,27 +3666,27 @@
             ('default', 'consume')
          names      ('InjectedParamQueryGet',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_get'
-         firstlineno 421
+         firstlineno 440
          lnotab 0x0201
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         425           0 RESUME                   0
+         444           0 RESUME                   0
          
-         426           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
+         445           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -3622,29 +3694,29 @@
             ('default', 'consume')
          names      ('InjectedParamQueryPost',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_post'
-         firstlineno 425
+         firstlineno 444
          lnotab 0x0201
       'default'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007404000000
             000000000000007407000000000000000000007c007c01ac01a6020000ab
             020000000000000000a6020000ab0200000000000000005300
-         429           0 RESUME                   0
+         448           0 RESUME                   0
          
-         430           2 LOAD_GLOBAL              1 (NULL + typing)
+         449           2 LOAD_GLOBAL              1 (NULL + typing)
                       14 LOAD_ATTR                1 (cast)
                       24 LOAD_GLOBAL              4 (T)
                       36 LOAD_GLOBAL              7 (NULL + InjectedParamQuery)
                       48 LOAD_FAST                0 (default)
                       50 LOAD_FAST                1 (consume)
                       52 KW_NAMES                 1
                       54 PRECALL                  2
@@ -3657,15 +3729,15 @@
             ('default', 'consume')
          names      ('typing', 'cast', 'T', 'InjectedParamQuery')
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param'
-         firstlineno 429
+         firstlineno 448
          lnotab 0x0201
       'values'
       'target_type'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 6
@@ -3691,148 +3763,148 @@
             00720264056e0164065300740b0000000000000000000074140000000000
             00000000006a0b00000000000000007c01a6020000ab0200000000000000
             0072147415000000000000000000006a0b00000000000000007c02a60100
             00ab010000000000000000530074190000000000000000000064077c019b
             0064087c029b009d04a6010000ab0100000000000000008201
                        0 MAKE_CELL                3 (list_type)
          
-         433           2 RESUME                   0
+         452           2 RESUME                   0
          
-         435           4 LOAD_GLOBAL              1 (NULL + typing)
+         454           4 LOAD_GLOBAL              1 (NULL + typing)
                       16 LOAD_ATTR                1 (get_origin)
                       26 LOAD_FAST                1 (target_type)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 LOAD_GLOBAL              4 (list)
                       54 COMPARE_OP               2 (==)
                       60 POP_JUMP_FORWARD_IF_FALSE    40 (to 142)
          
-         436          62 LOAD_GLOBAL              1 (NULL + typing)
+         455          62 LOAD_GLOBAL              1 (NULL + typing)
                       74 LOAD_ATTR                3 (get_args)
                       84 LOAD_FAST                1 (target_type)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_CONST               1 (0)
                      102 BINARY_SUBSCR
                      112 STORE_DEREF              3 (list_type)
          
-         437         114 LOAD_CLOSURE             3 (list_type)
+         456         114 LOAD_CLOSURE             3 (list_type)
                      116 BUILD_TUPLE              1
-                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 437>)
+                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 456>)
                      120 MAKE_FUNCTION            8 (closure)
                      122 LOAD_FAST                0 (values)
                      124 GET_ITER
                      126 PRECALL                  0
                      130 CALL                     0
                      140 RETURN_VALUE
          
-         439     >>  142 LOAD_FAST                1 (target_type)
+         458     >>  142 LOAD_FAST                1 (target_type)
                      144 LOAD_GLOBAL              4 (list)
                      156 COMPARE_OP               2 (==)
                      162 POP_JUMP_FORWARD_IF_FALSE    12 (to 188)
          
-         440         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 440>)
+         459         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 459>)
                      166 MAKE_FUNCTION            0
                      168 LOAD_FAST                0 (values)
                      170 GET_ITER
                      172 PRECALL                  0
                      176 CALL                     0
                      186 RETURN_VALUE
          
-         443     >>  188 LOAD_FAST                0 (values)
+         462     >>  188 LOAD_FAST                0 (values)
                      190 LOAD_CONST               1 (0)
                      192 BINARY_SUBSCR
                      202 STORE_FAST               2 (value)
          
-         445         204 LOAD_FAST                2 (value)
+         464         204 LOAD_FAST                2 (value)
                      206 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 210)
          
-         446         208 JUMP_FORWARD           201 (to 612)
+         465         208 JUMP_FORWARD           201 (to 612)
          
-         447     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
+         466     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
                      222 LOAD_FAST                2 (value)
                      224 LOAD_FAST                1 (target_type)
                      226 PRECALL                  2
                      230 CALL                     2
                      240 POP_JUMP_FORWARD_IF_FALSE     2 (to 246)
          
-         448         242 LOAD_FAST                2 (value)
+         467         242 LOAD_FAST                2 (value)
                      244 RETURN_VALUE
          
-         449     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
+         468     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
                      258 LOAD_GLOBAL             12 (str)
                      270 LOAD_FAST                1 (target_type)
                      272 PRECALL                  2
                      276 CALL                     2
                      286 POP_JUMP_FORWARD_IF_FALSE    15 (to 318)
          
-         450         288 LOAD_GLOBAL             13 (NULL + str)
+         469         288 LOAD_GLOBAL             13 (NULL + str)
                      300 LOAD_FAST                2 (value)
                      302 PRECALL                  1
                      306 CALL                     1
                      316 RETURN_VALUE
          
-         451     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
+         470     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
                      330 LOAD_GLOBAL             14 (int)
                      342 LOAD_FAST                1 (target_type)
                      344 PRECALL                  2
                      348 CALL                     2
                      358 POP_JUMP_FORWARD_IF_FALSE    15 (to 390)
          
-         452         360 LOAD_GLOBAL             15 (NULL + int)
+         471         360 LOAD_GLOBAL             15 (NULL + int)
                      372 LOAD_FAST                2 (value)
                      374 PRECALL                  1
                      378 CALL                     1
                      388 RETURN_VALUE
          
-         453     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
+         472     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
                      402 LOAD_GLOBAL             16 (float)
                      414 LOAD_FAST                1 (target_type)
                      416 PRECALL                  2
                      420 CALL                     2
                      430 POP_JUMP_FORWARD_IF_FALSE    15 (to 462)
          
-         454         432 LOAD_GLOBAL             17 (NULL + float)
+         473         432 LOAD_GLOBAL             17 (NULL + float)
                      444 LOAD_FAST                2 (value)
                      446 PRECALL                  1
                      450 CALL                     1
                      460 RETURN_VALUE
          
-         455     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
+         474     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
                      474 LOAD_GLOBAL             18 (bool)
                      486 LOAD_FAST                1 (target_type)
                      488 PRECALL                  2
                      492 CALL                     2
                      502 POP_JUMP_FORWARD_IF_FALSE     8 (to 520)
          
-         456         504 LOAD_FAST                2 (value)
+         475         504 LOAD_FAST                2 (value)
                      506 LOAD_CONST               4 ((False, '', 'false', 'False'))
                      508 CONTAINS_OP              0
                      510 POP_JUMP_FORWARD_IF_FALSE     2 (to 516)
                      512 LOAD_CONST               5 (False)
                      514 JUMP_FORWARD             1 (to 518)
                  >>  516 LOAD_CONST               6 (True)
                  >>  518 RETURN_VALUE
          
-         457     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
+         476     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
                      532 LOAD_GLOBAL             20 (uuid)
                      544 LOAD_ATTR               11 (UUID)
                      554 LOAD_FAST                1 (target_type)
                      556 PRECALL                  2
                      560 CALL                     2
                      570 POP_JUMP_FORWARD_IF_FALSE    20 (to 612)
          
-         458         572 LOAD_GLOBAL             21 (NULL + uuid)
+         477         572 LOAD_GLOBAL             21 (NULL + uuid)
                      584 LOAD_ATTR               11 (UUID)
                      594 LOAD_FAST                2 (value)
                      596 PRECALL                  1
                      600 CALL                     1
                      610 RETURN_VALUE
          
-         460     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
+         479     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
                      624 LOAD_CONST               7 ('Unsupported type: ')
                      626 LOAD_FAST                1 (target_type)
                      628 FORMAT_VALUE             0
                      630 LOAD_CONST               8 (' for value: ')
                      632 LOAD_FAST                2 (value)
                      634 FORMAT_VALUE             0
                      636 BUILD_STRING             4
@@ -3848,15 +3920,15 @@
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d137d017401000000000000000000007c01670189
                   02a6020000ab02000000000000000091028c145300
                              0 COPY_FREE_VARS           1
                
-               437           2 RESUME                   0
+               456           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                19 (to 48)
                             10 STORE_FAST               1 (v)
                             12 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             24 LOAD_FAST                1 (v)
                             26 BUILD_LIST               1
@@ -3869,25 +3941,25 @@
                consts
                names      ('_convert_value_to_type',)
                varnames   ('.0', 'v')
                freevars   ('list_type',)
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 437
+               firstlineno 456
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d187d017401000000000000000000007c016701740200
                   000000000000000000a6020000ab02000000000000000091028c195300
-               440           0 RESUME                   0
+               459           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                24 (to 56)
                              8 STORE_FAST               1 (v)
                             10 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             22 LOAD_FAST                1 (v)
                             24 BUILD_LIST               1
@@ -3900,81 +3972,81 @@
                consts
                names      ('_convert_value_to_type', 'str')
                varnames   ('.0', 'v')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 440
+               firstlineno 459
                lnotab 0x
             (False, '', 'false', 'False')
             False
             True
             'Unsupported type: '
             ' for value: '
          names      ('typing', 'get_origin', 'list', 'get_args', 'isinstance', 'issubclass', 'str', 'int', 'float', 'bool', 'uuid', 'UUID', 'ValueError')
          varnames   ('values', 'target_type', 'value')
          freevars   ()
          cellvars   ('list_type',)
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_convert_value_to_type'
-         firstlineno 433
+         firstlineno 452
          lnotab
             0x04023a0134011c0216011803100204010201200104012a011e012a011e
             012a011e012a01100134012802
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02640184005a0364026504640365056506650466
             02190000000000000000006604640484045a0764056508640665096a0a00
             000000000000006407650b650c190000000000000000006606640884045a
             0d64095300
-         468           0 RESUME                   0
+         487           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamForm')
                        8 STORE_NAME               2 (__qualname__)
          
-         469          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 469>)
+         488          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 488>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (check)
          
-         475          16 LOAD_CONST               2 ('args')
+         494          16 LOAD_CONST               2 ('args')
                       18 LOAD_NAME                4 (Any)
                       20 LOAD_CONST               3 ('kwargs')
                       22 LOAD_NAME                5 (dict)
                       24 LOAD_NAME                6 (str)
                       26 LOAD_NAME                4 (Any)
                       28 BUILD_TUPLE              2
                       30 BINARY_SUBSCR
                       40 BUILD_TUPLE              4
-                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 475>)
+                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 494>)
                       44 MAKE_FUNCTION            4 (annotations)
                       46 STORE_NAME               7 (get_value)
          
-         487          48 LOAD_CONST               5 ('request')
+         506          48 LOAD_CONST               5 ('request')
          
-         488          50 LOAD_NAME                8 (HttpRequest)
+         507          50 LOAD_NAME                8 (HttpRequest)
          
-         487          52 LOAD_CONST               6 ('value')
+         506          52 LOAD_CONST               6 ('value')
          
-         488          54 LOAD_NAME                9 (forms)
+         507          54 LOAD_NAME                9 (forms)
                       56 LOAD_ATTR               10 (Form)
          
-         487          66 LOAD_CONST               7 ('return')
+         506          66 LOAD_CONST               7 ('return')
          
-         489          68 LOAD_NAME               11 (Optional)
+         508          68 LOAD_NAME               11 (Optional)
                       70 LOAD_NAME               12 (HttpResponse)
                       72 BINARY_SUBSCR
          
-         487          82 BUILD_TUPLE              6
-                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 487>)
+         506          82 BUILD_TUPLE              6
+                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 506>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              13 (replace_response)
                       90 LOAD_CONST               9 (None)
                       92 RETURN_VALUE
          consts
             'InjectedParamForm'
             code
@@ -3983,49 +4055,49 @@
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000740400
                   0000000000000000006a030000000000000000a6020000ab020000000000
                   000000731774090000000000000000000064017c006a0100000000000000
                   009b009d02a6010000ab010000000000000000820164005300
-               469           0 RESUME                   0
+               488           0 RESUME                   0
                
-               470           2 LOAD_GLOBAL              1 (NULL + issubclass)
+               489           2 LOAD_GLOBAL              1 (NULL + issubclass)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (target_type)
                             26 LOAD_GLOBAL              4 (forms)
                             38 LOAD_ATTR                3 (BaseForm)
                             48 PRECALL                  2
                             52 CALL                     2
                             62 POP_JUMP_FORWARD_IF_TRUE    23 (to 110)
                
-               471          64 LOAD_GLOBAL              9 (NULL + Exception)
+               490          64 LOAD_GLOBAL              9 (NULL + Exception)
                
-               472          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
+               491          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                1 (target_type)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             2
                
-               471          94 PRECALL                  1
+               490          94 PRECALL                  1
                             98 CALL                     1
                            108 RAISE_VARARGS            1
                
-               470     >>  110 LOAD_CONST               0 (None)
+               489     >>  110 LOAD_CONST               0 (None)
                            112 RETURN_VALUE
                consts
                   None
                   'argument type for handle_form() must be a subclass of django.forms.BaseForm, got '
                names      ('issubclass', 'target_type', 'forms', 'BaseForm', 'Exception')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 469
+               firstlineno 488
                lnotab 0x02013e010c0112ff10ff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -4042,99 +4114,99 @@
                   0000000000000000007d057c05a00a000000000000000000000000000000
                   00000000007417000000000000000000006a0c00000000000000007c036a
                   0d0000000000000000a6010000ab010000000000000000a6010000ab0100
                   0000000000000001007c00a0020000000000000000000000000000000000
                   0000007c05ac03a6010000ab0100000000000000007d046e147c00a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007d047c045300
-               475           0 RESUME                   0
+               494           0 RESUME                   0
                
-               476           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               495           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               477          32 LOAD_GLOBAL              3 (NULL + is_post)
+               496          32 LOAD_GLOBAL              3 (NULL + is_post)
                             44 LOAD_FAST                3 (request)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 POP_JUMP_FORWARD_IF_FALSE    34 (to 130)
                
-               478          62 LOAD_FAST                0 (self)
+               497          62 LOAD_FAST                0 (self)
                             64 LOAD_METHOD              2 (target_type)
                             86 LOAD_FAST                3 (request)
                             88 LOAD_ATTR                3 (POST)
                             98 LOAD_FAST                3 (request)
                            100 LOAD_ATTR                4 (FILES)
                            110 KW_NAMES                 1
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               4 (form)
                            128 JUMP_FORWARD           147 (to 424)
                
-               479     >>  130 LOAD_FAST                3 (request)
+               498     >>  130 LOAD_FAST                3 (request)
                            132 LOAD_ATTR                5 (content_type)
                            142 LOAD_CONST               2 ('application/json')
                            144 COMPARE_OP               2 (==)
                            150 POP_JUMP_FORWARD_IF_FALSE   116 (to 384)
                
-               480         152 LOAD_GLOBAL             13 (NULL + typing)
+               499         152 LOAD_GLOBAL             13 (NULL + typing)
                            164 LOAD_ATTR                7 (cast)
                            174 LOAD_GLOBAL             16 (QueryDict)
                            186 LOAD_FAST                3 (request)
                            188 LOAD_ATTR                3 (POST)
                            198 PRECALL                  2
                            202 CALL                     2
                            212 LOAD_METHOD              9 (copy)
                            234 PRECALL                  0
                            238 CALL                     0
                            248 STORE_FAST               5 (new_post_dict)
                
-               481         250 LOAD_FAST                5 (new_post_dict)
+               500         250 LOAD_FAST                5 (new_post_dict)
                            252 LOAD_METHOD             10 (update)
                            274 LOAD_GLOBAL             23 (NULL + json)
                            286 LOAD_ATTR               12 (loads)
                            296 LOAD_FAST                3 (request)
                            298 LOAD_ATTR               13 (body)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 PRECALL                  1
                            326 CALL                     1
                            336 POP_TOP
                
-               482         338 LOAD_FAST                0 (self)
+               501         338 LOAD_FAST                0 (self)
                            340 LOAD_METHOD              2 (target_type)
                            362 LOAD_FAST                5 (new_post_dict)
                            364 KW_NAMES                 3
                            366 PRECALL                  1
                            370 CALL                     1
                            380 STORE_FAST               4 (form)
                            382 JUMP_FORWARD            20 (to 424)
                
-               484     >>  384 LOAD_FAST                0 (self)
+               503     >>  384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD              2 (target_type)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 STORE_FAST               4 (form)
                
-               485     >>  424 LOAD_FAST                4 (form)
+               504     >>  424 LOAD_FAST                4 (form)
                            426 RETURN_VALUE
                consts
                   None
                   ('data', 'files')
                   'application/json'
                   ('data',)
                names      ('_get_request_from_args', 'is_post', 'target_type', 'POST', 'FILES', 'content_type', 'typing', 'cast', 'QueryDict', 'copy', 'update', 'json', 'loads', 'body')
                varnames   ('self', 'args', 'kwargs', 'request', 'form', 'new_post_dict')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 475
+               firstlineno 494
                lnotab 0x02011e011e0144011601620158012e022801
             'request'
             'value'
             'return'
             code
                argcount  : 3
                nlocals   : 7
@@ -4153,243 +4225,244 @@
                   0000000000a6010000ab0100000000000000007c066a0b00000000000000
                   0064049c037c047c056a0a00000000000000003c0000008c557419000000
                   000000000000007c037c047413000000000000000000007c02a00d000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00a6010000ab0100000000000000007c02a0040000000000000000000000
                   000000000000000000a6000000ab00000000000000000064059c04a60100
                   00ab010000000000000000530064005300
-               487           0 RESUME                   0
+               506           0 RESUME                   0
                
-               490           2 LOAD_GLOBAL              1 (NULL + is_patch)
+               509           2 LOAD_GLOBAL              1 (NULL + is_patch)
                             14 LOAD_FAST                1 (request)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 POP_JUMP_FORWARD_IF_FALSE   215 (to 462)
                             32 LOAD_FAST                1 (request)
                             34 LOAD_ATTR                1 (content_type)
                             44 LOAD_CONST               1 ('application/json')
                             46 COMPARE_OP               2 (==)
                             52 POP_JUMP_FORWARD_IF_FALSE   204 (to 462)
                
-               491          54 LOAD_FAST                1 (request)
+               510          54 LOAD_FAST                1 (request)
                             56 LOAD_ATTR                2 (headers)
                             66 LOAD_METHOD              3 (get)
                             88 LOAD_CONST               2 ('X-DFV-Validate-Field')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 STORE_FAST               3 (validate_field)
                
-               492         106 LOAD_FAST                2 (value)
+               511         106 LOAD_FAST                2 (value)
                            108 LOAD_METHOD              4 (is_valid)
                            130 PRECALL                  0
                            134 CALL                     0
                            144 POP_TOP
                
-               493         146 BUILD_MAP                0
+               512         146 BUILD_MAP                0
                            148 STORE_FAST               4 (fields)
                
-               494         150 LOAD_FAST                2 (value)
+               513         150 LOAD_FAST                2 (value)
                            152 GET_ITER
                        >>  154 FOR_ITER                84 (to 324)
                            156 STORE_FAST               5 (bound_field)
                
-               495         158 LOAD_FAST                5 (bound_field)
+               514         158 LOAD_FAST                5 (bound_field)
                            160 LOAD_ATTR                5 (field)
                            170 LOAD_ATTR                6 (widget)
                            180 STORE_FAST               6 (widget)
                
-               497         182 LOAD_GLOBAL             15 (NULL + len)
+               516         182 LOAD_GLOBAL             15 (NULL + len)
                            194 LOAD_FAST                5 (bound_field)
                            196 LOAD_ATTR                8 (errors)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 LOAD_CONST               3 (0)
                            222 COMPARE_OP               2 (==)
                
-               498         228 LOAD_GLOBAL             19 (NULL + str)
+               517         228 LOAD_GLOBAL             19 (NULL + str)
                            240 LOAD_FAST                2 (value)
                            242 LOAD_FAST                5 (bound_field)
                            244 LOAD_ATTR               10 (name)
                            254 BINARY_SUBSCR
                            264 LOAD_ATTR                8 (errors)
                            274 PRECALL                  1
                            278 CALL                     1
                
-               499         288 LOAD_FAST                6 (widget)
+               518         288 LOAD_FAST                6 (widget)
                            290 LOAD_ATTR               11 (attrs)
                
-               496         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
+               515         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
                            302 BUILD_CONST_KEY_MAP      3
                            304 LOAD_FAST                4 (fields)
                            306 LOAD_FAST                5 (bound_field)
                            308 LOAD_ATTR               10 (name)
                            318 STORE_SUBSCR
                            322 JUMP_BACKWARD           85 (to 154)
                
-               502     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
+               521     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
                
-               504         336 LOAD_FAST                3 (validate_field)
+               523         336 LOAD_FAST                3 (validate_field)
                
-               505         338 LOAD_FAST                4 (fields)
+               524         338 LOAD_FAST                4 (fields)
                
-               506         340 LOAD_GLOBAL             19 (NULL + str)
+               525         340 LOAD_GLOBAL             19 (NULL + str)
                            352 LOAD_FAST                2 (value)
                            354 LOAD_METHOD             13 (non_field_errors)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 PRECALL                  1
                            394 CALL                     1
                
-               507         404 LOAD_FAST                2 (value)
+               526         404 LOAD_FAST                2 (value)
                            406 LOAD_METHOD              4 (is_valid)
                            428 PRECALL                  0
                            432 CALL                     0
                
-               503         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
+               522         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
                            444 BUILD_CONST_KEY_MAP      4
                
-               502         446 PRECALL                  1
+               521         446 PRECALL                  1
                            450 CALL                     1
                            460 RETURN_VALUE
                
-               511     >>  462 LOAD_CONST               0 (None)
+               530     >>  462 LOAD_CONST               0 (None)
                            464 RETURN_VALUE
                consts
                   None
                   'application/json'
                   'X-DFV-Validate-Field'
                   0
                   ('valid', 'errors', 'attrs')
                   ('name', 'fields', 'non_field_errors', 'form_valid')
                names      ('is_patch', 'content_type', 'headers', 'get', 'is_valid', 'field', 'widget', 'len', 'errors', 'str', 'name', 'attrs', 'JsonResponse', 'non_field_errors')
                varnames   ('self', 'request', 'value', 'validate_field', 'fields', 'bound_field', 'widget')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 487
+               firstlineno 506
                lnotab
                   0x02033401340128010401080118022e013c010cfd18060c020201020140
                   0126fc04ff1009
             None
          names      ('__name__', '__module__', '__qualname__', 'check', 'Any', 'dict', 'str', 'get_value', 'HttpRequest', 'forms', 'Form', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamForm'
-         firstlineno 468
+         firstlineno 487
          lnotab 0x0a010606200c020102ff02010cff02020efe
       'InjectedParamForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000053
             00
-         514           0 RESUME                   0
+         533           0 RESUME                   0
          
-         515           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
+         534           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 RETURN_VALUE
          consts
             None
          names      ('InjectedParamForm',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'handle_form'
-         firstlineno 514
+         firstlineno 533
          lnotab 0x0201
       'querydict'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401ac02a6010000ab010000000000
             0000007d027c02a00100000000000000000000000000000000000000007c
             00a6010000ab01000000000000000001007c027c013d007c025300
-         523           0 RESUME                   0
+         542           0 RESUME                   0
          
-         524           2 LOAD_GLOBAL              1 (NULL + QueryDict)
+         543           2 LOAD_GLOBAL              1 (NULL + QueryDict)
                       14 LOAD_CONST               1 (True)
                       16 KW_NAMES                 2
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               2 (temp)
          
-         525          34 LOAD_FAST                2 (temp)
+         544          34 LOAD_FAST                2 (temp)
                       36 LOAD_METHOD              1 (update)
                       58 LOAD_FAST                0 (querydict)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_TOP
          
-         526          76 LOAD_FAST                2 (temp)
+         545          76 LOAD_FAST                2 (temp)
                       78 LOAD_FAST                1 (key)
                       80 DELETE_SUBSCR
          
-         527          82 LOAD_FAST                2 (temp)
+         546          82 LOAD_FAST                2 (temp)
                       84 RETURN_VALUE
          consts
             None
             True
             ('mutable',)
          names      ('QueryDict', 'update')
          varnames   ('querydict', 'key', 'temp')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'querydict_key_removed'
-         firstlineno 523
+         firstlineno 542
          lnotab 0x020120012a010601
       'args'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006401190000000000000000005300
-         530           0 RESUME                   0
+         549           0 RESUME                   0
          
-         531           2 LOAD_FAST                0 (args)
+         550           2 LOAD_FAST                0 (args)
                        4 LOAD_CONST               1 (0)
                        6 BINARY_SUBSCR
                       16 RETURN_VALUE
          consts
             None
             0
          names      ()
          varnames   ('args',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_get_request_from_args'
-         firstlineno 530
+         firstlineno 549
          lnotab 0x0201
       (None,)
       ('outerHTML',)
       (True,)
       (None, True)
-   names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'element', 'swap_oob', 'overload', 'list', 'get_view_fn_call_stack_from_request', 'bool', 'view', 'is_view_fn_request_target', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete', 'inject_args', '_inject_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'dict', '_extract_injected_params', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', '_get_request_from_args')
+   names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'list', 'element', 'swap_oob', 'overload', 'get_view_fn_call_stack_from_request', 'bool', 'view', 'is_view_fn_request_target', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete', 'inject_args', '_inject_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'dict', '_extract_injected_params', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', '_get_request_from_args')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c012002080108010c010c0118
       010c0110021601160116082621160902ff02030201020102010201020102
-      f806010eff02060efa020934f7082902ff040102ff020102ff020202fe08
-      150c011aff0e0102040c01020102ff020102ff02021afe06ff0e01020702
-      ff040102ff02021afe080940140c050c040c040c040c040c040c0b020102
-      fd060214fe020314fd020434fc082204030c0118ff0e010211020114ff02
-      0202fe020302fd02040cfc081b02fc040114ff020218fe020326fd020414
-      fc020512fb08400c011aff0e01022f0c011aff0e01020c0c011aff0e0102
-      0c0e040e04340426231c2e0c091007
+      0102f706010eff02060efa02081af8020a34f6082e02ff040102ff020102
+      ff020202fe08150c011aff0e0102040c01020102ff020102ff02021afe06
+      ff0e01020702ff040102ff02021afe080b0201020102fc06021afe020534
+      fb08220c050c040c040c040c040c040c0b020102fd060214fe020314fd02
+      0434fc082204030c0118ff0e010211020114ff020202fe020302fd02040c
+      fc081b02fc040114ff020218fe020326fd020414fc020512fb08400c011a
+      ff0e01022f0c011aff0e01020c0c011aff0e01020c0e040e04340426231c
+      2e0c091007
```

### Comparing `dfv-0.7.0/dfv/__pycache__/test_element.cpython-311.pyc` & `dfv-0.8.0/dfv/__pycache__/test_element.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/__pycache__/test_form.cpython-311.pyc` & `dfv-0.8.0/dfv/__pycache__/test_form.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc` & `dfv-0.8.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/__pycache__/test_view.cpython-311.pyc` & `dfv-0.8.0/dfv/__pycache__/test_view.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/static/dfv.js` & `dfv-0.8.0/dfv/static/dfv.js`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc` & `dfv-0.8.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/test_element.py` & `dfv-0.8.0/dfv/test_element.py`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/test_form.py` & `dfv-0.8.0/dfv/test_form.py`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/test_params_to_args.py` & `dfv-0.8.0/dfv/test_params_to_args.py`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/dfv/test_view.py` & `dfv-0.8.0/dfv/test_view.py`

 * *Files identical despite different names*

### Comparing `dfv-0.7.0/pyproject.toml` & `dfv-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfv"
-version = "0.7.0"
+version = "0.8.0"
 description = "Django Function Views"
 authors = ["Roman Roelofsen <romanroe@gmail.com>"]
 include = ["dfv"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 django = "^4.1.7"
```

### Comparing `dfv-0.7.0/setup.py` & `dfv-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'django>=4.1.7,<5.0.0',
  'lxml>=4.9.2,<5.0.0',
  'typeguard',
  'wrapt>=1.15.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'dfv',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'Django Function Views',
     'long_description': 'None',
     'author': 'Roman Roelofsen',
     'author_email': 'romanroe@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dfv-0.7.0/PKG-INFO` & `dfv-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfv
-Version: 0.7.0
+Version: 0.8.0
 Summary: Django Function Views
 Author: Roman Roelofsen
 Author-email: romanroe@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

