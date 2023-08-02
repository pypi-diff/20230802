# Comparing `tmp/dfv-0.6.0.tar.gz` & `tmp/dfv-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfv-0.6.0.tar", max compression
+gzip compressed data, was "dfv-0.7.0.tar", max compression
```

## Comparing `dfv-0.6.0.tar` & `dfv-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    15349 2023-07-31 19:10:30.998195 dfv-0.6.0/dfv/__init__.py
--rw-r--r--   0        0        0    25559 2023-07-31 19:10:42.642339 dfv-0.6.0/dfv/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10456 2023-07-31 19:21:19.730323 dfv-0.6.0/dfv/__pycache__/test_element.cpython-311.pyc
--rw-r--r--   0        0        0     8642 2023-07-29 08:01:02.515193 dfv-0.6.0/dfv/__pycache__/test_form.cpython-311.pyc
--rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.6.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
--rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.6.0/dfv/static/dfv.js
--rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.6.0/dfv/templates/dfv/tests/TemplateResponse.html
--rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.6.0/dfv/templatetags/__init__.py
--rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.6.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.6.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
--rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.6.0/dfv/templatetags/dfv.py
--rw-r--r--   0        0        0     4328 2023-07-31 19:19:29.401041 dfv-0.6.0/dfv/test_element.py
--rw-r--r--   0        0        0     3340 2023-07-29 08:01:00.971175 dfv-0.6.0/dfv/test_form.py
--rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.6.0/dfv/test_params_to_args.py
--rw-r--r--   0        0        0     1438 2023-07-31 19:21:01.298109 dfv-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.6.0/setup.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    17371 2023-08-02 19:53:41.847374 dfv-0.7.0/dfv/__init__.py
+-rw-r--r--   0        0        0    28620 2023-08-02 19:53:44.291403 dfv-0.7.0/dfv/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10456 2023-07-31 19:21:19.730323 dfv-0.7.0/dfv/__pycache__/test_element.cpython-311.pyc
+-rw-r--r--   0        0        0     8642 2023-07-29 08:01:02.515193 dfv-0.7.0/dfv/__pycache__/test_form.cpython-311.pyc
+-rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.7.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
+-rw-r--r--   0        0        0     4496 2023-08-02 19:49:36.096341 dfv-0.7.0/dfv/__pycache__/test_view.cpython-311.pyc
+-rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.7.0/dfv/static/dfv.js
+-rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.7.0/dfv/templates/dfv/tests/TemplateResponse.html
+-rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.7.0/dfv/templatetags/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.7.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.7.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
+-rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.7.0/dfv/templatetags/dfv.py
+-rw-r--r--   0        0        0     4328 2023-07-31 19:19:29.401041 dfv-0.7.0/dfv/test_element.py
+-rw-r--r--   0        0        0     3340 2023-07-29 08:01:00.971175 dfv-0.7.0/dfv/test_form.py
+-rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.7.0/dfv/test_params_to_args.py
+-rw-r--r--   0        0        0     1646 2023-08-02 19:49:35.828337 dfv-0.7.0/dfv/test_view.py
+-rw-r--r--   0        0        0     1438 2023-08-01 20:43:58.184518 dfv-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.7.0/setup.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.7.0/PKG-INFO
```

### Comparing `dfv-0.6.0/dfv/__init__.py` & `dfv-0.7.0/dfv/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,17 +74,15 @@
     hx_swap="outerHTML",
     classes: Optional[str] = None,
     handle_args=True,
     login_required=False,
 ) -> Callable[[Callable[P, R]], Callable[P, R]]:
     def decorator(f: Callable[P, HttpResponse]) -> Callable[P, HttpResponse]:
         id = element_id if isinstance(element_id, str) else f.__name__
-
-        if handle_args:
-            f = _inject_args()(f)
+        f = view(handle_args)(f)
 
         if login_required:
             f = auth_decorators.login_required()(f)
 
         @functools.wraps(f)
         def inner(*args: P.args, **kwargs: P.kwargs) -> HttpResponse:
             response = f(*args, **kwargs)
@@ -121,28 +119,105 @@
 
     parsed.attrib["hx-swap-oob"] = f"{hx_swap_oob_method}:#{id}"
     response.content += lxml.html.tostring(parsed)
     return response
 
 
 ################################################################################
+### view
+################################################################################
+
+
+@typing.overload
+def get_view_fn_call_stack_from_request(request: HttpRequest) -> list[Callable]:
+    ...
+
+
+@typing.overload
+def get_view_fn_call_stack_from_request(
+    request: HttpRequest, create: bool
+) -> Optional[list[Callable]]:
+    ...
+
+
+def get_view_fn_call_stack_from_request(
+    request: HttpRequest, create=True
+) -> Optional[list[Callable]]:
+    call_stack = getattr(request, "__dfv_view_fn_call_stack", None)
+    call_stack = [] if call_stack is None and create else call_stack
+    setattr(request, "__dfv_view_fn_call_stack", call_stack)
+    return call_stack
+
+
+def view(handle_args=True) -> Callable[[Callable[P, R]], Callable[P, R]]:
+    def decorator(fn: Callable[P, R]) -> Callable[P, R]:
+        if handle_args:
+            fn = _inject_args()(fn)
+
+        @functools.wraps(fn)
+        def inner(*args: P.args, **kwargs: P.kwargs) -> R:
+            view_request: HttpRequest = args[0]
+            stack = get_view_fn_call_stack_from_request(view_request)
+            try:
+                stack.append(fn)
+                return fn(*args, **kwargs)
+            finally:
+                stack.pop()
+
+        return inner
+
+    return decorator
+
+
+def is_view_fn_request_target(request: HttpRequest):
+    stack = get_view_fn_call_stack_from_request(request, create=False)
+    return stack is None or len(stack) == 1
+
+
+def is_head(request: HttpRequest):
+    return is_view_fn_request_target(request) and request.method == "HEAD"
+
+
+def is_get(request: HttpRequest):
+    return request.method == "GET"
+
+
+def is_post(request: HttpRequest):
+    return is_view_fn_request_target(request) and request.method == "POST"
+
+
+def is_put(request: HttpRequest):
+    return is_view_fn_request_target(request) and request.method == "PUT"
+
+
+def is_patch(request: HttpRequest):
+    return is_view_fn_request_target(request) and request.method == "PATCH"
+
+
+def is_delete(request: HttpRequest):
+    return is_view_fn_request_target(request) and request.method == "DELETE"
+
+
+################################################################################
 ### inject_args
 ################################################################################
 
 
 def inject_args(
     *,
     auto_param: bool | Literal["get", "post"] = False,
     auto_form: Optional[bool | str] = True,
 ) -> Callable[[Callable[P, R]], Callable[P, R]]:
     def decorator(fn: Callable[P, R]) -> Callable[P, R]:
         parameters: list[inspect.Parameter] = list(
             inspect.signature(fn).parameters.values()
         )
-        injected_params = _extract_injected_params(parameters, auto_param, auto_form)
+        injected_params = _extract_injected_params(
+            fn, parameters, auto_param, auto_form
+        )
         arg_names = [p.name for p in parameters]
 
         @functools.wraps(fn)
         def inner(*args: P.args, **kwargs: P.kwargs) -> R:
             supplied_args = arg_names[: len(args)]
             for name, ip in injected_params.items():
                 if name not in kwargs and name not in supplied_args:
@@ -164,45 +239,53 @@
 _inject_args = inject_args
 
 
 @dataclasses.dataclass
 class InjectedParam:
     name: str = dataclasses.field(init=False)
     target_type: type = dataclasses.field(init=False)
+    view_fn: Callable[[Any], Any] = dataclasses.field(init=False)
 
     def check(self):
         pass
 
     def get_value(self, args: Any, kwargs: dict[str, Any]) -> Any:
         pass
 
     def replace_response(
         self, request: HttpRequest, value: Any
     ) -> Optional[HttpResponse]:
         pass
 
 
-def _setup_injected_param(ip: InjectedParam, name: str, parameter: inspect.Parameter):
+def _setup_injected_param(
+    view_fn: Callable[[Any], Any],
+    ip: InjectedParam,
+    name: str,
+    parameter: inspect.Parameter,
+):
     ip.name = name
     ip.target_type = (
         parameter.annotation
         if parameter.annotation is not inspect.Signature.empty
         else type(parameter.default)
         if parameter.default is not inspect.Parameter.empty
         and not isinstance(parameter.default, InjectedParam)
         else type(parameter.default.default)
         if isinstance(parameter.default, InjectedParamQuery)
         and parameter.default.default is not None
         else str
     )
+    ip.view_fn = view_fn
     ip.check()
     return ip
 
 
 def _extract_injected_params(
+    view_fn: Callable[[Any], Any],
     parameters: list[inspect.Parameter],
     auto_param: bool | Literal["get"] | Literal["post"],
     auto_form: Optional[bool | str] = True,
 ) -> dict[str, InjectedParam]:
     """
     Extracts all injected parameters from the given list of function arguments.
     """
@@ -211,15 +294,15 @@
     # skip first request parameter
     parameters = parameters[1:]
 
     found_form_arg = False
     for arg in parameters:
         if isinstance(arg.default, InjectedParam):
             ip: InjectedParam = arg.default
-            result[ip.name] = _setup_injected_param(ip, arg.name, arg)
+            result[ip.name] = _setup_injected_param(view_fn, ip, arg.name, arg)
 
         # elif arg.default == inspect.Parameter.empty:
         else:
             default_value = (
                 arg.default if arg.default != inspect.Parameter.empty else None
             )
             # handle form
@@ -229,36 +312,37 @@
                 and issubclass(arg.annotation, forms.BaseForm)
             ):
                 if found_form_arg:
                     raise Exception(
                         "You can only have one Form argument in a view function."
                     )
                 found_form_arg = True
-                result[arg.name] = _setup_injected_param(handle_form(), arg.name, arg)
+                result[arg.name] = _setup_injected_param(
+                    view_fn, handle_form(), arg.name, arg
+                )
             # from here, handle get and post params
             elif auto_param is True:
                 result[arg.name] = _setup_injected_param(
-                    InjectedParamQuery(default=default_value), arg.name, arg
+                    view_fn, InjectedParamQuery(default=default_value), arg.name, arg
                 )
             elif auto_param == "get":
                 result[arg.name] = _setup_injected_param(
-                    InjectedParamQueryGet(default=default_value), arg.name, arg
+                    view_fn, InjectedParamQueryGet(default=default_value), arg.name, arg
                 )
             elif auto_param == "post":
                 result[arg.name] = _setup_injected_param(
-                    InjectedParamQueryPost(default=default_value), arg.name, arg
+                    view_fn,
+                    InjectedParamQueryPost(default=default_value),
+                    arg.name,
+                    arg,
                 )
 
     return result
 
 
-def _get_request_from_args(args: list[Any]) -> HttpRequest:
-    return args[0]
-
-
 ################################################################################
 ### request params to args
 ################################################################################
 
 
 @dataclasses.dataclass
 class InjectedParamQuery(InjectedParam):
@@ -439,29 +523,9 @@
 def querydict_key_removed(querydict: dict, key) -> QueryDict:
     temp = QueryDict(mutable=True)
     temp.update(querydict)
     del temp[key]
     return temp
 
 
-def is_head(request: HttpRequest):
-    return request.method == "HEAD"
-
-
-def is_get(request: HttpRequest):
-    return request.method == "GET"
-
-
-def is_post(request: HttpRequest):
-    return request.method == "POST"
-
-
-def is_put(request: HttpRequest):
-    return request.method == "PUT"
-
-
-def is_patch(request: HttpRequest):
-    return request.method == "PATCH"
-
-
-def is_delete(request: HttpRequest):
-    return request.method == "DELETE"
+def _get_request_from_args(args: list[Any]) -> HttpRequest:
+    return args[0]
```

### Comparing `dfv-0.6.0/dfv/__pycache__/__init__.cpython-311.pyc` & `dfv-0.7.0/dfv/__pycache__/__init__.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,57 +1,66 @@
 magic:    0xa70d0d0a
-moddate:  0x2607c864 (Mon Jul 31 19:10:30 2023 UTC)
-files sz: 15349
+moddate:  0x45b4ca64 (Wed Aug  2 19:53:41 2023 UTC)
+files sz: 17371
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 12
+   stacksize : 13
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
-      00640f651f6604641084045a250900644664116412641364016414641564
+      00640f651f6604641084045a250900644d64116412641364016414641564
       169c066417650b6526190000000000000000006418650b65261900000000
       0000000000640f6509650965206521660219000000000000000000670165
       096520652166021900000000000000000066021900000000000000000066
-      06641984075a2709006447640e6518641a6518640f65186606641b84055a
-      2864156414641c9c02641d6529650a641e190000000000000000007a0700
-      00641f650b652965267a07000019000000000000000000640f6509650965
-      206521660219000000000000000000670165096520652166021900000000
-      00000000006602190000000000000000006606642084065a2a652a5a2b65
-      006a2c000000000000000002004700642184006422a6020000ab02000000
-      0000000000a6000000ab0000000000000000005a2d6423652d6424652664
-      2565026a2e00000000000000006606642684045a2f090064486427653065
-      026a2e000000000000000019000000000000000000641d6529650a642819
-      0000000000000000007a070000650a6429190000000000000000007a0700
-      00641f650b652965267a07000019000000000000000000640f6531652665
-      2d6602190000000000000000006608642a84055a32642b65306508190000
-      00000000000000640f65176604642c84045a3365006a2c00000000000000
-      0002004700642d8400642e652da6030000ab030000000000000000a60000
-      00ab0000000000000000005a3465006a2c00000000000000000200470064
-      2f840064306534a6030000ab030000000000000000a6000000ab00000000
-      00000000005a3565006a2c00000000000000000200470064318400643265
-      34a6030000ab030000000000000000a6000000ab0000000000000000005a
-      366449640f65086602643384055a376449640f65086602643484055a3802
-      0065046a39000000000000000065086401a6020000ab0200000000000000
-      006414660264356522640f65226604643684055a3a6437653065046a0800
-      00000000000000190000000000000000006438653b6604643984045a3c02
-      004700643a8400643b652da6030000ab0300000000000000005a3d640f65
-      086602643c84045a3e643d6531640f651a6604643e84045a3f643f651766
-      02644084045a40643f65176602644184045a41643f65176602644284045a
-      42643f65176602644384045a43643f65176602644484045a44643f651766
-      02644584045a4564015300
+      06641984075a270900644e640e6518641a6518640f65186606641b84055a
+      2865046a290000000000000000641c6517640f652a650919000000000000
+      0000006604641d8404a6000000ab0000000000000000005a2b65046a2900
+      00000000000000641c6517641e652c640f650b652a650919000000000000
+      000000190000000000000000006606641f8404a6000000ab000000000000
+      0000005a2b0900644f641c6517640f650b652a6509190000000000000000
+      00190000000000000000006604642084055a2b644f640f65096509652065
+      216602190000000000000000006701650965206521660219000000000000
+      0000006602190000000000000000006602642184055a2d641c6517660264
+      2284045a2e641c65176602642384045a2f641c65176602642484045a3064
+      1c65176602642584045a31641c65176602642684045a32641c6517660264
+      2784045a33641c65176602642884045a346415641464299c02642a652c65
+      0a642b190000000000000000007a070000642c650b652c65267a07000019
+      000000000000000000640f65096509652065216602190000000000000000
+      006701650965206521660219000000000000000000660219000000000000
+      0000006606642d84065a3565355a3665006a370000000000000000020047
+      00642e8400642fa6020000ab020000000000000000a6000000ab00000000
+      00000000005a386430650965086701650866021900000000000000000064
+      31653864326526643365026a3900000000000000006608643484045a3a09
+      00644f643065096508670165086602190000000000000000006435652a65
+      026a39000000000000000019000000000000000000642a652c650a643619
+      0000000000000000007a070000650a6437190000000000000000007a0700
+      00642c650b652c65267a07000019000000000000000000640f653b652665
+      38660219000000000000000000660a643884055a3c65006a370000000000
+      0000000200470064398400643a6538a6030000ab030000000000000000a6
+      000000ab0000000000000000005a3d65006a370000000000000000020047
+      00643b8400643c653da6030000ab030000000000000000a6000000ab0000
+      000000000000005a3e65006a37000000000000000002004700643d840064
+      3e653da6030000ab030000000000000000a6000000ab0000000000000000
+      005a3f6450640f65086602643f84055a406450640f65086602644084055a
+      41020065046a42000000000000000065086401a6020000ab020000000000
+      0000006414660264416522640f65226604644284055a436443652a65046a
+      08000000000000000019000000000000000000644465446604644584045a
+      45020047006446840064476538a6030000ab0300000000000000005a4664
+      0f65086602644884045a476449653b640f651a6604644a84045a48644b65
+      2a650819000000000000000000640f65176604644c84045a4964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (dataclasses)
                  8 STORE_NAME               0 (dataclasses)
    
@@ -198,15 +207,15 @@
                304 BUILD_TUPLE              4
                306 LOAD_CONST              16 (<code object response_to_str, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 61>)
                308 MAKE_FUNCTION            4 (annotations)
                310 STORE_NAME              37 (response_to_str)
    
     70         312 NOP
    
-    69         314 LOAD_CONST              70 ((None,))
+    69         314 LOAD_CONST              77 ((None,))
    
     72         316 LOAD_CONST              17 ('div')
    
     73         318 LOAD_CONST              18 ('this')
    
     74         320 LOAD_CONST              19 ('outerHTML')
    
@@ -248,329 +257,447 @@
                408 BINARY_SUBSCR
    
     69         418 BUILD_TUPLE              6
                420 LOAD_CONST              25 (<code object element, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 69>)
                422 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                424 STORE_NAME              39 (element)
    
-   112         426 NOP
+   110         426 NOP
    
-   111         428 LOAD_CONST              71 (('outerHTML',))
+   109         428 LOAD_CONST              78 (('outerHTML',))
                430 LOAD_CONST              14 ('response')
    
-   112         432 LOAD_NAME               24 (HttpResponse)
+   110         432 LOAD_NAME               24 (HttpResponse)
    
-   111         434 LOAD_CONST              26 ('additional')
+   109         434 LOAD_CONST              26 ('additional')
    
-   112         436 LOAD_NAME               24 (HttpResponse)
+   110         436 LOAD_NAME               24 (HttpResponse)
    
-   111         438 LOAD_CONST              15 ('return')
+   109         438 LOAD_CONST              15 ('return')
    
-   113         440 LOAD_NAME               24 (HttpResponse)
+   111         440 LOAD_NAME               24 (HttpResponse)
    
-   111         442 BUILD_TUPLE              6
-               444 LOAD_CONST              27 (<code object swap_oob, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 111>)
+   109         442 BUILD_TUPLE              6
+               444 LOAD_CONST              27 (<code object swap_oob, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 109>)
                446 MAKE_FUNCTION            5 (defaults, annotations)
                448 STORE_NAME              40 (swap_oob)
    
-   134         450 LOAD_CONST              21 (False)
+   130         450 LOAD_NAME                4 (typing)
+               452 LOAD_ATTR               41 (overload)
    
-   135         452 LOAD_CONST              20 (True)
-   
-   132         454 LOAD_CONST              28 (('auto_param', 'auto_form'))
-               456 BUILD_CONST_KEY_MAP      2
-               458 LOAD_CONST              29 ('auto_param')
-   
-   134         460 LOAD_NAME               41 (bool)
-               462 LOAD_NAME               10 (Literal)
-               464 LOAD_CONST              30 (('get', 'post'))
-               466 BINARY_SUBSCR
-               476 BINARY_OP                7 (|)
-   
-   132         480 LOAD_CONST              31 ('auto_form')
-   
-   135         482 LOAD_NAME               11 (Optional)
-               484 LOAD_NAME               41 (bool)
-               486 LOAD_NAME               38 (str)
-               488 BINARY_OP                7 (|)
-               492 BINARY_SUBSCR
-   
-   132         502 LOAD_CONST              15 ('return')
-   
-   136         504 LOAD_NAME                9 (Callable)
-               506 LOAD_NAME                9 (Callable)
-               508 LOAD_NAME               32 (P)
-               510 LOAD_NAME               33 (R)
-               512 BUILD_TUPLE              2
-               514 BINARY_SUBSCR
-               524 BUILD_LIST               1
-               526 LOAD_NAME                9 (Callable)
-               528 LOAD_NAME               32 (P)
-               530 LOAD_NAME               33 (R)
-               532 BUILD_TUPLE              2
-               534 BINARY_SUBSCR
-               544 BUILD_TUPLE              2
-               546 BINARY_SUBSCR
-   
-   132         556 BUILD_TUPLE              6
-               558 LOAD_CONST              32 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 132>)
-               560 MAKE_FUNCTION            6 (kwdefaults, annotations)
-               562 STORE_NAME              42 (inject_args)
-   
-   164         564 LOAD_NAME               42 (inject_args)
-               566 STORE_NAME              43 (_inject_args)
-   
-   167         568 LOAD_NAME                0 (dataclasses)
-               570 LOAD_ATTR               44 (dataclass)
-   
-   168         580 PUSH_NULL
-               582 LOAD_BUILD_CLASS
-               584 LOAD_CONST              33 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 167>)
-               586 MAKE_FUNCTION            0
-               588 LOAD_CONST              34 ('InjectedParam')
-               590 PRECALL                  2
-               594 CALL                     2
-   
-   167         604 PRECALL                  0
-               608 CALL                     0
-   
-   168         618 STORE_NAME              45 (InjectedParam)
-   
-   184         620 LOAD_CONST              35 ('ip')
-               622 LOAD_NAME               45 (InjectedParam)
-               624 LOAD_CONST              36 ('name')
-               626 LOAD_NAME               38 (str)
-               628 LOAD_CONST              37 ('parameter')
-               630 LOAD_NAME                2 (inspect)
-               632 LOAD_ATTR               46 (Parameter)
-               642 BUILD_TUPLE              6
-               644 LOAD_CONST              38 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 184>)
-               646 MAKE_FUNCTION            4 (annotations)
-               648 STORE_NAME              47 (_setup_injected_param)
-   
-   204         650 NOP
-   
-   201         652 LOAD_CONST              72 ((True,))
-               654 LOAD_CONST              39 ('parameters')
-   
-   202         656 LOAD_NAME               48 (list)
-               658 LOAD_NAME                2 (inspect)
-               660 LOAD_ATTR               46 (Parameter)
-               670 BINARY_SUBSCR
-   
-   201         680 LOAD_CONST              29 ('auto_param')
-   
-   203         682 LOAD_NAME               41 (bool)
-               684 LOAD_NAME               10 (Literal)
-               686 LOAD_CONST              40 ('get')
-               688 BINARY_SUBSCR
-               698 BINARY_OP                7 (|)
-               702 LOAD_NAME               10 (Literal)
-               704 LOAD_CONST              41 ('post')
-               706 BINARY_SUBSCR
-               716 BINARY_OP                7 (|)
-   
-   201         720 LOAD_CONST              31 ('auto_form')
-   
-   204         722 LOAD_NAME               11 (Optional)
-               724 LOAD_NAME               41 (bool)
-               726 LOAD_NAME               38 (str)
-               728 BINARY_OP                7 (|)
-               732 BINARY_SUBSCR
-   
-   201         742 LOAD_CONST              15 ('return')
-   
-   205         744 LOAD_NAME               49 (dict)
-               746 LOAD_NAME               38 (str)
-               748 LOAD_NAME               45 (InjectedParam)
-               750 BUILD_TUPLE              2
-               752 BINARY_SUBSCR
-   
-   201         762 BUILD_TUPLE              8
-               764 LOAD_CONST              42 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 201>)
-               766 MAKE_FUNCTION            5 (defaults, annotations)
-               768 STORE_NAME              50 (_extract_injected_params)
-   
-   254         770 LOAD_CONST              43 ('args')
-               772 LOAD_NAME               48 (list)
-               774 LOAD_NAME                8 (Any)
-               776 BINARY_SUBSCR
-               786 LOAD_CONST              15 ('return')
-               788 LOAD_NAME               23 (HttpRequest)
-               790 BUILD_TUPLE              4
-               792 LOAD_CONST              44 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 254>)
-               794 MAKE_FUNCTION            4 (annotations)
-               796 STORE_NAME              51 (_get_request_from_args)
-   
-   263         798 LOAD_NAME                0 (dataclasses)
-               800 LOAD_ATTR               44 (dataclass)
-   
-   264         810 PUSH_NULL
-               812 LOAD_BUILD_CLASS
-               814 LOAD_CONST              45 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 263>)
-               816 MAKE_FUNCTION            0
-               818 LOAD_CONST              46 ('InjectedParamQuery')
-               820 LOAD_NAME               45 (InjectedParam)
-               822 PRECALL                  3
-               826 CALL                     3
-   
-   263         836 PRECALL                  0
-               840 CALL                     0
-   
-   264         850 STORE_NAME              52 (InjectedParamQuery)
-   
-   311         852 LOAD_NAME                0 (dataclasses)
-               854 LOAD_ATTR               44 (dataclass)
-   
-   312         864 PUSH_NULL
-               866 LOAD_BUILD_CLASS
-               868 LOAD_CONST              47 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 311>)
-               870 MAKE_FUNCTION            0
-               872 LOAD_CONST              48 ('InjectedParamQueryGet')
-               874 LOAD_NAME               52 (InjectedParamQuery)
-               876 PRECALL                  3
-               880 CALL                     3
-   
-   311         890 PRECALL                  0
-               894 CALL                     0
-   
-   312         904 STORE_NAME              53 (InjectedParamQueryGet)
-   
-   324         906 LOAD_NAME                0 (dataclasses)
-               908 LOAD_ATTR               44 (dataclass)
-   
-   325         918 PUSH_NULL
-               920 LOAD_BUILD_CLASS
-               922 LOAD_CONST              49 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 324>)
-               924 MAKE_FUNCTION            0
-               926 LOAD_CONST              50 ('InjectedParamQueryPost')
-               928 LOAD_NAME               52 (InjectedParamQuery)
-               930 PRECALL                  3
-               934 CALL                     3
-   
-   324         944 PRECALL                  0
-               948 CALL                     0
-   
-   325         958 STORE_NAME              54 (InjectedParamQueryPost)
-   
-   337         960 LOAD_CONST              73 ((None, True))
-               962 LOAD_CONST              15 ('return')
-               964 LOAD_NAME                8 (Any)
-               966 BUILD_TUPLE              2
-               968 LOAD_CONST              51 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 337>)
-               970 MAKE_FUNCTION            5 (defaults, annotations)
-               972 STORE_NAME              55 (param_get)
-   
-   341         974 LOAD_CONST              73 ((None, True))
-               976 LOAD_CONST              15 ('return')
-               978 LOAD_NAME                8 (Any)
-               980 BUILD_TUPLE              2
-               982 LOAD_CONST              52 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 341>)
-               984 MAKE_FUNCTION            5 (defaults, annotations)
-               986 STORE_NAME              56 (param_post)
-   
-   345         988 PUSH_NULL
-               990 LOAD_NAME                4 (typing)
-               992 LOAD_ATTR               57 (cast)
-              1002 LOAD_NAME                8 (Any)
-              1004 LOAD_CONST               1 (None)
-              1006 PRECALL                  2
-              1010 CALL                     2
-              1020 LOAD_CONST              20 (True)
-              1022 BUILD_TUPLE              2
-              1024 LOAD_CONST              53 ('default')
-              1026 LOAD_NAME               34 (T)
-              1028 LOAD_CONST              15 ('return')
-              1030 LOAD_NAME               34 (T)
-              1032 BUILD_TUPLE              4
-              1034 LOAD_CONST              54 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 345>)
-              1036 MAKE_FUNCTION            5 (defaults, annotations)
-              1038 STORE_NAME              58 (param)
-   
-   349        1040 LOAD_CONST              55 ('values')
-              1042 LOAD_NAME               48 (list)
-              1044 LOAD_NAME                4 (typing)
-              1046 LOAD_ATTR                8 (Any)
-              1056 BINARY_SUBSCR
-              1066 LOAD_CONST              56 ('target_type')
-              1068 LOAD_NAME               59 (type)
-              1070 BUILD_TUPLE              4
-              1072 LOAD_CONST              57 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 349>)
-              1074 MAKE_FUNCTION            4 (annotations)
-              1076 STORE_NAME              60 (_convert_value_to_type)
-   
-   384        1078 PUSH_NULL
-              1080 LOAD_BUILD_CLASS
-              1082 LOAD_CONST              58 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 384>)
-              1084 MAKE_FUNCTION            0
-              1086 LOAD_CONST              59 ('InjectedParamForm')
-              1088 LOAD_NAME               45 (InjectedParam)
-              1090 PRECALL                  3
-              1094 CALL                     3
-              1104 STORE_NAME              61 (InjectedParamForm)
-   
-   430        1106 LOAD_CONST              15 ('return')
-              1108 LOAD_NAME                8 (Any)
+   131         462 LOAD_CONST              28 ('request')
+               464 LOAD_NAME               23 (HttpRequest)
+               466 LOAD_CONST              15 ('return')
+               468 LOAD_NAME               42 (list)
+               470 LOAD_NAME                9 (Callable)
+               472 BINARY_SUBSCR
+               482 BUILD_TUPLE              4
+               484 LOAD_CONST              29 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 130>)
+               486 MAKE_FUNCTION            4 (annotations)
+   
+   130         488 PRECALL                  0
+               492 CALL                     0
+   
+   131         502 STORE_NAME              43 (get_view_fn_call_stack_from_request)
+   
+   135         504 LOAD_NAME                4 (typing)
+               506 LOAD_ATTR               41 (overload)
+   
+   136         516 LOAD_CONST              28 ('request')
+   
+   137         518 LOAD_NAME               23 (HttpRequest)
+   
+   136         520 LOAD_CONST              30 ('create')
+   
+   137         522 LOAD_NAME               44 (bool)
+   
+   136         524 LOAD_CONST              15 ('return')
+   
+   138         526 LOAD_NAME               11 (Optional)
+               528 LOAD_NAME               42 (list)
+               530 LOAD_NAME                9 (Callable)
+               532 BINARY_SUBSCR
+               542 BINARY_SUBSCR
+   
+   136         552 BUILD_TUPLE              6
+               554 LOAD_CONST              31 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 135>)
+               556 MAKE_FUNCTION            4 (annotations)
+   
+   135         558 PRECALL                  0
+               562 CALL                     0
+   
+   136         572 STORE_NAME              43 (get_view_fn_call_stack_from_request)
+   
+   143         574 NOP
+   
+   142         576 LOAD_CONST              79 ((True,))
+               578 LOAD_CONST              28 ('request')
+   
+   143         580 LOAD_NAME               23 (HttpRequest)
+   
+   142         582 LOAD_CONST              15 ('return')
+   
+   144         584 LOAD_NAME               11 (Optional)
+               586 LOAD_NAME               42 (list)
+               588 LOAD_NAME                9 (Callable)
+               590 BINARY_SUBSCR
+               600 BINARY_SUBSCR
+   
+   142         610 BUILD_TUPLE              4
+               612 LOAD_CONST              32 (<code object get_view_fn_call_stack_from_request, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 142>)
+               614 MAKE_FUNCTION            5 (defaults, annotations)
+               616 STORE_NAME              43 (get_view_fn_call_stack_from_request)
+   
+   151         618 LOAD_CONST              79 ((True,))
+               620 LOAD_CONST              15 ('return')
+               622 LOAD_NAME                9 (Callable)
+               624 LOAD_NAME                9 (Callable)
+               626 LOAD_NAME               32 (P)
+               628 LOAD_NAME               33 (R)
+               630 BUILD_TUPLE              2
+               632 BINARY_SUBSCR
+               642 BUILD_LIST               1
+               644 LOAD_NAME                9 (Callable)
+               646 LOAD_NAME               32 (P)
+               648 LOAD_NAME               33 (R)
+               650 BUILD_TUPLE              2
+               652 BINARY_SUBSCR
+               662 BUILD_TUPLE              2
+               664 BINARY_SUBSCR
+               674 BUILD_TUPLE              2
+               676 LOAD_CONST              33 (<code object view, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 151>)
+               678 MAKE_FUNCTION            5 (defaults, annotations)
+               680 STORE_NAME              45 (view)
+   
+   171         682 LOAD_CONST              28 ('request')
+               684 LOAD_NAME               23 (HttpRequest)
+               686 BUILD_TUPLE              2
+               688 LOAD_CONST              34 (<code object is_view_fn_request_target, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 171>)
+               690 MAKE_FUNCTION            4 (annotations)
+               692 STORE_NAME              46 (is_view_fn_request_target)
+   
+   176         694 LOAD_CONST              28 ('request')
+               696 LOAD_NAME               23 (HttpRequest)
+               698 BUILD_TUPLE              2
+               700 LOAD_CONST              35 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 176>)
+               702 MAKE_FUNCTION            4 (annotations)
+               704 STORE_NAME              47 (is_head)
+   
+   180         706 LOAD_CONST              28 ('request')
+               708 LOAD_NAME               23 (HttpRequest)
+               710 BUILD_TUPLE              2
+               712 LOAD_CONST              36 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 180>)
+               714 MAKE_FUNCTION            4 (annotations)
+               716 STORE_NAME              48 (is_get)
+   
+   184         718 LOAD_CONST              28 ('request')
+               720 LOAD_NAME               23 (HttpRequest)
+               722 BUILD_TUPLE              2
+               724 LOAD_CONST              37 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 184>)
+               726 MAKE_FUNCTION            4 (annotations)
+               728 STORE_NAME              49 (is_post)
+   
+   188         730 LOAD_CONST              28 ('request')
+               732 LOAD_NAME               23 (HttpRequest)
+               734 BUILD_TUPLE              2
+               736 LOAD_CONST              38 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 188>)
+               738 MAKE_FUNCTION            4 (annotations)
+               740 STORE_NAME              50 (is_put)
+   
+   192         742 LOAD_CONST              28 ('request')
+               744 LOAD_NAME               23 (HttpRequest)
+               746 BUILD_TUPLE              2
+               748 LOAD_CONST              39 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 192>)
+               750 MAKE_FUNCTION            4 (annotations)
+               752 STORE_NAME              51 (is_patch)
+   
+   196         754 LOAD_CONST              28 ('request')
+               756 LOAD_NAME               23 (HttpRequest)
+               758 BUILD_TUPLE              2
+               760 LOAD_CONST              40 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 196>)
+               762 MAKE_FUNCTION            4 (annotations)
+               764 STORE_NAME              52 (is_delete)
+   
+   207         766 LOAD_CONST              21 (False)
+   
+   208         768 LOAD_CONST              20 (True)
+   
+   205         770 LOAD_CONST              41 (('auto_param', 'auto_form'))
+               772 BUILD_CONST_KEY_MAP      2
+               774 LOAD_CONST              42 ('auto_param')
+   
+   207         776 LOAD_NAME               44 (bool)
+               778 LOAD_NAME               10 (Literal)
+               780 LOAD_CONST              43 (('get', 'post'))
+               782 BINARY_SUBSCR
+               792 BINARY_OP                7 (|)
+   
+   205         796 LOAD_CONST              44 ('auto_form')
+   
+   208         798 LOAD_NAME               11 (Optional)
+               800 LOAD_NAME               44 (bool)
+               802 LOAD_NAME               38 (str)
+               804 BINARY_OP                7 (|)
+               808 BINARY_SUBSCR
+   
+   205         818 LOAD_CONST              15 ('return')
+   
+   209         820 LOAD_NAME                9 (Callable)
+               822 LOAD_NAME                9 (Callable)
+               824 LOAD_NAME               32 (P)
+               826 LOAD_NAME               33 (R)
+               828 BUILD_TUPLE              2
+               830 BINARY_SUBSCR
+               840 BUILD_LIST               1
+               842 LOAD_NAME                9 (Callable)
+               844 LOAD_NAME               32 (P)
+               846 LOAD_NAME               33 (R)
+               848 BUILD_TUPLE              2
+               850 BINARY_SUBSCR
+               860 BUILD_TUPLE              2
+               862 BINARY_SUBSCR
+   
+   205         872 BUILD_TUPLE              6
+               874 LOAD_CONST              45 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 205>)
+               876 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               878 STORE_NAME              53 (inject_args)
+   
+   239         880 LOAD_NAME               53 (inject_args)
+               882 STORE_NAME              54 (_inject_args)
+   
+   242         884 LOAD_NAME                0 (dataclasses)
+               886 LOAD_ATTR               55 (dataclass)
+   
+   243         896 PUSH_NULL
+               898 LOAD_BUILD_CLASS
+               900 LOAD_CONST              46 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 242>)
+               902 MAKE_FUNCTION            0
+               904 LOAD_CONST              47 ('InjectedParam')
+               906 PRECALL                  2
+               910 CALL                     2
+   
+   242         920 PRECALL                  0
+               924 CALL                     0
+   
+   243         934 STORE_NAME              56 (InjectedParam)
+   
+   260         936 LOAD_CONST              48 ('view_fn')
+   
+   261         938 LOAD_NAME                9 (Callable)
+               940 LOAD_NAME                8 (Any)
+               942 BUILD_LIST               1
+               944 LOAD_NAME                8 (Any)
+               946 BUILD_TUPLE              2
+               948 BINARY_SUBSCR
+   
+   260         958 LOAD_CONST              49 ('ip')
+   
+   262         960 LOAD_NAME               56 (InjectedParam)
+   
+   260         962 LOAD_CONST              50 ('name')
+   
+   263         964 LOAD_NAME               38 (str)
+   
+   260         966 LOAD_CONST              51 ('parameter')
+   
+   264         968 LOAD_NAME                2 (inspect)
+               970 LOAD_ATTR               57 (Parameter)
+   
+   260         980 BUILD_TUPLE              8
+               982 LOAD_CONST              52 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 260>)
+               984 MAKE_FUNCTION            4 (annotations)
+               986 STORE_NAME              58 (_setup_injected_param)
+   
+   287         988 NOP
+   
+   283         990 LOAD_CONST              79 ((True,))
+               992 LOAD_CONST              48 ('view_fn')
+   
+   284         994 LOAD_NAME                9 (Callable)
+               996 LOAD_NAME                8 (Any)
+               998 BUILD_LIST               1
+              1000 LOAD_NAME                8 (Any)
+              1002 BUILD_TUPLE              2
+              1004 BINARY_SUBSCR
+   
+   283        1014 LOAD_CONST              53 ('parameters')
+   
+   285        1016 LOAD_NAME               42 (list)
+              1018 LOAD_NAME                2 (inspect)
+              1020 LOAD_ATTR               57 (Parameter)
+              1030 BINARY_SUBSCR
+   
+   283        1040 LOAD_CONST              42 ('auto_param')
+   
+   286        1042 LOAD_NAME               44 (bool)
+              1044 LOAD_NAME               10 (Literal)
+              1046 LOAD_CONST              54 ('get')
+              1048 BINARY_SUBSCR
+              1058 BINARY_OP                7 (|)
+              1062 LOAD_NAME               10 (Literal)
+              1064 LOAD_CONST              55 ('post')
+              1066 BINARY_SUBSCR
+              1076 BINARY_OP                7 (|)
+   
+   283        1080 LOAD_CONST              44 ('auto_form')
+   
+   287        1082 LOAD_NAME               11 (Optional)
+              1084 LOAD_NAME               44 (bool)
+              1086 LOAD_NAME               38 (str)
+              1088 BINARY_OP                7 (|)
+              1092 BINARY_SUBSCR
+   
+   283        1102 LOAD_CONST              15 ('return')
+   
+   288        1104 LOAD_NAME               59 (dict)
+              1106 LOAD_NAME               38 (str)
+              1108 LOAD_NAME               56 (InjectedParam)
               1110 BUILD_TUPLE              2
-              1112 LOAD_CONST              60 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 430>)
-              1114 MAKE_FUNCTION            4 (annotations)
-              1116 STORE_NAME              62 (handle_form)
-   
-   439        1118 LOAD_CONST              61 ('querydict')
-              1120 LOAD_NAME               49 (dict)
-              1122 LOAD_CONST              15 ('return')
-              1124 LOAD_NAME               26 (QueryDict)
-              1126 BUILD_TUPLE              4
-              1128 LOAD_CONST              62 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 439>)
-              1130 MAKE_FUNCTION            4 (annotations)
-              1132 STORE_NAME              63 (querydict_key_removed)
-   
-   446        1134 LOAD_CONST              63 ('request')
-              1136 LOAD_NAME               23 (HttpRequest)
-              1138 BUILD_TUPLE              2
-              1140 LOAD_CONST              64 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 446>)
-              1142 MAKE_FUNCTION            4 (annotations)
-              1144 STORE_NAME              64 (is_head)
-   
-   450        1146 LOAD_CONST              63 ('request')
-              1148 LOAD_NAME               23 (HttpRequest)
-              1150 BUILD_TUPLE              2
-              1152 LOAD_CONST              65 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 450>)
-              1154 MAKE_FUNCTION            4 (annotations)
-              1156 STORE_NAME              65 (is_get)
-   
-   454        1158 LOAD_CONST              63 ('request')
-              1160 LOAD_NAME               23 (HttpRequest)
-              1162 BUILD_TUPLE              2
-              1164 LOAD_CONST              66 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 454>)
-              1166 MAKE_FUNCTION            4 (annotations)
-              1168 STORE_NAME              66 (is_post)
-   
-   458        1170 LOAD_CONST              63 ('request')
-              1172 LOAD_NAME               23 (HttpRequest)
-              1174 BUILD_TUPLE              2
-              1176 LOAD_CONST              67 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 458>)
-              1178 MAKE_FUNCTION            4 (annotations)
-              1180 STORE_NAME              67 (is_put)
-   
-   462        1182 LOAD_CONST              63 ('request')
-              1184 LOAD_NAME               23 (HttpRequest)
-              1186 BUILD_TUPLE              2
-              1188 LOAD_CONST              68 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 462>)
-              1190 MAKE_FUNCTION            4 (annotations)
-              1192 STORE_NAME              68 (is_patch)
-   
-   466        1194 LOAD_CONST              63 ('request')
-              1196 LOAD_NAME               23 (HttpRequest)
-              1198 BUILD_TUPLE              2
-              1200 LOAD_CONST              69 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 466>)
-              1202 MAKE_FUNCTION            4 (annotations)
-              1204 STORE_NAME              69 (is_delete)
-              1206 LOAD_CONST               1 (None)
-              1208 RETURN_VALUE
+              1112 BINARY_SUBSCR
+   
+   283        1122 BUILD_TUPLE             10
+              1124 LOAD_CONST              56 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 283>)
+              1126 MAKE_FUNCTION            5 (defaults, annotations)
+              1128 STORE_NAME              60 (_extract_injected_params)
+   
+   347        1130 LOAD_NAME                0 (dataclasses)
+              1132 LOAD_ATTR               55 (dataclass)
+   
+   348        1142 PUSH_NULL
+              1144 LOAD_BUILD_CLASS
+              1146 LOAD_CONST              57 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 347>)
+              1148 MAKE_FUNCTION            0
+              1150 LOAD_CONST              58 ('InjectedParamQuery')
+              1152 LOAD_NAME               56 (InjectedParam)
+              1154 PRECALL                  3
+              1158 CALL                     3
+   
+   347        1168 PRECALL                  0
+              1172 CALL                     0
+   
+   348        1182 STORE_NAME              61 (InjectedParamQuery)
+   
+   395        1184 LOAD_NAME                0 (dataclasses)
+              1186 LOAD_ATTR               55 (dataclass)
+   
+   396        1196 PUSH_NULL
+              1198 LOAD_BUILD_CLASS
+              1200 LOAD_CONST              59 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 395>)
+              1202 MAKE_FUNCTION            0
+              1204 LOAD_CONST              60 ('InjectedParamQueryGet')
+              1206 LOAD_NAME               61 (InjectedParamQuery)
+              1208 PRECALL                  3
+              1212 CALL                     3
+   
+   395        1222 PRECALL                  0
+              1226 CALL                     0
+   
+   396        1236 STORE_NAME              62 (InjectedParamQueryGet)
+   
+   408        1238 LOAD_NAME                0 (dataclasses)
+              1240 LOAD_ATTR               55 (dataclass)
+   
+   409        1250 PUSH_NULL
+              1252 LOAD_BUILD_CLASS
+              1254 LOAD_CONST              61 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 408>)
+              1256 MAKE_FUNCTION            0
+              1258 LOAD_CONST              62 ('InjectedParamQueryPost')
+              1260 LOAD_NAME               61 (InjectedParamQuery)
+              1262 PRECALL                  3
+              1266 CALL                     3
+   
+   408        1276 PRECALL                  0
+              1280 CALL                     0
+   
+   409        1290 STORE_NAME              63 (InjectedParamQueryPost)
+   
+   421        1292 LOAD_CONST              80 ((None, True))
+              1294 LOAD_CONST              15 ('return')
+              1296 LOAD_NAME                8 (Any)
+              1298 BUILD_TUPLE              2
+              1300 LOAD_CONST              63 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 421>)
+              1302 MAKE_FUNCTION            5 (defaults, annotations)
+              1304 STORE_NAME              64 (param_get)
+   
+   425        1306 LOAD_CONST              80 ((None, True))
+              1308 LOAD_CONST              15 ('return')
+              1310 LOAD_NAME                8 (Any)
+              1312 BUILD_TUPLE              2
+              1314 LOAD_CONST              64 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 425>)
+              1316 MAKE_FUNCTION            5 (defaults, annotations)
+              1318 STORE_NAME              65 (param_post)
+   
+   429        1320 PUSH_NULL
+              1322 LOAD_NAME                4 (typing)
+              1324 LOAD_ATTR               66 (cast)
+              1334 LOAD_NAME                8 (Any)
+              1336 LOAD_CONST               1 (None)
+              1338 PRECALL                  2
+              1342 CALL                     2
+              1352 LOAD_CONST              20 (True)
+              1354 BUILD_TUPLE              2
+              1356 LOAD_CONST              65 ('default')
+              1358 LOAD_NAME               34 (T)
+              1360 LOAD_CONST              15 ('return')
+              1362 LOAD_NAME               34 (T)
+              1364 BUILD_TUPLE              4
+              1366 LOAD_CONST              66 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 429>)
+              1368 MAKE_FUNCTION            5 (defaults, annotations)
+              1370 STORE_NAME              67 (param)
+   
+   433        1372 LOAD_CONST              67 ('values')
+              1374 LOAD_NAME               42 (list)
+              1376 LOAD_NAME                4 (typing)
+              1378 LOAD_ATTR                8 (Any)
+              1388 BINARY_SUBSCR
+              1398 LOAD_CONST              68 ('target_type')
+              1400 LOAD_NAME               68 (type)
+              1402 BUILD_TUPLE              4
+              1404 LOAD_CONST              69 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 433>)
+              1406 MAKE_FUNCTION            4 (annotations)
+              1408 STORE_NAME              69 (_convert_value_to_type)
+   
+   468        1410 PUSH_NULL
+              1412 LOAD_BUILD_CLASS
+              1414 LOAD_CONST              70 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 468>)
+              1416 MAKE_FUNCTION            0
+              1418 LOAD_CONST              71 ('InjectedParamForm')
+              1420 LOAD_NAME               56 (InjectedParam)
+              1422 PRECALL                  3
+              1426 CALL                     3
+              1436 STORE_NAME              70 (InjectedParamForm)
+   
+   514        1438 LOAD_CONST              15 ('return')
+              1440 LOAD_NAME                8 (Any)
+              1442 BUILD_TUPLE              2
+              1444 LOAD_CONST              72 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 514>)
+              1446 MAKE_FUNCTION            4 (annotations)
+              1448 STORE_NAME              71 (handle_form)
+   
+   523        1450 LOAD_CONST              73 ('querydict')
+              1452 LOAD_NAME               59 (dict)
+              1454 LOAD_CONST              15 ('return')
+              1456 LOAD_NAME               26 (QueryDict)
+              1458 BUILD_TUPLE              4
+              1460 LOAD_CONST              74 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 523>)
+              1462 MAKE_FUNCTION            4 (annotations)
+              1464 STORE_NAME              72 (querydict_key_removed)
+   
+   530        1466 LOAD_CONST              75 ('args')
+              1468 LOAD_NAME               42 (list)
+              1470 LOAD_NAME                8 (Any)
+              1472 BINARY_SUBSCR
+              1482 LOAD_CONST              15 ('return')
+              1484 LOAD_NAME               23 (HttpRequest)
+              1486 BUILD_TUPLE              4
+              1488 LOAD_CONST              76 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 530>)
+              1490 MAKE_FUNCTION            4 (annotations)
+              1492 STORE_NAME              73 (_get_request_from_args)
+              1494 LOAD_CONST               1 (None)
+              1496 RETURN_VALUE
    consts
       0
       None
       ('NoneType',)
       ('Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar')
       ('forms',)
       ('decorators',)
@@ -972,37 +1099,37 @@
                      128 LOAD_CLOSURE             6 (login_required)
                      130 LOAD_CLOSURE             1 (tag)
                      132 BUILD_TUPLE              7
                      134 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 79>)
                      136 MAKE_FUNCTION           12 (annotations, closure)
                      138 STORE_FAST               7 (decorator)
          
-         108         140 LOAD_FAST                7 (decorator)
+         106         140 LOAD_FAST                7 (decorator)
                      142 RETURN_VALUE
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
                   0x9507870087029700740100000000000000000000890474020000000000
                   0000000000a6020000ab020000000000000000720289046e0689006a0200
-                  000000000000008a02890572170200740700000000000000000000a60000
-                  00ab0000000000000000008900a6010000ab0100000000000000008a0089
-                  08721c02007409000000000000000000006a050000000000000000a60000
-                  00ab0000000000000000008900a6010000ab0100000000000000008a0074
-                  0d000000000000000000006a0700000000000000008900a6010000ab0100
-                  0000000000000064017410000000000000000000006a0900000000000000
-                  0064027410000000000000000000006a0a00000000000000006403741600
-                  000000000000000000660688038800880688078802880966066404840ca6
-                  000000ab0000000000000000007d017c015300
+                  000000000000008a0202007407000000000000000000008905a6010000ab
+                  0100000000000000008900a6010000ab0100000000000000008a00890872
+                  1c02007409000000000000000000006a050000000000000000a6000000ab
+                  0000000000000000008900a6010000ab0100000000000000008a00740d00
+                  0000000000000000006a0700000000000000008900a6010000ab01000000
+                  000000000064017410000000000000000000006a09000000000000000064
+                  027410000000000000000000006a0a000000000000000064037416000000
+                  00000000000000660688038800880688078802880966066404840ca60000
+                  00ab0000000000000000007d017c015300
                              0 COPY_FREE_VARS           7
                              2 MAKE_CELL                0 (f)
                              4 MAKE_CELL                2 (id)
                
                 79           6 RESUME                   0
                
                 80           8 LOAD_GLOBAL              1 (NULL + isinstance)
@@ -1013,71 +1140,69 @@
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                             50 LOAD_DEREF               4 (element_id)
                             52 JUMP_FORWARD             6 (to 66)
                        >>   54 LOAD_DEREF               0 (f)
                             56 LOAD_ATTR                2 (__name__)
                        >>   66 STORE_DEREF              2 (id)
                
-                82          68 LOAD_DEREF               5 (handle_args)
-                            70 POP_JUMP_FORWARD_IF_FALSE    23 (to 118)
-               
-                83          72 PUSH_NULL
-                            74 LOAD_GLOBAL              7 (NULL + _inject_args)
-                            86 PRECALL                  0
-                            90 CALL                     0
-                           100 LOAD_DEREF               0 (f)
-                           102 PRECALL                  1
-                           106 CALL                     1
-                           116 STORE_DEREF              0 (f)
-               
-                85     >>  118 LOAD_DEREF               8 (login_required)
-                           120 POP_JUMP_FORWARD_IF_FALSE    28 (to 178)
-               
-                86         122 PUSH_NULL
-                           124 LOAD_GLOBAL              9 (NULL + auth_decorators)
-                           136 LOAD_ATTR                5 (login_required)
-                           146 PRECALL                  0
-                           150 CALL                     0
-                           160 LOAD_DEREF               0 (f)
-                           162 PRECALL                  1
-                           166 CALL                     1
-                           176 STORE_DEREF              0 (f)
-               
-                88     >>  178 LOAD_GLOBAL             13 (NULL + functools)
-                           190 LOAD_ATTR                7 (wraps)
-                           200 LOAD_DEREF               0 (f)
-                           202 PRECALL                  1
-                           206 CALL                     1
-               
-                89         216 LOAD_CONST               1 ('args')
-                           218 LOAD_GLOBAL             16 (P)
-                           230 LOAD_ATTR                9 (args)
-                           240 LOAD_CONST               2 ('kwargs')
-                           242 LOAD_GLOBAL             16 (P)
-                           254 LOAD_ATTR               10 (kwargs)
-                           264 LOAD_CONST               3 ('return')
-                           266 LOAD_GLOBAL             22 (HttpResponse)
-                           278 BUILD_TUPLE              6
-                           280 LOAD_CLOSURE             3 (classes)
-                           282 LOAD_CLOSURE             0 (f)
-                           284 LOAD_CLOSURE             6 (hx_swap)
-                           286 LOAD_CLOSURE             7 (hx_target)
-                           288 LOAD_CLOSURE             2 (id)
-                           290 LOAD_CLOSURE             9 (tag)
-                           292 BUILD_TUPLE              6
-                           294 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 88>)
-                           296 MAKE_FUNCTION           12 (annotations, closure)
+                81          68 PUSH_NULL
+                            70 LOAD_GLOBAL              7 (NULL + view)
+                            82 LOAD_DEREF               5 (handle_args)
+                            84 PRECALL                  1
+                            88 CALL                     1
+                            98 LOAD_DEREF               0 (f)
+                           100 PRECALL                  1
+                           104 CALL                     1
+                           114 STORE_DEREF              0 (f)
+               
+                83         116 LOAD_DEREF               8 (login_required)
+                           118 POP_JUMP_FORWARD_IF_FALSE    28 (to 176)
+               
+                84         120 PUSH_NULL
+                           122 LOAD_GLOBAL              9 (NULL + auth_decorators)
+                           134 LOAD_ATTR                5 (login_required)
+                           144 PRECALL                  0
+                           148 CALL                     0
+                           158 LOAD_DEREF               0 (f)
+                           160 PRECALL                  1
+                           164 CALL                     1
+                           174 STORE_DEREF              0 (f)
+               
+                86     >>  176 LOAD_GLOBAL             13 (NULL + functools)
+                           188 LOAD_ATTR                7 (wraps)
+                           198 LOAD_DEREF               0 (f)
+                           200 PRECALL                  1
+                           204 CALL                     1
+               
+                87         214 LOAD_CONST               1 ('args')
+                           216 LOAD_GLOBAL             16 (P)
+                           228 LOAD_ATTR                9 (args)
+                           238 LOAD_CONST               2 ('kwargs')
+                           240 LOAD_GLOBAL             16 (P)
+                           252 LOAD_ATTR               10 (kwargs)
+                           262 LOAD_CONST               3 ('return')
+                           264 LOAD_GLOBAL             22 (HttpResponse)
+                           276 BUILD_TUPLE              6
+                           278 LOAD_CLOSURE             3 (classes)
+                           280 LOAD_CLOSURE             0 (f)
+                           282 LOAD_CLOSURE             6 (hx_swap)
+                           284 LOAD_CLOSURE             7 (hx_target)
+                           286 LOAD_CLOSURE             2 (id)
+                           288 LOAD_CLOSURE             9 (tag)
+                           290 BUILD_TUPLE              6
+                           292 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 86>)
+                           294 MAKE_FUNCTION           12 (annotations, closure)
                
-                88         298 PRECALL                  0
-                           302 CALL                     0
+                86         296 PRECALL                  0
+                           300 CALL                     0
                
-                89         312 STORE_FAST               1 (inner)
+                87         310 STORE_FAST               1 (inner)
                
-               106         314 LOAD_FAST                1 (inner)
-                           316 RETURN_VALUE
+               104         312 LOAD_FAST                1 (inner)
+                           314 RETURN_VALUE
                consts
                   None
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
@@ -1089,94 +1214,94 @@
                         0000000000a00000000000000000000000000000000000000000006402a6
                         010000ab01000000000000000073027c0253007403000000000000000000
                         007c02740400000000000000000000a6020000ab02000000000000000072
                         027c0253007405000000000000000000007c0289078908890689058903ac
                         03a6060000ab0600000000000000005300
                                    0 COPY_FREE_VARS           6
                      
-                      88           2 RESUME                   0
+                      86           2 RESUME                   0
                      
-                      90           4 PUSH_NULL
+                      88           4 PUSH_NULL
                                    6 LOAD_DEREF               4 (f)
                                    8 LOAD_FAST                0 (args)
                                   10 BUILD_MAP                0
                                   12 LOAD_FAST                1 (kwargs)
                                   14 DICT_MERGE               1
                                   16 CALL_FUNCTION_EX         1
                                   18 STORE_FAST               2 (response)
                      
-                      91          20 LOAD_FAST                2 (response)
+                      89          20 LOAD_FAST                2 (response)
                                   22 LOAD_CONST               1 ('Content-Type')
                                   24 BINARY_SUBSCR
                                   34 LOAD_METHOD              0 (startswith)
                                   56 LOAD_CONST               2 ('text/html')
                                   58 PRECALL                  1
                                   62 CALL                     1
                                   72 POP_JUMP_FORWARD_IF_TRUE     2 (to 78)
                      
-                      92          74 LOAD_FAST                2 (response)
+                      90          74 LOAD_FAST                2 (response)
                                   76 RETURN_VALUE
                      
-                      94     >>   78 LOAD_GLOBAL              3 (NULL + isinstance)
+                      92     >>   78 LOAD_GLOBAL              3 (NULL + isinstance)
                                   90 LOAD_FAST                2 (response)
                                   92 LOAD_GLOBAL              4 (ElementResponse)
                                  104 PRECALL                  2
                                  108 CALL                     2
                                  118 POP_JUMP_FORWARD_IF_FALSE     2 (to 124)
                      
-                      95         120 LOAD_FAST                2 (response)
+                      93         120 LOAD_FAST                2 (response)
                                  122 RETURN_VALUE
                      
-                      97     >>  124 LOAD_GLOBAL              5 (NULL + ElementResponse)
+                      95     >>  124 LOAD_GLOBAL              5 (NULL + ElementResponse)
                      
-                      98         136 LOAD_FAST                2 (response)
+                      96         136 LOAD_FAST                2 (response)
                      
-                      99         138 LOAD_DEREF               7 (id)
+                      97         138 LOAD_DEREF               7 (id)
                      
-                     100         140 LOAD_DEREF               8 (tag)
+                      98         140 LOAD_DEREF               8 (tag)
                      
-                     101         142 LOAD_DEREF               6 (hx_target)
+                      99         142 LOAD_DEREF               6 (hx_target)
                      
-                     102         144 LOAD_DEREF               5 (hx_swap)
+                     100         144 LOAD_DEREF               5 (hx_swap)
                      
-                     103         146 LOAD_DEREF               3 (classes)
+                     101         146 LOAD_DEREF               3 (classes)
                      
-                      97         148 KW_NAMES                 3
+                      95         148 KW_NAMES                 3
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
-                     firstlineno 88
+                     firstlineno 86
                      lnotab 0x04021001360104022a0104020c010201020102010201020102fa
-               names      ('isinstance', 'str', '__name__', '_inject_args', 'auth_decorators', 'login_required', 'functools', 'wraps', 'P', 'args', 'kwargs', 'HttpResponse')
+               names      ('isinstance', 'str', '__name__', 'view', 'auth_decorators', 'login_required', 'functools', 'wraps', 'P', 'args', 'kwargs', 'HttpResponse')
                varnames   ('f', 'inner')
                freevars   ('classes', 'element_id', 'handle_args', 'hx_swap', 'hx_target', 'login_required', 'tag')
                cellvars   ('f', 'id')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
                firstlineno 79
-               lnotab 0x08013c0204012e0204013802260152ff0e010211
+               lnotab 0x08013c01300204013802260152ff0e010211
          names      ('Callable', 'P', 'HttpResponse')
          varnames   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required', 'decorator')
          freevars   ()
          cellvars   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'element'
          firstlineno 69
-         lnotab 0x100a7c1d
+         lnotab 0x100a7c1b
       'additional'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1188,92 +1313,599 @@
             0000000000000000000000000000006401a6010000ab0100000000000000
             007d057c05800f740f000000000000000000006402a6010000ab01000000
             000000000082017c029b0064037c059b009d037c046a0500000000000000
             0064043c0000007c0078016a080000000000000000740400000000000000
             0000006a030000000000000000a009000000000000000000000000000000
             00000000007c04a6010000ab0100000000000000007a0d000063025f0800
             000000000000007c005300
-         111           0 RESUME                   0
+         109           0 RESUME                   0
          
-         114           2 LOAD_GLOBAL              1 (NULL + response_to_str)
+         112           2 LOAD_GLOBAL              1 (NULL + response_to_str)
                       14 LOAD_FAST                1 (additional)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_METHOD              1 (strip)
                       52 PRECALL                  0
                       56 CALL                     0
                       66 STORE_FAST               3 (oob_content)
          
-         115          68 LOAD_GLOBAL              4 (lxml)
+         113          68 LOAD_GLOBAL              4 (lxml)
                       80 LOAD_ATTR                3 (html)
                       90 LOAD_METHOD              4 (fromstring)
                      112 LOAD_FAST                3 (oob_content)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 STORE_FAST               4 (parsed)
          
-         116         130 LOAD_FAST                4 (parsed)
+         114         130 LOAD_FAST                4 (parsed)
                      132 LOAD_ATTR                5 (attrib)
                      142 LOAD_METHOD              6 (get)
                      164 LOAD_CONST               1 ('id')
                      166 PRECALL                  1
                      170 CALL                     1
                      180 STORE_FAST               5 (id)
          
-         117         182 LOAD_FAST                5 (id)
+         115         182 LOAD_FAST                5 (id)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 216)
          
-         118         186 LOAD_GLOBAL             15 (NULL + Exception)
+         116         186 LOAD_GLOBAL             15 (NULL + Exception)
          
-         119         198 LOAD_CONST               2 ('The additional response does not contain exactly one element with an id attribute.')
+         117         198 LOAD_CONST               2 ('The additional response does not contain exactly one element with an id attribute.')
          
-         118         200 PRECALL                  1
+         116         200 PRECALL                  1
                      204 CALL                     1
                      214 RAISE_VARARGS            1
          
-         122     >>  216 LOAD_FAST                2 (hx_swap_oob_method)
+         120     >>  216 LOAD_FAST                2 (hx_swap_oob_method)
                      218 FORMAT_VALUE             0
                      220 LOAD_CONST               3 (':#')
                      222 LOAD_FAST                5 (id)
                      224 FORMAT_VALUE             0
                      226 BUILD_STRING             3
                      228 LOAD_FAST                4 (parsed)
                      230 LOAD_ATTR                5 (attrib)
                      240 LOAD_CONST               4 ('hx-swap-oob')
                      242 STORE_SUBSCR
          
-         123         246 LOAD_FAST                0 (response)
+         121         246 LOAD_FAST                0 (response)
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
          
-         124         336 LOAD_FAST                0 (response)
+         122         336 LOAD_FAST                0 (response)
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
-         firstlineno 111
+         firstlineno 109
          lnotab 0x020342013e01340104010c0102ff10041e015a01
+      'request'
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 1
+         flags     : 3
+         code 0x970064005300
+         130           0 RESUME                   0
+         
+         132           2 LOAD_CONST               0 (None)
+                       4 RETURN_VALUE
+         consts
+            None
+         names      ()
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'get_view_fn_call_stack_from_request'
+         firstlineno 130
+         lnotab 0x0202
+      'create'
+      code
+         argcount  : 2
+         nlocals   : 2
+         stacksize : 1
+         flags     : 3
+         code 0x970064005300
+         135           0 RESUME                   0
+         
+         139           2 LOAD_CONST               0 (None)
+                       4 RETURN_VALUE
+         consts
+            None
+         names      ()
+         varnames   ('request', 'create')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'get_view_fn_call_stack_from_request'
+         firstlineno 135
+         lnotab 0x0204
+      code
+         argcount  : 2
+         nlocals   : 3
+         stacksize : 5
+         flags     : 3
+         code
+            0x97007401000000000000000000007c0064016400a6030000ab03000000
+            00000000007d027c0280047c01720267006e017c027d0274030000000000
+            00000000007c0064017c02a6030000ab03000000000000000001007c0253
+            00
+         142           0 RESUME                   0
+         
+         145           2 LOAD_GLOBAL              1 (NULL + getattr)
+                      14 LOAD_FAST                0 (request)
+                      16 LOAD_CONST               1 ('__dfv_view_fn_call_stack')
+                      18 LOAD_CONST               0 (None)
+                      20 PRECALL                  3
+                      24 CALL                     3
+                      34 STORE_FAST               2 (call_stack)
+         
+         146          36 LOAD_FAST                2 (call_stack)
+                      38 POP_JUMP_FORWARD_IF_NOT_NONE     4 (to 48)
+                      40 LOAD_FAST                1 (create)
+                      42 POP_JUMP_FORWARD_IF_FALSE     2 (to 48)
+                      44 BUILD_LIST               0
+                      46 JUMP_FORWARD             1 (to 50)
+                 >>   48 LOAD_FAST                2 (call_stack)
+                 >>   50 STORE_FAST               2 (call_stack)
+         
+         147          52 LOAD_GLOBAL              3 (NULL + setattr)
+                      64 LOAD_FAST                0 (request)
+                      66 LOAD_CONST               1 ('__dfv_view_fn_call_stack')
+                      68 LOAD_FAST                2 (call_stack)
+                      70 PRECALL                  3
+                      74 CALL                     3
+                      84 POP_TOP
+         
+         148          86 LOAD_FAST                2 (call_stack)
+                      88 RETURN_VALUE
+         consts
+            None
+            '__dfv_view_fn_call_stack'
+         names      ('getattr', 'setattr')
+         varnames   ('request', 'create', 'call_stack')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'get_view_fn_call_stack_from_request'
+         firstlineno 142
+         lnotab 0x0203220110012201
+      code
+         argcount  : 1
+         nlocals   : 2
+         stacksize : 6
+         flags     : 3
+         code
+            0x8700970064017400000000000000000000007402000000000000000000
+            007404000000000000000000006602190000000000000000006402740000
+            000000000000000000740200000000000000000000740400000000000000
+            0000006602190000000000000000006604880066016403840c7d017c0153
+            00
+                       0 MAKE_CELL                0 (handle_args)
+         
+         151           2 RESUME                   0
+         
+         152           4 LOAD_CONST               1 ('fn')
+                       6 LOAD_GLOBAL              0 (Callable)
+                      18 LOAD_GLOBAL              2 (P)
+                      30 LOAD_GLOBAL              4 (R)
+                      42 BUILD_TUPLE              2
+                      44 BINARY_SUBSCR
+                      54 LOAD_CONST               2 ('return')
+                      56 LOAD_GLOBAL              0 (Callable)
+                      68 LOAD_GLOBAL              2 (P)
+                      80 LOAD_GLOBAL              4 (R)
+                      92 BUILD_TUPLE              2
+                      94 BINARY_SUBSCR
+                     104 BUILD_TUPLE              4
+                     106 LOAD_CLOSURE             0 (handle_args)
+                     108 BUILD_TUPLE              1
+                     110 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 152>)
+                     112 MAKE_FUNCTION           12 (annotations, closure)
+                     114 STORE_FAST               1 (decorator)
+         
+         168         116 LOAD_FAST                1 (decorator)
+                     118 RETURN_VALUE
+         consts
+            None
+            'fn'
+            'return'
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 7
+               flags     : 19
+               code
+                  0x950187009700890272170200740100000000000000000000a6000000ab
+                  0000000000000000008900a6010000ab0100000000000000008a00740300
+                  0000000000000000006a0200000000000000008900a6010000ab01000000
+                  000000000064017406000000000000000000006a04000000000000000064
+                  027406000000000000000000006a0500000000000000006403740c000000
+                  000000000000006606880066016404840ca6000000ab0000000000000000
+                  007d017c015300
+                             0 COPY_FREE_VARS           1
+                             2 MAKE_CELL                0 (fn)
+               
+               152           4 RESUME                   0
+               
+               153           6 LOAD_DEREF               2 (handle_args)
+                             8 POP_JUMP_FORWARD_IF_FALSE    23 (to 56)
+               
+               154          10 PUSH_NULL
+                            12 LOAD_GLOBAL              1 (NULL + _inject_args)
+                            24 PRECALL                  0
+                            28 CALL                     0
+                            38 LOAD_DEREF               0 (fn)
+                            40 PRECALL                  1
+                            44 CALL                     1
+                            54 STORE_DEREF              0 (fn)
+               
+               156     >>   56 LOAD_GLOBAL              3 (NULL + functools)
+                            68 LOAD_ATTR                2 (wraps)
+                            78 LOAD_DEREF               0 (fn)
+                            80 PRECALL                  1
+                            84 CALL                     1
+               
+               157          94 LOAD_CONST               1 ('args')
+                            96 LOAD_GLOBAL              6 (P)
+                           108 LOAD_ATTR                4 (args)
+                           118 LOAD_CONST               2 ('kwargs')
+                           120 LOAD_GLOBAL              6 (P)
+                           132 LOAD_ATTR                5 (kwargs)
+                           142 LOAD_CONST               3 ('return')
+                           144 LOAD_GLOBAL             12 (R)
+                           156 BUILD_TUPLE              6
+                           158 LOAD_CLOSURE             0 (fn)
+                           160 BUILD_TUPLE              1
+                           162 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 156>)
+                           164 MAKE_FUNCTION           12 (annotations, closure)
+               
+               156         166 PRECALL                  0
+                           170 CALL                     0
+               
+               157         180 STORE_FAST               1 (inner)
+               
+               166         182 LOAD_FAST                1 (inner)
+                           184 RETURN_VALUE
+               consts
+                  None
+                  'args'
+                  'kwargs'
+                  'return'
+                  code
+                     argcount  : 0
+                     nlocals   : 4
+                     stacksize : 5
+                     flags     : 31
+                     code
+                        0x950197007c006401190000000000000000007d02740100000000000000
+                        0000007c02a6010000ab0100000000000000007d0309007c03a001000000
+                        00000000000000000000000000000000008904a6010000ab010000000000
+                        0000000100020089047c0069007c01a4018e017c03a00200000000000000
+                        00000000000000000000000000a6000000ab000000000000000000010053
+                        0023007c03a0020000000000000000000000000000000000000000a60000
+                        00ab00000000000000000001007700780359007701
+                                   0 COPY_FREE_VARS           1
+                     
+                     156           2 RESUME                   0
+                     
+                     158           4 LOAD_FAST                0 (args)
+                                   6 LOAD_CONST               1 (0)
+                                   8 BINARY_SUBSCR
+                                  18 STORE_FAST               2 (view_request)
+                     
+                     159          20 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
+                                  32 LOAD_FAST                2 (view_request)
+                                  34 PRECALL                  1
+                                  38 CALL                     1
+                                  48 STORE_FAST               3 (stack)
+                     
+                     160          50 NOP
+                     
+                     161          52 LOAD_FAST                3 (stack)
+                                  54 LOAD_METHOD              1 (append)
+                                  76 LOAD_DEREF               4 (fn)
+                                  78 PRECALL                  1
+                                  82 CALL                     1
+                                  92 POP_TOP
+                     
+                     162          94 PUSH_NULL
+                                  96 LOAD_DEREF               4 (fn)
+                                  98 LOAD_FAST                0 (args)
+                                 100 BUILD_MAP                0
+                                 102 LOAD_FAST                1 (kwargs)
+                                 104 DICT_MERGE               1
+                                 106 CALL_FUNCTION_EX         1
+                     
+                     164         108 LOAD_FAST                3 (stack)
+                                 110 LOAD_METHOD              2 (pop)
+                                 132 PRECALL                  0
+                                 136 CALL                     0
+                                 146 POP_TOP
+                                 148 RETURN_VALUE
+                             >>  150 PUSH_EXC_INFO
+                                 152 LOAD_FAST                3 (stack)
+                                 154 LOAD_METHOD              2 (pop)
+                                 176 PRECALL                  0
+                                 180 CALL                     0
+                                 190 POP_TOP
+                                 192 RERAISE                  0
+                             >>  194 COPY                     3
+                                 196 POP_EXCEPT
+                                 198 RERAISE                  1
+                     ExceptionTable:
+                       52 to 106 -> 150 [0]
+                       150 to 192 -> 194 [1] lasti
+                     consts
+                        None
+                        0
+                     names      ('get_view_fn_call_stack_from_request', 'append', 'pop')
+                     varnames   ('args', 'kwargs', 'view_request', 'stack')
+                     freevars   ('fn',)
+                     cellvars   ()
+                     filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+                     name       'inner'
+                     firstlineno 156
+                     lnotab 0x040210011e0102012a010e02
+               names      ('_inject_args', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
+               varnames   ('fn', 'inner')
+               freevars   ('handle_args',)
+               cellvars   ('fn',)
+               filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+               name       'decorator'
+               firstlineno 152
+               lnotab 0x060104012e02260148ff0e010209
+         names      ('Callable', 'P', 'R')
+         varnames   ('handle_args', 'decorator')
+         freevars   ()
+         cellvars   ('handle_args',)
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'view'
+         firstlineno 151
+         lnotab 0x04017010
+      code
+         argcount  : 1
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007c006401ac02a6020000ab02000000
+            00000000007d017c016400750070127403000000000000000000007c01a6
+            010000ab01000000000000000064036b02000000005300
+         171           0 RESUME                   0
+         
+         172           2 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
+                      14 LOAD_FAST                0 (request)
+                      16 LOAD_CONST               1 (False)
+                      18 KW_NAMES                 2
+                      20 PRECALL                  2
+                      24 CALL                     2
+                      34 STORE_FAST               1 (stack)
+         
+         173          36 LOAD_FAST                1 (stack)
+                      38 LOAD_CONST               0 (None)
+                      40 IS_OP                    0
+                      42 JUMP_IF_TRUE_OR_POP     18 (to 80)
+                      44 LOAD_GLOBAL              3 (NULL + len)
+                      56 LOAD_FAST                1 (stack)
+                      58 PRECALL                  1
+                      62 CALL                     1
+                      72 LOAD_CONST               3 (1)
+                      74 COMPARE_OP               2 (==)
+                 >>   80 RETURN_VALUE
+         consts
+            None
+            False
+            ('create',)
+            1
+         names      ('get_view_fn_call_stack_from_request', 'len')
+         varnames   ('request', 'stack')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_view_fn_request_target'
+         firstlineno 171
+         lnotab 0x02012201
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 3
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            006f0a7c006a01000000000000000064016b02000000005300
+         176           0 RESUME                   0
+         
+         177           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+                      14 LOAD_FAST                0 (request)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 JUMP_IF_FALSE_OR_POP    10 (to 52)
+                      32 LOAD_FAST                0 (request)
+                      34 LOAD_ATTR                1 (method)
+                      44 LOAD_CONST               1 ('HEAD')
+                      46 COMPARE_OP               2 (==)
+                 >>   52 RETURN_VALUE
+         consts
+            None
+            'HEAD'
+         names      ('is_view_fn_request_target', 'method')
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_head'
+         firstlineno 176
+         lnotab 0x0201
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 2
+         flags     : 3
+         code 0x97007c006a00000000000000000064016b02000000005300
+         180           0 RESUME                   0
+         
+         181           2 LOAD_FAST                0 (request)
+                       4 LOAD_ATTR                0 (method)
+                      14 LOAD_CONST               1 ('GET')
+                      16 COMPARE_OP               2 (==)
+                      22 RETURN_VALUE
+         consts
+            None
+            'GET'
+         names      ('method',)
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_get'
+         firstlineno 180
+         lnotab 0x0201
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 3
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            006f0a7c006a01000000000000000064016b02000000005300
+         184           0 RESUME                   0
+         
+         185           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+                      14 LOAD_FAST                0 (request)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 JUMP_IF_FALSE_OR_POP    10 (to 52)
+                      32 LOAD_FAST                0 (request)
+                      34 LOAD_ATTR                1 (method)
+                      44 LOAD_CONST               1 ('POST')
+                      46 COMPARE_OP               2 (==)
+                 >>   52 RETURN_VALUE
+         consts
+            None
+            'POST'
+         names      ('is_view_fn_request_target', 'method')
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_post'
+         firstlineno 184
+         lnotab 0x0201
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 3
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            006f0a7c006a01000000000000000064016b02000000005300
+         188           0 RESUME                   0
+         
+         189           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+                      14 LOAD_FAST                0 (request)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 JUMP_IF_FALSE_OR_POP    10 (to 52)
+                      32 LOAD_FAST                0 (request)
+                      34 LOAD_ATTR                1 (method)
+                      44 LOAD_CONST               1 ('PUT')
+                      46 COMPARE_OP               2 (==)
+                 >>   52 RETURN_VALUE
+         consts
+            None
+            'PUT'
+         names      ('is_view_fn_request_target', 'method')
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_put'
+         firstlineno 188
+         lnotab 0x0201
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 3
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            006f0a7c006a01000000000000000064016b02000000005300
+         192           0 RESUME                   0
+         
+         193           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+                      14 LOAD_FAST                0 (request)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 JUMP_IF_FALSE_OR_POP    10 (to 52)
+                      32 LOAD_FAST                0 (request)
+                      34 LOAD_ATTR                1 (method)
+                      44 LOAD_CONST               1 ('PATCH')
+                      46 COMPARE_OP               2 (==)
+                 >>   52 RETURN_VALUE
+         consts
+            None
+            'PATCH'
+         names      ('is_view_fn_request_target', 'method')
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_patch'
+         firstlineno 192
+         lnotab 0x0201
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 3
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            006f0a7c006a01000000000000000064016b02000000005300
+         196           0 RESUME                   0
+         
+         197           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+                      14 LOAD_FAST                0 (request)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 JUMP_IF_FALSE_OR_POP    10 (to 52)
+                      32 LOAD_FAST                0 (request)
+                      34 LOAD_ATTR                1 (method)
+                      44 LOAD_CONST               1 ('DELETE')
+                      46 COMPARE_OP               2 (==)
+                 >>   52 RETURN_VALUE
+         consts
+            None
+            'DELETE'
+         names      ('is_view_fn_request_target', 'method')
+         varnames   ('request',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
+         name       'is_delete'
+         firstlineno 196
+         lnotab 0x0201
       ('auto_param', 'auto_form')
       'auto_param'
       ('get', 'post')
       'auto_form'
       code
          argcount  : 0
          nlocals   : 3
@@ -1284,17 +1916,17 @@
             000000740400000000000000000000660219000000000000000000640274
             000000000000000000000074020000000000000000000074040000000000
             000000000066021900000000000000000066048801880066026403840c7d
             027c025300
                        0 MAKE_CELL                0 (auto_param)
                        2 MAKE_CELL                1 (auto_form)
          
-         132           4 RESUME                   0
+         205           4 RESUME                   0
          
-         137           6 LOAD_CONST               1 ('fn')
+         210           6 LOAD_CONST               1 ('fn')
                        8 LOAD_GLOBAL              0 (Callable)
                       20 LOAD_GLOBAL              2 (P)
                       32 LOAD_GLOBAL              4 (R)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('return')
                       58 LOAD_GLOBAL              0 (Callable)
@@ -1302,19 +1934,19 @@
                       82 LOAD_GLOBAL              4 (R)
                       94 BUILD_TUPLE              2
                       96 BINARY_SUBSCR
                      106 BUILD_TUPLE              4
                      108 LOAD_CLOSURE             1 (auto_form)
                      110 LOAD_CLOSURE             0 (auto_param)
                      112 BUILD_TUPLE              2
-                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 137>)
+                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 210>)
                      116 MAKE_FUNCTION           12 (annotations, closure)
                      118 STORE_FAST               2 (decorator)
          
-         160         120 LOAD_FAST                2 (decorator)
+         235         120 LOAD_FAST                2 (decorator)
                      122 RETURN_VALUE
          consts
             None
             'fn'
             'return'
             code
                argcount  : 1
@@ -1322,98 +1954,101 @@
                stacksize : 7
                flags     : 19
                code
                   0x9502870087038704970074010000000000000000000074030000000000
                   00000000006a0200000000000000008900a6010000ab0100000000000000
                   006a030000000000000000a0040000000000000000000000000000000000
                   000000a6000000ab000000000000000000a6010000ab0100000000000000
-                  007d01740b000000000000000000007c0189068905a6030000ab03000000
-                  00000000008a04640184007c014400a6000000ab0000000000000000008a
-                  03740d000000000000000000006a0700000000000000008900a6010000ab
-                  01000000000000000064027410000000000000000000006a090000000000
-                  00000064037410000000000000000000006a0a0000000000000000640474
-                  1600000000000000000000660688038800880466036405840ca6000000ab
-                  0000000000000000007d027c025300
+                  007d01740b0000000000000000000089007c0189068905a6040000ab0400
+                  000000000000008a04640184007c014400a6000000ab0000000000000000
+                  008a03740d000000000000000000006a0700000000000000008900a60100
+                  00ab01000000000000000064027410000000000000000000006a09000000
+                  000000000064037410000000000000000000006a0a000000000000000064
+                  04741600000000000000000000660688038800880466036405840ca60000
+                  00ab0000000000000000007d027c025300
                              0 COPY_FREE_VARS           2
                              2 MAKE_CELL                0 (fn)
                              4 MAKE_CELL                3 (arg_names)
                              6 MAKE_CELL                4 (injected_params)
                
-               137           8 RESUME                   0
+               210           8 RESUME                   0
                
-               138          10 LOAD_GLOBAL              1 (NULL + list)
+               211          10 LOAD_GLOBAL              1 (NULL + list)
                
-               139          22 LOAD_GLOBAL              3 (NULL + inspect)
+               212          22 LOAD_GLOBAL              3 (NULL + inspect)
                             34 LOAD_ATTR                2 (signature)
                             44 LOAD_DEREF               0 (fn)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 LOAD_ATTR                3 (parameters)
                             70 LOAD_METHOD              4 (values)
                             92 PRECALL                  0
                             96 CALL                     0
                
-               138         106 PRECALL                  1
+               211         106 PRECALL                  1
                            110 CALL                     1
                            120 STORE_FAST               1 (parameters)
                
-               141         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
-                           134 LOAD_FAST                1 (parameters)
-                           136 LOAD_DEREF               6 (auto_param)
-                           138 LOAD_DEREF               5 (auto_form)
-                           140 PRECALL                  3
-                           144 CALL                     3
-                           154 STORE_DEREF              4 (injected_params)
-               
-               142         156 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 142>)
-                           158 MAKE_FUNCTION            0
-                           160 LOAD_FAST                1 (parameters)
-                           162 GET_ITER
-                           164 PRECALL                  0
-                           168 CALL                     0
-                           178 STORE_DEREF              3 (arg_names)
-               
-               144         180 LOAD_GLOBAL             13 (NULL + functools)
-                           192 LOAD_ATTR                7 (wraps)
-                           202 LOAD_DEREF               0 (fn)
-                           204 PRECALL                  1
-                           208 CALL                     1
-               
-               145         218 LOAD_CONST               2 ('args')
-                           220 LOAD_GLOBAL             16 (P)
-                           232 LOAD_ATTR                9 (args)
-                           242 LOAD_CONST               3 ('kwargs')
-                           244 LOAD_GLOBAL             16 (P)
-                           256 LOAD_ATTR               10 (kwargs)
-                           266 LOAD_CONST               4 ('return')
-                           268 LOAD_GLOBAL             22 (R)
-                           280 BUILD_TUPLE              6
-                           282 LOAD_CLOSURE             3 (arg_names)
-                           284 LOAD_CLOSURE             0 (fn)
-                           286 LOAD_CLOSURE             4 (injected_params)
-                           288 BUILD_TUPLE              3
-                           290 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 144>)
-                           292 MAKE_FUNCTION           12 (annotations, closure)
+               214         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
                
-               144         294 PRECALL                  0
-                           298 CALL                     0
+               215         134 LOAD_DEREF               0 (fn)
+                           136 LOAD_FAST                1 (parameters)
+                           138 LOAD_DEREF               6 (auto_param)
+                           140 LOAD_DEREF               5 (auto_form)
+               
+               214         142 PRECALL                  4
+                           146 CALL                     4
+                           156 STORE_DEREF              4 (injected_params)
+               
+               217         158 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 217>)
+                           160 MAKE_FUNCTION            0
+                           162 LOAD_FAST                1 (parameters)
+                           164 GET_ITER
+                           166 PRECALL                  0
+                           170 CALL                     0
+                           180 STORE_DEREF              3 (arg_names)
+               
+               219         182 LOAD_GLOBAL             13 (NULL + functools)
+                           194 LOAD_ATTR                7 (wraps)
+                           204 LOAD_DEREF               0 (fn)
+                           206 PRECALL                  1
+                           210 CALL                     1
                
-               145         308 STORE_FAST               2 (inner)
+               220         220 LOAD_CONST               2 ('args')
+                           222 LOAD_GLOBAL             16 (P)
+                           234 LOAD_ATTR                9 (args)
+                           244 LOAD_CONST               3 ('kwargs')
+                           246 LOAD_GLOBAL             16 (P)
+                           258 LOAD_ATTR               10 (kwargs)
+                           268 LOAD_CONST               4 ('return')
+                           270 LOAD_GLOBAL             22 (R)
+                           282 BUILD_TUPLE              6
+                           284 LOAD_CLOSURE             3 (arg_names)
+                           286 LOAD_CLOSURE             0 (fn)
+                           288 LOAD_CLOSURE             4 (injected_params)
+                           290 BUILD_TUPLE              3
+                           292 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 219>)
+                           294 MAKE_FUNCTION           12 (annotations, closure)
                
-               158         310 LOAD_FAST                2 (inner)
-                           312 RETURN_VALUE
+               219         296 PRECALL                  0
+                           300 CALL                     0
+               
+               220         310 STORE_FAST               2 (inner)
+               
+               233         312 LOAD_FAST                2 (inner)
+                           314 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     142           0 RESUME                   0
+                     217           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (p)
                                   10 LOAD_FAST                1 (p)
                                   12 LOAD_ATTR                0 (name)
                                   22 LIST_APPEND              2
@@ -1422,15 +2057,15 @@
                      consts
                      names      ('name',)
                      varnames   ('.0', 'p')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<listcomp>'
-                     firstlineno 142
+                     firstlineno 217
                      lnotab 0x
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
                      nlocals   : 6
@@ -1448,90 +2083,90 @@
                         020000ab020000000000000000a6010000ab0100000000000000007c017c
                         0319000000000000000000a6020000ab0200000000000000007d057c0581
                         1c740b000000000000000000006a06000000000000000074100000000000
                         00000000007c05a6020000ab0200000000000000006302010053008c8602
                         0089077c0069007c01a4018e015300
                                    0 COPY_FREE_VARS           3
                      
-                     144           2 RESUME                   0
+                     219           2 RESUME                   0
                      
-                     146           4 LOAD_DEREF               6 (arg_names)
+                     221           4 LOAD_DEREF               6 (arg_names)
                                    6 LOAD_CONST               0 (None)
                                    8 LOAD_GLOBAL              1 (NULL + len)
                                   20 LOAD_FAST                0 (args)
                                   22 PRECALL                  1
                                   26 CALL                     1
                                   36 BUILD_SLICE              2
                                   38 BINARY_SUBSCR
                                   48 STORE_FAST               2 (supplied_args)
                      
-                     147          50 LOAD_DEREF               8 (injected_params)
+                     222          50 LOAD_DEREF               8 (injected_params)
                                   52 LOAD_METHOD              1 (items)
                                   74 PRECALL                  0
                                   78 CALL                     0
                                   88 GET_ITER
                              >>   90 FOR_ITER               133 (to 358)
                                   92 UNPACK_SEQUENCE          2
                                   96 STORE_FAST               3 (name)
                                   98 STORE_FAST               4 (ip)
                      
-                     148         100 LOAD_FAST                3 (name)
+                     223         100 LOAD_FAST                3 (name)
                                  102 LOAD_FAST                1 (kwargs)
                                  104 CONTAINS_OP              1
                                  106 POP_JUMP_FORWARD_IF_FALSE   124 (to 356)
                                  108 LOAD_FAST                3 (name)
                                  110 LOAD_FAST                2 (supplied_args)
                                  112 CONTAINS_OP              1
                                  114 POP_JUMP_FORWARD_IF_FALSE   120 (to 356)
                      
-                     149         116 LOAD_FAST                4 (ip)
+                     224         116 LOAD_FAST                4 (ip)
                                  118 LOAD_METHOD              2 (get_value)
                                  140 LOAD_FAST                0 (args)
                                  142 LOAD_FAST                1 (kwargs)
                                  144 PRECALL                  2
                                  148 CALL                     2
                                  158 LOAD_FAST                1 (kwargs)
                                  160 LOAD_FAST                3 (name)
                                  162 STORE_SUBSCR
                      
-                     150         166 LOAD_FAST                4 (ip)
+                     225         166 LOAD_FAST                4 (ip)
                                  168 LOAD_METHOD              3 (replace_response)
                      
-                     151         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
+                     226         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
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
                      
-                     150         280 PRECALL                  2
+                     225         280 PRECALL                  2
                                  284 CALL                     2
                                  294 STORE_FAST               5 (replace_response)
                      
-                     153         296 LOAD_FAST                5 (replace_response)
+                     228         296 LOAD_FAST                5 (replace_response)
                                  298 POP_JUMP_FORWARD_IF_NONE    28 (to 356)
                      
-                     154         300 LOAD_GLOBAL             11 (NULL + typing)
+                     229         300 LOAD_GLOBAL             11 (NULL + typing)
                                  312 LOAD_ATTR                6 (cast)
                                  322 LOAD_GLOBAL             16 (R)
                                  334 LOAD_FAST                5 (replace_response)
                                  336 PRECALL                  2
                                  340 CALL                     2
                                  350 SWAP                     2
                                  352 POP_TOP
                                  354 RETURN_VALUE
                              >>  356 JUMP_BACKWARD          134 (to 90)
                      
-                     156     >>  358 PUSH_NULL
+                     231     >>  358 PUSH_NULL
                                  360 LOAD_DEREF               7 (fn)
                                  362 LOAD_FAST                0 (args)
                                  364 BUILD_MAP                0
                                  366 LOAD_FAST                1 (kwargs)
                                  368 DICT_MERGE               1
                                  370 CALL_FUNCTION_EX         1
                                  372 RETURN_VALUE
@@ -1539,669 +2174,683 @@
                         None
                      names      ('len', 'items', 'get_value', 'replace_response', '_get_request_from_args', 'typing', 'cast', 'Any', 'R')
                      varnames   ('args', 'kwargs', 'supplied_args', 'name', 'ip', 'replace_response')
                      freevars   ('arg_names', 'fn', 'injected_params')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 144
+                     firstlineno 219
                      lnotab 0x04022e0132011001320118015aff100304013a02
                names      ('list', 'inspect', 'signature', 'parameters', 'values', '_extract_injected_params', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
                varnames   ('fn', 'parameters', 'inner')
                freevars   ('auto_form', 'auto_param')
                cellvars   ('fn', 'arg_names', 'injected_params')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 137
-               lnotab 0x0a010c0154ff10032201180226014cff0e01020d
+               firstlineno 210
+               lnotab 0x0a010c0154ff10030c0108ff1003180226014cff0e01020d
          names      ('Callable', 'P', 'R')
          varnames   ('auto_param', 'auto_form', 'decorator')
          freevars   ()
          cellvars   ('auto_param', 'auto_form')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'inject_args'
-         firstlineno 132
-         lnotab 0x06057217
+         firstlineno 205
+         lnotab 0x06057219
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a025500020065036a0400000000000000006401ac
             02a6010000ab0100000000000000005a056506650764033c000000020065
             036a0400000000000000006401ac02a6010000ab0100000000000000005a
-            086509650764043c000000640584005a0a6406650b6407650c6506650b66
-            02190000000000000000006408650b6606640984045a0d640a650e640b65
-            0b6408650f6510190000000000000000006606640c84045a11640d5300
-         167           0 RESUME                   0
+            086509650764043c000000020065036a0400000000000000006401ac02a6
+            010000ab0100000000000000005a0a650b650c6701650c66021900000000
+            0000000000650764053c000000640684005a0d6407650c6408650e650665
+            0c6602190000000000000000006409650c6606640a84045a0f640b651064
+            0c650c640965116512190000000000000000006606640d84045a13640e53
+            00
+         242           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParam')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         169          12 PUSH_NULL
+         244          12 PUSH_NULL
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
          
-         170          56 PUSH_NULL
+         245          56 PUSH_NULL
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
          
-         172         100 LOAD_CONST               5 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 172>)
-                     102 MAKE_FUNCTION            0
-                     104 STORE_NAME              10 (check)
-         
-         175         106 LOAD_CONST               6 ('args')
-                     108 LOAD_NAME               11 (Any)
-                     110 LOAD_CONST               7 ('kwargs')
-                     112 LOAD_NAME               12 (dict)
-                     114 LOAD_NAME                6 (str)
-                     116 LOAD_NAME               11 (Any)
-                     118 BUILD_TUPLE              2
-                     120 BINARY_SUBSCR
-                     130 LOAD_CONST               8 ('return')
-                     132 LOAD_NAME               11 (Any)
-                     134 BUILD_TUPLE              6
-                     136 LOAD_CONST               9 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 175>)
-                     138 MAKE_FUNCTION            4 (annotations)
-                     140 STORE_NAME              13 (get_value)
-         
-         178         142 LOAD_CONST              10 ('request')
-         
-         179         144 LOAD_NAME               14 (HttpRequest)
-         
-         178         146 LOAD_CONST              11 ('value')
-         
-         179         148 LOAD_NAME               11 (Any)
-         
-         178         150 LOAD_CONST               8 ('return')
-         
-         180         152 LOAD_NAME               15 (Optional)
-                     154 LOAD_NAME               16 (HttpResponse)
-                     156 BINARY_SUBSCR
-         
-         178         166 BUILD_TUPLE              6
-                     168 LOAD_CONST              12 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 178>)
-                     170 MAKE_FUNCTION            4 (annotations)
-                     172 STORE_NAME              17 (replace_response)
-                     174 LOAD_CONST              13 (None)
-                     176 RETURN_VALUE
+         246         100 PUSH_NULL
+                     102 LOAD_NAME                3 (dataclasses)
+                     104 LOAD_ATTR                4 (field)
+                     114 LOAD_CONST               1 (False)
+                     116 KW_NAMES                 2
+                     118 PRECALL                  1
+                     122 CALL                     1
+                     132 STORE_NAME              10 (view_fn)
+                     134 LOAD_NAME               11 (Callable)
+                     136 LOAD_NAME               12 (Any)
+                     138 BUILD_LIST               1
+                     140 LOAD_NAME               12 (Any)
+                     142 BUILD_TUPLE              2
+                     144 BINARY_SUBSCR
+                     154 LOAD_NAME                7 (__annotations__)
+                     156 LOAD_CONST               5 ('view_fn')
+                     158 STORE_SUBSCR
+         
+         248         162 LOAD_CONST               6 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 248>)
+                     164 MAKE_FUNCTION            0
+                     166 STORE_NAME              13 (check)
+         
+         251         168 LOAD_CONST               7 ('args')
+                     170 LOAD_NAME               12 (Any)
+                     172 LOAD_CONST               8 ('kwargs')
+                     174 LOAD_NAME               14 (dict)
+                     176 LOAD_NAME                6 (str)
+                     178 LOAD_NAME               12 (Any)
+                     180 BUILD_TUPLE              2
+                     182 BINARY_SUBSCR
+                     192 LOAD_CONST               9 ('return')
+                     194 LOAD_NAME               12 (Any)
+                     196 BUILD_TUPLE              6
+                     198 LOAD_CONST              10 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 251>)
+                     200 MAKE_FUNCTION            4 (annotations)
+                     202 STORE_NAME              15 (get_value)
+         
+         254         204 LOAD_CONST              11 ('request')
+         
+         255         206 LOAD_NAME               16 (HttpRequest)
+         
+         254         208 LOAD_CONST              12 ('value')
+         
+         255         210 LOAD_NAME               12 (Any)
+         
+         254         212 LOAD_CONST               9 ('return')
+         
+         256         214 LOAD_NAME               17 (Optional)
+                     216 LOAD_NAME               18 (HttpResponse)
+                     218 BINARY_SUBSCR
+         
+         254         228 BUILD_TUPLE              6
+                     230 LOAD_CONST              13 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 254>)
+                     232 MAKE_FUNCTION            4 (annotations)
+                     234 STORE_NAME              19 (replace_response)
+                     236 LOAD_CONST              14 (None)
+                     238 RETURN_VALUE
          consts
             'InjectedParam'
             False
             ('init',)
             'name'
             'target_type'
+            'view_fn'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               172           0 RESUME                   0
+               248           0 RESUME                   0
                
-               173           2 LOAD_CONST               0 (None)
+               249           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 172
+               firstlineno 248
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
-               175           0 RESUME                   0
+               251           0 RESUME                   0
                
-               176           2 LOAD_CONST               0 (None)
+               252           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 175
+               firstlineno 251
                lnotab 0x0201
             'request'
             'value'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               178           0 RESUME                   0
+               254           0 RESUME                   0
                
-               181           2 LOAD_CONST               0 (None)
+               257           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'request', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 178
+               firstlineno 254
                lnotab 0x0203
             None
-         names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'name', 'str', '__annotations__', 'target_type', 'type', 'check', 'Any', 'dict', 'get_value', 'HttpRequest', 'Optional', 'HttpResponse', 'replace_response')
+         names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'name', 'str', '__annotations__', 'target_type', 'type', 'view_fn', 'Callable', 'Any', 'check', 'dict', 'get_value', 'HttpRequest', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParam'
-         firstlineno 167
-         lnotab 0x0c022c012c0206032403020102ff020102ff02020efe
+         firstlineno 242
+         lnotab 0x0c022c012c013e0206032403020102ff020102ff02020efe
       'InjectedParam'
+      'view_fn'
       'ip'
       'name'
       'parameter'
       code
-         argcount  : 3
-         nlocals   : 3
+         argcount  : 4
+         nlocals   : 4
          stacksize : 4
          flags     : 3
          code
-            0x97007c017c005f0000000000000000007c026a01000000000000000074
+            0x97007c027c015f0000000000000000007c036a01000000000000000074
             04000000000000000000006a0300000000000000006a0400000000000000
-            00750172077c026a0100000000000000006e8b7c026a0500000000000000
+            00750172077c036a0100000000000000006e8b7c036a0500000000000000
             007404000000000000000000006a0600000000000000006a040000000000
-            0000007501722e740f000000000000000000007c026a0500000000000000
+            0000007501722e740f000000000000000000007c036a0500000000000000
             00741000000000000000000000a6020000ab020000000000000000731474
-            13000000000000000000007c026a050000000000000000a6010000ab0100
-            000000000000006e45740f000000000000000000007c026a050000000000
+            13000000000000000000007c036a050000000000000000a6010000ab0100
+            000000000000006e45740f000000000000000000007c036a050000000000
             000000741400000000000000000000a6020000ab02000000000000000072
-            257c026a0500000000000000006a05000000000000000081197413000000
-            000000000000007c026a0500000000000000006a050000000000000000a6
-            010000ab0100000000000000006e067416000000000000000000007c005f
-            0c00000000000000007c00a00d0000000000000000000000000000000000
-            000000a6000000ab00000000000000000001007c005300
-         184           0 RESUME                   0
+            257c036a0500000000000000006a05000000000000000081197413000000
+            000000000000007c036a0500000000000000006a050000000000000000a6
+            010000ab0100000000000000006e067416000000000000000000007c015f
+            0c00000000000000007c007c015f0d00000000000000007c01a00e000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0001007c015300
+         260           0 RESUME                   0
          
-         185           2 LOAD_FAST                1 (name)
-                       4 LOAD_FAST                0 (ip)
+         266           2 LOAD_FAST                2 (name)
+                       4 LOAD_FAST                1 (ip)
                        6 STORE_ATTR               0 (name)
          
-         188          16 LOAD_FAST                2 (parameter)
+         269          16 LOAD_FAST                3 (parameter)
                       18 LOAD_ATTR                1 (annotation)
                       28 LOAD_GLOBAL              4 (inspect)
                       40 LOAD_ATTR                3 (Signature)
                       50 LOAD_ATTR                4 (empty)
                       60 IS_OP                    1
                       62 POP_JUMP_FORWARD_IF_FALSE     7 (to 78)
          
-         187          64 LOAD_FAST                2 (parameter)
+         268          64 LOAD_FAST                3 (parameter)
                       66 LOAD_ATTR                1 (annotation)
                       76 JUMP_FORWARD           139 (to 356)
          
-         190     >>   78 LOAD_FAST                2 (parameter)
+         271     >>   78 LOAD_FAST                3 (parameter)
                       80 LOAD_ATTR                5 (default)
                       90 LOAD_GLOBAL              4 (inspect)
                      102 LOAD_ATTR                6 (Parameter)
                      112 LOAD_ATTR                4 (empty)
                      122 IS_OP                    1
                      124 POP_JUMP_FORWARD_IF_FALSE    46 (to 218)
          
-         191         126 LOAD_GLOBAL             15 (NULL + isinstance)
-                     138 LOAD_FAST                2 (parameter)
+         272         126 LOAD_GLOBAL             15 (NULL + isinstance)
+                     138 LOAD_FAST                3 (parameter)
                      140 LOAD_ATTR                5 (default)
                      150 LOAD_GLOBAL             16 (InjectedParam)
                      162 PRECALL                  2
                      166 CALL                     2
          
-         190         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
+         271         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
          
-         189         178 LOAD_GLOBAL             19 (NULL + type)
-                     190 LOAD_FAST                2 (parameter)
+         270         178 LOAD_GLOBAL             19 (NULL + type)
+                     190 LOAD_FAST                3 (parameter)
                      192 LOAD_ATTR                5 (default)
                      202 PRECALL                  1
                      206 CALL                     1
                      216 JUMP_FORWARD            69 (to 356)
          
-         193     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
-                     230 LOAD_FAST                2 (parameter)
+         274     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
+                     230 LOAD_FAST                3 (parameter)
                      232 LOAD_ATTR                5 (default)
                      242 LOAD_GLOBAL             20 (InjectedParamQuery)
                      254 PRECALL                  2
                      258 CALL                     2
          
-         192         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
+         273         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
          
-         194         270 LOAD_FAST                2 (parameter)
+         275         270 LOAD_FAST                3 (parameter)
                      272 LOAD_ATTR                5 (default)
                      282 LOAD_ATTR                5 (default)
                      292 POP_JUMP_FORWARD_IF_NONE    25 (to 344)
          
-         192         294 LOAD_GLOBAL             19 (NULL + type)
-                     306 LOAD_FAST                2 (parameter)
+         273         294 LOAD_GLOBAL             19 (NULL + type)
+                     306 LOAD_FAST                3 (parameter)
                      308 LOAD_ATTR                5 (default)
                      318 LOAD_ATTR                5 (default)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 JUMP_FORWARD             6 (to 356)
          
-         195     >>  344 LOAD_GLOBAL             22 (str)
+         276     >>  344 LOAD_GLOBAL             22 (str)
          
-         186     >>  356 LOAD_FAST                0 (ip)
+         267     >>  356 LOAD_FAST                1 (ip)
                      358 STORE_ATTR              12 (target_type)
          
-         197         368 LOAD_FAST                0 (ip)
-                     370 LOAD_METHOD             13 (check)
-                     392 PRECALL                  0
-                     396 CALL                     0
-                     406 POP_TOP
+         278         368 LOAD_FAST                0 (view_fn)
+                     370 LOAD_FAST                1 (ip)
+                     372 STORE_ATTR              13 (view_fn)
+         
+         279         382 LOAD_FAST                1 (ip)
+                     384 LOAD_METHOD             14 (check)
+                     406 PRECALL                  0
+                     410 CALL                     0
+                     420 POP_TOP
          
-         198         408 LOAD_FAST                0 (ip)
-                     410 RETURN_VALUE
+         280         422 LOAD_FAST                1 (ip)
+                     424 RETURN_VALUE
          consts
             None
-         names      ('name', 'annotation', 'inspect', 'Signature', 'empty', 'default', 'Parameter', 'isinstance', 'InjectedParam', 'type', 'InjectedParamQuery', 'str', 'target_type', 'check')
-         varnames   ('ip', 'name', 'parameter')
+         names      ('name', 'annotation', 'inspect', 'Signature', 'empty', 'default', 'Parameter', 'isinstance', 'InjectedParam', 'type', 'InjectedParamQuery', 'str', 'target_type', 'view_fn', 'check')
+         varnames   ('view_fn', 'ip', 'name', 'parameter')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_setup_injected_param'
-         firstlineno 184
+         firstlineno 260
          lnotab
-            0x02010e0330ff0e03300132ff02ff280432ff020218fe32030cf70c0b28
-            01
+            0x02060e0330ff0e03300132ff02ff280432ff020218fe32030cf70c0b0e
+            012801
       'parameters'
       'get'
       'post'
       code
-         argcount  : 3
-         nlocals   : 8
-         stacksize : 6
+         argcount  : 4
+         nlocals   : 9
+         stacksize : 7
          flags     : 3
          code
-            0x970069007d037c00640164028502190000000000000000007d0064037d
-            047c00440090015d777d057401000000000000000000007c056a01000000
+            0x970069007d047c01640164028502190000000000000000007d0164037d
+            057c01440090015d7c7d067401000000000000000000007c066a01000000
             0000000000740400000000000000000000a6020000ab0200000000000000
-            0072267c056a0100000000000000007d067407000000000000000000007c
-            067c056a0400000000000000007c05a6030000ab0300000000000000007c
-            037c066a0400000000000000003c0000008c437c056a0100000000000000
-            00740a000000000000000000006a0600000000000000006a070000000000
-            0000006b030000000072077c056a0100000000000000006e0164027d077c
-            0272777401000000000000000000007c056a080000000000000000741200
-            000000000000000000a6020000ab020000000000000000725d7415000000
-            000000000000007c056a0800000000000000007416000000000000000000
-            006a0c0000000000000000a6020000ab020000000000000000723e7c0472
-            0f741b000000000000000000006404a6010000ab01000000000000000082
-            0164057d04740700000000000000000000741d00000000000000000000a6
-            000000ab0000000000000000007c056a0400000000000000007c05a60300
-            00ab0300000000000000007c037c056a0400000000000000003c0000008c
-            df7c0164057500722e740700000000000000000000741f00000000000000
-            0000007c07ac06a6010000ab0100000000000000007c056a040000000000
-            0000007c05a6030000ab0300000000000000007c037c056a040000000000
-            0000003c00000090018c117c0164076b0200000000722e74070000000000
-            00000000007421000000000000000000007c07ac06a6010000ab01000000
-            00000000007c056a0400000000000000007c05a6030000ab030000000000
-            0000007c037c056a0400000000000000003c00000090018c457c0164086b
-            0200000000722c7407000000000000000000007423000000000000000000
-            007c07ac06a6010000ab0100000000000000007c056a0400000000000000
-            007c05a6030000ab0300000000000000007c037c056a0400000000000000
-            003c00000090018c797c035300
-         201           0 RESUME                   0
+            0072277c066a0100000000000000007d077407000000000000000000007c
+            007c077c066a0400000000000000007c06a6040000ab0400000000000000
+            007c047c076a0400000000000000003c0000008c447c066a010000000000
+            000000740a000000000000000000006a0600000000000000006a07000000
+            00000000006b030000000072077c066a0100000000000000006e0164027d
+            087c0372787401000000000000000000007c066a08000000000000000074
+            1200000000000000000000a6020000ab020000000000000000725e741500
+            0000000000000000007c066a080000000000000000741600000000000000
+            0000006a0c0000000000000000a6020000ab020000000000000000723f7c
+            05720f741b000000000000000000006404a6010000ab0100000000000000
+            00820164057d057407000000000000000000007c00741d00000000000000
+            000000a6000000ab0000000000000000007c066a0400000000000000007c
+            06a6040000ab0400000000000000007c047c066a0400000000000000003c
+            0000008ce17c0264057500722f7407000000000000000000007c00741f00
+            0000000000000000007c08ac06a6010000ab0100000000000000007c066a
+            0400000000000000007c06a6040000ab0400000000000000007c047c066a
+            0400000000000000003c00000090018c147c0264076b0200000000722f74
+            07000000000000000000007c007421000000000000000000007c08ac06a6
+            010000ab0100000000000000007c066a0400000000000000007c06a60400
+            00ab0400000000000000007c047c066a0400000000000000003c00000090
+            018c497c0264086b0200000000722d7407000000000000000000007c0074
+            23000000000000000000007c08ac06a6010000ab0100000000000000007c
+            066a0400000000000000007c06a6040000ab0400000000000000007c047c
+            066a0400000000000000003c00000090018c7e7c045300
+         283           0 RESUME                   0
          
-         209           2 BUILD_MAP                0
-                       4 STORE_FAST               3 (result)
+         292           2 BUILD_MAP                0
+                       4 STORE_FAST               4 (result)
          
-         212           6 LOAD_FAST                0 (parameters)
+         295           6 LOAD_FAST                1 (parameters)
                        8 LOAD_CONST               1 (1)
                       10 LOAD_CONST               2 (None)
                       12 BUILD_SLICE              2
                       14 BINARY_SUBSCR
-                      24 STORE_FAST               0 (parameters)
+                      24 STORE_FAST               1 (parameters)
          
-         214          26 LOAD_CONST               3 (False)
-                      28 STORE_FAST               4 (found_form_arg)
+         297          26 LOAD_CONST               3 (False)
+                      28 STORE_FAST               5 (found_form_arg)
          
-         215          30 LOAD_FAST                0 (parameters)
+         298          30 LOAD_FAST                1 (parameters)
                       32 GET_ITER
                  >>   34 EXTENDED_ARG             1
-                      36 FOR_ITER               375 (to 788)
-                      38 STORE_FAST               5 (arg)
+                      36 FOR_ITER               380 (to 798)
+                      38 STORE_FAST               6 (arg)
          
-         216          40 LOAD_GLOBAL              1 (NULL + isinstance)
-                      52 LOAD_FAST                5 (arg)
+         299          40 LOAD_GLOBAL              1 (NULL + isinstance)
+                      52 LOAD_FAST                6 (arg)
                       54 LOAD_ATTR                1 (default)
                       64 LOAD_GLOBAL              4 (InjectedParam)
                       76 PRECALL                  2
                       80 CALL                     2
-                      90 POP_JUMP_FORWARD_IF_FALSE    38 (to 168)
+                      90 POP_JUMP_FORWARD_IF_FALSE    39 (to 170)
          
-         217          92 LOAD_FAST                5 (arg)
+         300          92 LOAD_FAST                6 (arg)
                       94 LOAD_ATTR                1 (default)
-                     104 STORE_FAST               6 (ip)
+                     104 STORE_FAST               7 (ip)
          
-         218         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
-                     118 LOAD_FAST                6 (ip)
-                     120 LOAD_FAST                5 (arg)
-                     122 LOAD_ATTR                4 (name)
-                     132 LOAD_FAST                5 (arg)
-                     134 PRECALL                  3
-                     138 CALL                     3
-                     148 LOAD_FAST                3 (result)
-                     150 LOAD_FAST                6 (ip)
-                     152 LOAD_ATTR                4 (name)
-                     162 STORE_SUBSCR
-                     166 JUMP_BACKWARD           67 (to 34)
-         
-         223     >>  168 LOAD_FAST                5 (arg)
-                     170 LOAD_ATTR                1 (default)
-                     180 LOAD_GLOBAL             10 (inspect)
-                     192 LOAD_ATTR                6 (Parameter)
-                     202 LOAD_ATTR                7 (empty)
-                     212 COMPARE_OP               3 (!=)
-                     218 POP_JUMP_FORWARD_IF_FALSE     7 (to 234)
-                     220 LOAD_FAST                5 (arg)
-                     222 LOAD_ATTR                1 (default)
-                     232 JUMP_FORWARD             1 (to 236)
-                 >>  234 LOAD_CONST               2 (None)
-         
-         222     >>  236 STORE_FAST               7 (default_value)
-         
-         227         238 LOAD_FAST                2 (auto_form)
-         
-         226         240 POP_JUMP_FORWARD_IF_FALSE   119 (to 480)
-         
-         228         242 LOAD_GLOBAL              1 (NULL + isinstance)
-                     254 LOAD_FAST                5 (arg)
-                     256 LOAD_ATTR                8 (annotation)
-                     266 LOAD_GLOBAL             18 (type)
-                     278 PRECALL                  2
-                     282 CALL                     2
-         
-         226         292 POP_JUMP_FORWARD_IF_FALSE    93 (to 480)
-         
-         229         294 LOAD_GLOBAL             21 (NULL + issubclass)
-                     306 LOAD_FAST                5 (arg)
-                     308 LOAD_ATTR                8 (annotation)
-                     318 LOAD_GLOBAL             22 (forms)
-                     330 LOAD_ATTR               12 (BaseForm)
-                     340 PRECALL                  2
-                     344 CALL                     2
-         
-         226         354 POP_JUMP_FORWARD_IF_FALSE    62 (to 480)
-         
-         231         356 LOAD_FAST                4 (found_form_arg)
-                     358 POP_JUMP_FORWARD_IF_FALSE    15 (to 390)
+         301         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+                     118 LOAD_FAST                0 (view_fn)
+                     120 LOAD_FAST                7 (ip)
+                     122 LOAD_FAST                6 (arg)
+                     124 LOAD_ATTR                4 (name)
+                     134 LOAD_FAST                6 (arg)
+                     136 PRECALL                  4
+                     140 CALL                     4
+                     150 LOAD_FAST                4 (result)
+                     152 LOAD_FAST                7 (ip)
+                     154 LOAD_ATTR                4 (name)
+                     164 STORE_SUBSCR
+                     168 JUMP_BACKWARD           68 (to 34)
+         
+         306     >>  170 LOAD_FAST                6 (arg)
+                     172 LOAD_ATTR                1 (default)
+                     182 LOAD_GLOBAL             10 (inspect)
+                     194 LOAD_ATTR                6 (Parameter)
+                     204 LOAD_ATTR                7 (empty)
+                     214 COMPARE_OP               3 (!=)
+                     220 POP_JUMP_FORWARD_IF_FALSE     7 (to 236)
+                     222 LOAD_FAST                6 (arg)
+                     224 LOAD_ATTR                1 (default)
+                     234 JUMP_FORWARD             1 (to 238)
+                 >>  236 LOAD_CONST               2 (None)
+         
+         305     >>  238 STORE_FAST               8 (default_value)
+         
+         310         240 LOAD_FAST                3 (auto_form)
+         
+         309         242 POP_JUMP_FORWARD_IF_FALSE   120 (to 484)
+         
+         311         244 LOAD_GLOBAL              1 (NULL + isinstance)
+                     256 LOAD_FAST                6 (arg)
+                     258 LOAD_ATTR                8 (annotation)
+                     268 LOAD_GLOBAL             18 (type)
+                     280 PRECALL                  2
+                     284 CALL                     2
+         
+         309         294 POP_JUMP_FORWARD_IF_FALSE    94 (to 484)
+         
+         312         296 LOAD_GLOBAL             21 (NULL + issubclass)
+                     308 LOAD_FAST                6 (arg)
+                     310 LOAD_ATTR                8 (annotation)
+                     320 LOAD_GLOBAL             22 (forms)
+                     332 LOAD_ATTR               12 (BaseForm)
+                     342 PRECALL                  2
+                     346 CALL                     2
+         
+         309         356 POP_JUMP_FORWARD_IF_FALSE    63 (to 484)
+         
+         314         358 LOAD_FAST                5 (found_form_arg)
+                     360 POP_JUMP_FORWARD_IF_FALSE    15 (to 392)
+         
+         315         362 LOAD_GLOBAL             27 (NULL + Exception)
+         
+         316         374 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
+         
+         315         376 PRECALL                  1
+                     380 CALL                     1
+                     390 RAISE_VARARGS            1
+         
+         318     >>  392 LOAD_CONST               5 (True)
+                     394 STORE_FAST               5 (found_form_arg)
+         
+         319         396 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         
+         320         408 LOAD_FAST                0 (view_fn)
+                     410 LOAD_GLOBAL             29 (NULL + handle_form)
+                     422 PRECALL                  0
+                     426 CALL                     0
+                     436 LOAD_FAST                6 (arg)
+                     438 LOAD_ATTR                4 (name)
+                     448 LOAD_FAST                6 (arg)
+         
+         319         450 PRECALL                  4
+                     454 CALL                     4
+                     464 LOAD_FAST                4 (result)
+                     466 LOAD_FAST                6 (arg)
+                     468 LOAD_ATTR                4 (name)
+                     478 STORE_SUBSCR
+                     482 JUMP_BACKWARD          225 (to 34)
+         
+         323     >>  484 LOAD_FAST                2 (auto_param)
+                     486 LOAD_CONST               5 (True)
+                     488 IS_OP                    0
+                     490 POP_JUMP_FORWARD_IF_FALSE    47 (to 586)
+         
+         324         492 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         
+         325         504 LOAD_FAST                0 (view_fn)
+                     506 LOAD_GLOBAL             31 (NULL + InjectedParamQuery)
+                     518 LOAD_FAST                8 (default_value)
+                     520 KW_NAMES                 6
+                     522 PRECALL                  1
+                     526 CALL                     1
+                     536 LOAD_FAST                6 (arg)
+                     538 LOAD_ATTR                4 (name)
+                     548 LOAD_FAST                6 (arg)
+         
+         324         550 PRECALL                  4
+                     554 CALL                     4
+                     564 LOAD_FAST                4 (result)
+                     566 LOAD_FAST                6 (arg)
+                     568 LOAD_ATTR                4 (name)
+                     578 STORE_SUBSCR
+                     582 EXTENDED_ARG             1
+                     584 JUMP_BACKWARD          276 (to 34)
+         
+         327     >>  586 LOAD_FAST                2 (auto_param)
+                     588 LOAD_CONST               7 ('get')
+                     590 COMPARE_OP               2 (==)
+                     596 POP_JUMP_FORWARD_IF_FALSE    47 (to 692)
+         
+         328         598 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         
+         329         610 LOAD_FAST                0 (view_fn)
+                     612 LOAD_GLOBAL             33 (NULL + InjectedParamQueryGet)
+                     624 LOAD_FAST                8 (default_value)
+                     626 KW_NAMES                 6
+                     628 PRECALL                  1
+                     632 CALL                     1
+                     642 LOAD_FAST                6 (arg)
+                     644 LOAD_ATTR                4 (name)
+                     654 LOAD_FAST                6 (arg)
+         
+         328         656 PRECALL                  4
+                     660 CALL                     4
+                     670 LOAD_FAST                4 (result)
+                     672 LOAD_FAST                6 (arg)
+                     674 LOAD_ATTR                4 (name)
+                     684 STORE_SUBSCR
+                     688 EXTENDED_ARG             1
+                     690 JUMP_BACKWARD          329 (to 34)
+         
+         331     >>  692 LOAD_FAST                2 (auto_param)
+                     694 LOAD_CONST               8 ('post')
+                     696 COMPARE_OP               2 (==)
+                     702 POP_JUMP_FORWARD_IF_FALSE    45 (to 794)
+         
+         332         704 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         
+         333         716 LOAD_FAST                0 (view_fn)
+         
+         334         718 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
+                     730 LOAD_FAST                8 (default_value)
+                     732 KW_NAMES                 6
+                     734 PRECALL                  1
+                     738 CALL                     1
+         
+         335         748 LOAD_FAST                6 (arg)
+                     750 LOAD_ATTR                4 (name)
+         
+         336         760 LOAD_FAST                6 (arg)
+         
+         332         762 PRECALL                  4
+                     766 CALL                     4
+                     776 LOAD_FAST                4 (result)
+                     778 LOAD_FAST                6 (arg)
+                     780 LOAD_ATTR                4 (name)
+                     790 STORE_SUBSCR
+                 >>  794 EXTENDED_ARG             1
+                     796 JUMP_BACKWARD          382 (to 34)
          
-         232         360 LOAD_GLOBAL             27 (NULL + Exception)
-         
-         233         372 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
-         
-         232         374 PRECALL                  1
-                     378 CALL                     1
-                     388 RAISE_VARARGS            1
-         
-         235     >>  390 LOAD_CONST               5 (True)
-                     392 STORE_FAST               4 (found_form_arg)
-         
-         236         394 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
-                     406 LOAD_GLOBAL             29 (NULL + handle_form)
-                     418 PRECALL                  0
-                     422 CALL                     0
-                     432 LOAD_FAST                5 (arg)
-                     434 LOAD_ATTR                4 (name)
-                     444 LOAD_FAST                5 (arg)
-                     446 PRECALL                  3
-                     450 CALL                     3
-                     460 LOAD_FAST                3 (result)
-                     462 LOAD_FAST                5 (arg)
-                     464 LOAD_ATTR                4 (name)
-                     474 STORE_SUBSCR
-                     478 JUMP_BACKWARD          223 (to 34)
-         
-         238     >>  480 LOAD_FAST                1 (auto_param)
-                     482 LOAD_CONST               5 (True)
-                     484 IS_OP                    0
-                     486 POP_JUMP_FORWARD_IF_FALSE    46 (to 580)
-         
-         239         488 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
-         
-         240         500 LOAD_GLOBAL             31 (NULL + InjectedParamQuery)
-                     512 LOAD_FAST                7 (default_value)
-                     514 KW_NAMES                 6
-                     516 PRECALL                  1
-                     520 CALL                     1
-                     530 LOAD_FAST                5 (arg)
-                     532 LOAD_ATTR                4 (name)
-                     542 LOAD_FAST                5 (arg)
-         
-         239         544 PRECALL                  3
-                     548 CALL                     3
-                     558 LOAD_FAST                3 (result)
-                     560 LOAD_FAST                5 (arg)
-                     562 LOAD_ATTR                4 (name)
-                     572 STORE_SUBSCR
-                     576 EXTENDED_ARG             1
-                     578 JUMP_BACKWARD          273 (to 34)
-         
-         242     >>  580 LOAD_FAST                1 (auto_param)
-                     582 LOAD_CONST               7 ('get')
-                     584 COMPARE_OP               2 (==)
-                     590 POP_JUMP_FORWARD_IF_FALSE    46 (to 684)
-         
-         243         592 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
-         
-         244         604 LOAD_GLOBAL             33 (NULL + InjectedParamQueryGet)
-                     616 LOAD_FAST                7 (default_value)
-                     618 KW_NAMES                 6
-                     620 PRECALL                  1
-                     624 CALL                     1
-                     634 LOAD_FAST                5 (arg)
-                     636 LOAD_ATTR                4 (name)
-                     646 LOAD_FAST                5 (arg)
-         
-         243         648 PRECALL                  3
-                     652 CALL                     3
-                     662 LOAD_FAST                3 (result)
-                     664 LOAD_FAST                5 (arg)
-                     666 LOAD_ATTR                4 (name)
-                     676 STORE_SUBSCR
-                     680 EXTENDED_ARG             1
-                     682 JUMP_BACKWARD          325 (to 34)
-         
-         246     >>  684 LOAD_FAST                1 (auto_param)
-                     686 LOAD_CONST               8 ('post')
-                     688 COMPARE_OP               2 (==)
-                     694 POP_JUMP_FORWARD_IF_FALSE    44 (to 784)
-         
-         247         696 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
-         
-         248         708 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
-                     720 LOAD_FAST                7 (default_value)
-                     722 KW_NAMES                 6
-                     724 PRECALL                  1
-                     728 CALL                     1
-                     738 LOAD_FAST                5 (arg)
-                     740 LOAD_ATTR                4 (name)
-                     750 LOAD_FAST                5 (arg)
-         
-         247         752 PRECALL                  3
-                     756 CALL                     3
-                     766 LOAD_FAST                3 (result)
-                     768 LOAD_FAST                5 (arg)
-                     770 LOAD_ATTR                4 (name)
-                     780 STORE_SUBSCR
-                 >>  784 EXTENDED_ARG             1
-                     786 JUMP_BACKWARD          377 (to 34)
-         
-         251     >>  788 LOAD_FAST                3 (result)
-                     790 RETURN_VALUE
+         339     >>  798 LOAD_FAST                4 (result)
+                     800 RETURN_VALUE
          consts
             '\n    Extracts all injected parameters from the given list of function arguments.\n    '
             1
             None
             False
             'You can only have one Form argument in a view function.'
             True
             ('default',)
             'get'
             'post'
          names      ('isinstance', 'default', 'InjectedParam', '_setup_injected_param', 'name', 'inspect', 'Parameter', 'empty', 'annotation', 'type', 'issubclass', 'forms', 'BaseForm', 'Exception', 'handle_form', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost')
-         varnames   ('parameters', 'auto_param', 'auto_form', 'result', 'found_form_arg', 'arg', 'ip', 'default_value')
+         varnames   ('view_fn', 'parameters', 'auto_param', 'auto_form', 'result', 'found_form_arg', 'arg', 'ip', 'default_value')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_extract_injected_params'
-         firstlineno 201
+         firstlineno 283
          lnotab
-            0x02080403140204010a0134010e013e0544ff020502ff020232fe02033c
-            fd020504010c0102ff10030401560208010c012cff24030c010c012cff24
-            030c010c012cff2404
-      'args'
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 2
-         flags     : 3
-         code 0x97007c006401190000000000000000005300
-         254           0 RESUME                   0
-         
-         255           2 LOAD_FAST                0 (args)
-                       4 LOAD_CONST               1 (0)
-                       6 BINARY_SUBSCR
-                      16 RETURN_VALUE
-         consts
-            None
-            0
-         names      ()
-         varnames   ('args',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       '_get_request_from_args'
-         firstlineno 254
-         lnotab 0x0201
+            0x02090403140204010a0134010e01400544ff020502ff020232fe02033c
+            fd020504010c0102ff100304010c012aff220408010c012eff24030c010c
+            012eff24030c010c0102011e010c0102fc2407
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a025500020065036a0400000000000000006401ac
             02a6010000ab0100000000000000005a0565066507190000000000000000
             00650864033c000000020065036a0400000000000000006401ac02a60100
             00ab0100000000000000005a09650a650864043c000000020065036a0400
             000000000000006405ac02a6010000ab0100000000000000005a0b650c65
             0864063c000000640784005a0d6408650e6602640984045a0f6408650e66
             02640a84045a10640b650a640c65116507650a6602190000000000000000
             006604640d84045a1264015300
-         263           0 RESUME                   0
+         347           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQuery')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         265          12 PUSH_NULL
+         349          12 PUSH_NULL
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
          
-         266          68 PUSH_NULL
+         350          68 PUSH_NULL
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
          
-         267         112 PUSH_NULL
+         351         112 PUSH_NULL
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
          
-         269         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 269>)
+         353         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 353>)
                      158 MAKE_FUNCTION            0
                      160 STORE_NAME              13 (check)
          
-         273         162 LOAD_CONST               8 ('request')
+         357         162 LOAD_CONST               8 ('request')
                      164 LOAD_NAME               14 (HttpRequest)
                      166 BUILD_TUPLE              2
-                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 273>)
+                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 357>)
                      170 MAKE_FUNCTION            4 (annotations)
                      172 STORE_NAME              15 (_create_lookup_dict)
          
-         280         174 LOAD_CONST               8 ('request')
+         364         174 LOAD_CONST               8 ('request')
                      176 LOAD_NAME               14 (HttpRequest)
                      178 BUILD_TUPLE              2
-                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 280>)
+                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 364>)
                      182 MAKE_FUNCTION            4 (annotations)
                      184 STORE_NAME              16 (_consume_param)
          
-         290         186 LOAD_CONST              11 ('args')
+         374         186 LOAD_CONST              11 ('args')
                      188 LOAD_NAME               10 (Any)
                      190 LOAD_CONST              12 ('kwargs')
                      192 LOAD_NAME               17 (dict)
                      194 LOAD_NAME                7 (str)
                      196 LOAD_NAME               10 (Any)
                      198 BUILD_TUPLE              2
                      200 BINARY_SUBSCR
                      210 BUILD_TUPLE              4
-                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 290>)
+                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 374>)
                      214 MAKE_FUNCTION            4 (annotations)
                      216 STORE_NAME              18 (get_value)
                      218 LOAD_CONST               1 (None)
                      220 RETURN_VALUE
          consts
             'InjectedParamQuery'
             None
@@ -2214,38 +2863,38 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000800e7c006a0100000000000000007c
                   005f0000000000000000006400530064005300
-               269           0 RESUME                   0
+               353           0 RESUME                   0
                
-               270           2 LOAD_FAST                0 (self)
+               354           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 44)
                
-               271          16 LOAD_FAST                0 (self)
+               355          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (name)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               0 (query_param_name)
                             40 LOAD_CONST               0 (None)
                             42 RETURN_VALUE
                
-               270     >>   44 LOAD_CONST               0 (None)
+               354     >>   44 LOAD_CONST               0 (None)
                             46 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 269
+               firstlineno 353
                lnotab 0x02010e011cff
             'request'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -2256,55 +2905,55 @@
                   00000000007d027401000000000000000000006a01000000000000000074
                   04000000000000000000007c016a040000000000000000a6020000ab0200
                   000000000000008a05880566016402840889054400a6000000ab00000000
                   00000000007d037c037c027a0700005300
                              0 MAKE_CELL                4 (getqd)
                              2 MAKE_CELL                5 (postqd)
                
-               273           4 RESUME                   0
+               357           4 RESUME                   0
                
-               274           6 LOAD_GLOBAL              1 (NULL + typing)
+               358           6 LOAD_GLOBAL              1 (NULL + typing)
                             18 LOAD_ATTR                1 (cast)
                             28 LOAD_GLOBAL              4 (QueryDict)
                             40 LOAD_FAST                1 (request)
                             42 LOAD_ATTR                3 (GET)
                             52 PRECALL                  2
                             56 CALL                     2
                             66 STORE_DEREF              4 (getqd)
                
-               275          68 LOAD_CLOSURE             4 (getqd)
+               359          68 LOAD_CLOSURE             4 (getqd)
                             70 BUILD_TUPLE              1
-                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 275>)
+                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 359>)
                             74 MAKE_FUNCTION            8 (closure)
                             76 LOAD_DEREF               4 (getqd)
                             78 GET_ITER
                             80 PRECALL                  0
                             84 CALL                     0
                             94 STORE_FAST               2 (getd)
                
-               276          96 LOAD_GLOBAL              1 (NULL + typing)
+               360          96 LOAD_GLOBAL              1 (NULL + typing)
                            108 LOAD_ATTR                1 (cast)
                            118 LOAD_GLOBAL              4 (QueryDict)
                            130 LOAD_FAST                1 (request)
                            132 LOAD_ATTR                4 (POST)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_DEREF              5 (postqd)
                
-               277         158 LOAD_CLOSURE             5 (postqd)
+               361         158 LOAD_CLOSURE             5 (postqd)
                            160 BUILD_TUPLE              1
-                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 277>)
+                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 361>)
                            164 MAKE_FUNCTION            8 (closure)
                            166 LOAD_DEREF               5 (postqd)
                            168 GET_ITER
                            170 PRECALL                  0
                            174 CALL                     0
                            184 STORE_FAST               3 (postd)
                
-               278         186 LOAD_FAST                3 (postd)
+               362         186 LOAD_FAST                3 (postd)
                            188 LOAD_FAST                2 (getd)
                            190 BINARY_OP                7 (|)
                            194 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
@@ -2313,15 +2962,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     275           2 RESUME                   0
+                     359           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (getqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2334,28 +2983,28 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('getqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 275
+                     firstlineno 359
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
                      
-                     277           2 RESUME                   0
+                     361           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (postqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2368,23 +3017,23 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('postqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 277
+                     firstlineno 361
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET', 'POST')
                varnames   ('self', 'request', 'getd', 'postd')
                freevars   ()
                cellvars   ('getqd', 'postqd')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 273
+               firstlineno 357
                lnotab 0x06013e011c013e011c01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -2394,79 +3043,79 @@
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f010000000000000000640053007c006a0000
                   000000000000007c016a0600000000000000007600723974050000000000
                   00000000007407000000000000000000006a040000000000000000740a00
                   0000000000000000007c016a060000000000000000a6020000ab02000000
                   00000000007c006a000000000000000000a6020000ab0200000000000000
                   007c015f0600000000000000006400530064005300
-               280           0 RESUME                   0
+               364           0 RESUME                   0
                
-               281           2 LOAD_FAST                0 (self)
+               365           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               282          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               366          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               283          42 LOAD_GLOBAL              7 (NULL + typing)
+               367          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               282         114 PRECALL                  2
+               366         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               285     >>  144 LOAD_FAST                0 (self)
+               369     >>  144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                0 (query_param_name)
                            156 LOAD_FAST                1 (request)
                            158 LOAD_ATTR                6 (POST)
                            168 CONTAINS_OP              0
                            170 POP_JUMP_FORWARD_IF_FALSE    57 (to 286)
                
-               286         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               370         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               287         184 LOAD_GLOBAL              7 (NULL + typing)
+               371         184 LOAD_GLOBAL              7 (NULL + typing)
                            196 LOAD_ATTR                4 (cast)
                            206 LOAD_GLOBAL             10 (Any)
                            218 LOAD_FAST                1 (request)
                            220 LOAD_ATTR                6 (POST)
                            230 PRECALL                  2
                            234 CALL                     2
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR                0 (query_param_name)
                
-               286         256 PRECALL                  2
+               370         256 PRECALL                  2
                            260 CALL                     2
                            270 LOAD_FAST                1 (request)
                            272 STORE_ATTR               6 (POST)
                            282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                
-               285     >>  286 LOAD_CONST               0 (None)
+               369     >>  286 LOAD_CONST               0 (None)
                            288 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 280
+               firstlineno 364
                lnotab 0x02011c010c0148ff1e031c010c0148ff1eff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -2481,87 +3130,87 @@
                   0000000000000000007c006a070000000000000000a6020000ab02000000
                   000000000072026400530074110000000000000000000064017c006a0300
                   000000000000009b0064029d03a6010000ab01000000000000000082017c
                   006a09000000000000000072157c00a00a00000000000000000000000000
                   000000000000007c03a6010000ab01000000000000000001007417000000
                   000000000000007c057c006a070000000000000000a6020000ab02000000
                   00000000005300
-               290           0 RESUME                   0
+               374           0 RESUME                   0
                
-               291           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               375           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               292          32 LOAD_FAST                0 (self)
+               376          32 LOAD_FAST                0 (self)
                             34 LOAD_METHOD              1 (_create_lookup_dict)
                             56 LOAD_FAST                3 (request)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               4 (lookup_dict)
                
-               293          74 LOAD_FAST                4 (lookup_dict)
+               377          74 LOAD_FAST                4 (lookup_dict)
                             76 LOAD_METHOD              2 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (query_param_name)
                            110 LOAD_CONST               0 (None)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               5 (values)
                
-               295         128 LOAD_FAST                5 (values)
+               379         128 LOAD_FAST                5 (values)
                            130 POP_JUMP_FORWARD_IF_NOT_NONE    68 (to 268)
                
-               296         132 LOAD_FAST                0 (self)
+               380         132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                4 (default)
                            144 POP_JUMP_FORWARD_IF_NONE     9 (to 164)
                
-               297         146 LOAD_FAST                0 (self)
+               381         146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                4 (default)
                            158 BUILD_LIST               1
                            160 STORE_FAST               5 (values)
                            162 JUMP_FORWARD            52 (to 268)
                
-               298     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
+               382     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
                            176 LOAD_GLOBAL             12 (NoneType)
                            188 LOAD_FAST                0 (self)
                            190 LOAD_ATTR                7 (target_type)
                            200 PRECALL                  2
                            204 CALL                     2
                            214 POP_JUMP_FORWARD_IF_FALSE     2 (to 220)
                
-               299         216 LOAD_CONST               0 (None)
+               383         216 LOAD_CONST               0 (None)
                            218 RETURN_VALUE
                
-               301     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
+               385     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
                
-               302         232 LOAD_CONST               1 ("No value found for request parameter '")
+               386         232 LOAD_CONST               1 ("No value found for request parameter '")
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (query_param_name)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               2 ("'")
                            250 BUILD_STRING             3
                
-               301         252 PRECALL                  1
+               385         252 PRECALL                  1
                            256 CALL                     1
                            266 RAISE_VARARGS            1
                
-               305     >>  268 LOAD_FAST                0 (self)
+               389     >>  268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                9 (consume)
                            280 POP_JUMP_FORWARD_IF_FALSE    21 (to 324)
                
-               306         282 LOAD_FAST                0 (self)
+               390         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD             10 (_consume_param)
                            306 LOAD_FAST                3 (request)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               308     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
+               392     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
                            336 LOAD_FAST                5 (values)
                            338 LOAD_FAST                0 (self)
                            340 LOAD_ATTR                7 (target_type)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 RETURN_VALUE
                consts
@@ -2570,50 +3219,50 @@
                   "'"
                names      ('_get_request_from_args', '_create_lookup_dict', 'get', 'query_param_name', 'default', 'issubclass', 'NoneType', 'target_type', 'Exception', 'consume', '_consume_param', '_convert_value_to_type')
                varnames   ('self', 'args', 'kwargs', 'request', 'lookup_dict', 'values')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 290
+               firstlineno 374
                lnotab 0x02011e012a01360204010e011201340104020c0114ff10040e012a02
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'query_param_name', 'Optional', 'str', '__annotations__', 'default', 'Any', 'consume', 'bool', 'check', 'HttpRequest', '_create_lookup_dict', '_consume_param', 'dict', 'get_value')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQuery'
-         firstlineno 263
+         firstlineno 347
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
-         311           0 RESUME                   0
+         395           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryGet')
                        8 STORE_NAME               2 (__qualname__)
          
-         313          10 LOAD_CONST               1 ('request')
+         397          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 313>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 397>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         317          22 LOAD_CONST               1 ('request')
+         401          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 317>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 401>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryGet'
             'request'
@@ -2625,28 +3274,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               313           2 RESUME                   0
+               397           2 RESUME                   0
                
-               314           4 LOAD_GLOBAL              1 (NULL + typing)
+               398           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (GET)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               315          66 LOAD_CLOSURE             2 (qd)
+               399          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 315>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 399>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -2658,15 +3307,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     315           2 RESUME                   0
+                     399           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2679,110 +3328,110 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 315
+                     firstlineno 399
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 313
+               firstlineno 397
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
-               317           0 RESUME                   0
+               401           0 RESUME                   0
                
-               318           2 LOAD_FAST                0 (self)
+               402           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               319          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               403          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               320          42 LOAD_GLOBAL              7 (NULL + typing)
+               404          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               319         114 PRECALL                  2
+               403         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               318     >>  144 LOAD_CONST               0 (None)
+               402     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 317
+               firstlineno 401
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryGet'
-         firstlineno 311
+         firstlineno 395
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
-         324           0 RESUME                   0
+         408           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryPost')
                        8 STORE_NAME               2 (__qualname__)
          
-         326          10 LOAD_CONST               1 ('request')
+         410          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 326>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 410>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         330          22 LOAD_CONST               1 ('request')
+         414          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 330>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 414>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryPost'
             'request'
@@ -2794,28 +3443,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               326           2 RESUME                   0
+               410           2 RESUME                   0
                
-               327           4 LOAD_GLOBAL              1 (NULL + typing)
+               411           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (POST)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               328          66 LOAD_CLOSURE             2 (qd)
+               412          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 328>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 412>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -2827,15 +3476,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     328           2 RESUME                   0
+                     412           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2848,96 +3497,96 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 328
+                     firstlineno 412
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 326
+               firstlineno 410
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
-               330           0 RESUME                   0
+               414           0 RESUME                   0
                
-               331           2 LOAD_FAST                0 (self)
+               415           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (POST)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               332          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               416          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               333          42 LOAD_GLOBAL              7 (NULL + typing)
+               417          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (POST)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               332         114 PRECALL                  2
+               416         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (POST)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               331     >>  144 LOAD_CONST               0 (None)
+               415     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'POST', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 330
+               firstlineno 414
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryPost'
-         firstlineno 324
+         firstlineno 408
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
-         337           0 RESUME                   0
+         421           0 RESUME                   0
          
-         338           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
+         422           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -2945,27 +3594,27 @@
             ('default', 'consume')
          names      ('InjectedParamQueryGet',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_get'
-         firstlineno 337
+         firstlineno 421
          lnotab 0x0201
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         341           0 RESUME                   0
+         425           0 RESUME                   0
          
-         342           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
+         426           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -2973,29 +3622,29 @@
             ('default', 'consume')
          names      ('InjectedParamQueryPost',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_post'
-         firstlineno 341
+         firstlineno 425
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
-         345           0 RESUME                   0
+         429           0 RESUME                   0
          
-         346           2 LOAD_GLOBAL              1 (NULL + typing)
+         430           2 LOAD_GLOBAL              1 (NULL + typing)
                       14 LOAD_ATTR                1 (cast)
                       24 LOAD_GLOBAL              4 (T)
                       36 LOAD_GLOBAL              7 (NULL + InjectedParamQuery)
                       48 LOAD_FAST                0 (default)
                       50 LOAD_FAST                1 (consume)
                       52 KW_NAMES                 1
                       54 PRECALL                  2
@@ -3008,15 +3657,15 @@
             ('default', 'consume')
          names      ('typing', 'cast', 'T', 'InjectedParamQuery')
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param'
-         firstlineno 345
+         firstlineno 429
          lnotab 0x0201
       'values'
       'target_type'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 6
@@ -3042,148 +3691,148 @@
             00720264056e0164065300740b0000000000000000000074140000000000
             00000000006a0b00000000000000007c01a6020000ab0200000000000000
             0072147415000000000000000000006a0b00000000000000007c02a60100
             00ab010000000000000000530074190000000000000000000064077c019b
             0064087c029b009d04a6010000ab0100000000000000008201
                        0 MAKE_CELL                3 (list_type)
          
-         349           2 RESUME                   0
+         433           2 RESUME                   0
          
-         351           4 LOAD_GLOBAL              1 (NULL + typing)
+         435           4 LOAD_GLOBAL              1 (NULL + typing)
                       16 LOAD_ATTR                1 (get_origin)
                       26 LOAD_FAST                1 (target_type)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 LOAD_GLOBAL              4 (list)
                       54 COMPARE_OP               2 (==)
                       60 POP_JUMP_FORWARD_IF_FALSE    40 (to 142)
          
-         352          62 LOAD_GLOBAL              1 (NULL + typing)
+         436          62 LOAD_GLOBAL              1 (NULL + typing)
                       74 LOAD_ATTR                3 (get_args)
                       84 LOAD_FAST                1 (target_type)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_CONST               1 (0)
                      102 BINARY_SUBSCR
                      112 STORE_DEREF              3 (list_type)
          
-         353         114 LOAD_CLOSURE             3 (list_type)
+         437         114 LOAD_CLOSURE             3 (list_type)
                      116 BUILD_TUPLE              1
-                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 353>)
+                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 437>)
                      120 MAKE_FUNCTION            8 (closure)
                      122 LOAD_FAST                0 (values)
                      124 GET_ITER
                      126 PRECALL                  0
                      130 CALL                     0
                      140 RETURN_VALUE
          
-         355     >>  142 LOAD_FAST                1 (target_type)
+         439     >>  142 LOAD_FAST                1 (target_type)
                      144 LOAD_GLOBAL              4 (list)
                      156 COMPARE_OP               2 (==)
                      162 POP_JUMP_FORWARD_IF_FALSE    12 (to 188)
          
-         356         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 356>)
+         440         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 440>)
                      166 MAKE_FUNCTION            0
                      168 LOAD_FAST                0 (values)
                      170 GET_ITER
                      172 PRECALL                  0
                      176 CALL                     0
                      186 RETURN_VALUE
          
-         359     >>  188 LOAD_FAST                0 (values)
+         443     >>  188 LOAD_FAST                0 (values)
                      190 LOAD_CONST               1 (0)
                      192 BINARY_SUBSCR
                      202 STORE_FAST               2 (value)
          
-         361         204 LOAD_FAST                2 (value)
+         445         204 LOAD_FAST                2 (value)
                      206 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 210)
          
-         362         208 JUMP_FORWARD           201 (to 612)
+         446         208 JUMP_FORWARD           201 (to 612)
          
-         363     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
+         447     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
                      222 LOAD_FAST                2 (value)
                      224 LOAD_FAST                1 (target_type)
                      226 PRECALL                  2
                      230 CALL                     2
                      240 POP_JUMP_FORWARD_IF_FALSE     2 (to 246)
          
-         364         242 LOAD_FAST                2 (value)
+         448         242 LOAD_FAST                2 (value)
                      244 RETURN_VALUE
          
-         365     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
+         449     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
                      258 LOAD_GLOBAL             12 (str)
                      270 LOAD_FAST                1 (target_type)
                      272 PRECALL                  2
                      276 CALL                     2
                      286 POP_JUMP_FORWARD_IF_FALSE    15 (to 318)
          
-         366         288 LOAD_GLOBAL             13 (NULL + str)
+         450         288 LOAD_GLOBAL             13 (NULL + str)
                      300 LOAD_FAST                2 (value)
                      302 PRECALL                  1
                      306 CALL                     1
                      316 RETURN_VALUE
          
-         367     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
+         451     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
                      330 LOAD_GLOBAL             14 (int)
                      342 LOAD_FAST                1 (target_type)
                      344 PRECALL                  2
                      348 CALL                     2
                      358 POP_JUMP_FORWARD_IF_FALSE    15 (to 390)
          
-         368         360 LOAD_GLOBAL             15 (NULL + int)
+         452         360 LOAD_GLOBAL             15 (NULL + int)
                      372 LOAD_FAST                2 (value)
                      374 PRECALL                  1
                      378 CALL                     1
                      388 RETURN_VALUE
          
-         369     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
+         453     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
                      402 LOAD_GLOBAL             16 (float)
                      414 LOAD_FAST                1 (target_type)
                      416 PRECALL                  2
                      420 CALL                     2
                      430 POP_JUMP_FORWARD_IF_FALSE    15 (to 462)
          
-         370         432 LOAD_GLOBAL             17 (NULL + float)
+         454         432 LOAD_GLOBAL             17 (NULL + float)
                      444 LOAD_FAST                2 (value)
                      446 PRECALL                  1
                      450 CALL                     1
                      460 RETURN_VALUE
          
-         371     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
+         455     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
                      474 LOAD_GLOBAL             18 (bool)
                      486 LOAD_FAST                1 (target_type)
                      488 PRECALL                  2
                      492 CALL                     2
                      502 POP_JUMP_FORWARD_IF_FALSE     8 (to 520)
          
-         372         504 LOAD_FAST                2 (value)
+         456         504 LOAD_FAST                2 (value)
                      506 LOAD_CONST               4 ((False, '', 'false', 'False'))
                      508 CONTAINS_OP              0
                      510 POP_JUMP_FORWARD_IF_FALSE     2 (to 516)
                      512 LOAD_CONST               5 (False)
                      514 JUMP_FORWARD             1 (to 518)
                  >>  516 LOAD_CONST               6 (True)
                  >>  518 RETURN_VALUE
          
-         373     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
+         457     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
                      532 LOAD_GLOBAL             20 (uuid)
                      544 LOAD_ATTR               11 (UUID)
                      554 LOAD_FAST                1 (target_type)
                      556 PRECALL                  2
                      560 CALL                     2
                      570 POP_JUMP_FORWARD_IF_FALSE    20 (to 612)
          
-         374         572 LOAD_GLOBAL             21 (NULL + uuid)
+         458         572 LOAD_GLOBAL             21 (NULL + uuid)
                      584 LOAD_ATTR               11 (UUID)
                      594 LOAD_FAST                2 (value)
                      596 PRECALL                  1
                      600 CALL                     1
                      610 RETURN_VALUE
          
-         376     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
+         460     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
                      624 LOAD_CONST               7 ('Unsupported type: ')
                      626 LOAD_FAST                1 (target_type)
                      628 FORMAT_VALUE             0
                      630 LOAD_CONST               8 (' for value: ')
                      632 LOAD_FAST                2 (value)
                      634 FORMAT_VALUE             0
                      636 BUILD_STRING             4
@@ -3199,15 +3848,15 @@
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d137d017401000000000000000000007c01670189
                   02a6020000ab02000000000000000091028c145300
                              0 COPY_FREE_VARS           1
                
-               353           2 RESUME                   0
+               437           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                19 (to 48)
                             10 STORE_FAST               1 (v)
                             12 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             24 LOAD_FAST                1 (v)
                             26 BUILD_LIST               1
@@ -3220,25 +3869,25 @@
                consts
                names      ('_convert_value_to_type',)
                varnames   ('.0', 'v')
                freevars   ('list_type',)
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 353
+               firstlineno 437
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d187d017401000000000000000000007c016701740200
                   000000000000000000a6020000ab02000000000000000091028c195300
-               356           0 RESUME                   0
+               440           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                24 (to 56)
                              8 STORE_FAST               1 (v)
                             10 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             22 LOAD_FAST                1 (v)
                             24 BUILD_LIST               1
@@ -3251,81 +3900,81 @@
                consts
                names      ('_convert_value_to_type', 'str')
                varnames   ('.0', 'v')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 356
+               firstlineno 440
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
-         firstlineno 349
+         firstlineno 433
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
-         384           0 RESUME                   0
+         468           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamForm')
                        8 STORE_NAME               2 (__qualname__)
          
-         385          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 385>)
+         469          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 469>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (check)
          
-         391          16 LOAD_CONST               2 ('args')
+         475          16 LOAD_CONST               2 ('args')
                       18 LOAD_NAME                4 (Any)
                       20 LOAD_CONST               3 ('kwargs')
                       22 LOAD_NAME                5 (dict)
                       24 LOAD_NAME                6 (str)
                       26 LOAD_NAME                4 (Any)
                       28 BUILD_TUPLE              2
                       30 BINARY_SUBSCR
                       40 BUILD_TUPLE              4
-                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 391>)
+                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 475>)
                       44 MAKE_FUNCTION            4 (annotations)
                       46 STORE_NAME               7 (get_value)
          
-         403          48 LOAD_CONST               5 ('request')
+         487          48 LOAD_CONST               5 ('request')
          
-         404          50 LOAD_NAME                8 (HttpRequest)
+         488          50 LOAD_NAME                8 (HttpRequest)
          
-         403          52 LOAD_CONST               6 ('value')
+         487          52 LOAD_CONST               6 ('value')
          
-         404          54 LOAD_NAME                9 (forms)
+         488          54 LOAD_NAME                9 (forms)
                       56 LOAD_ATTR               10 (Form)
          
-         403          66 LOAD_CONST               7 ('return')
+         487          66 LOAD_CONST               7 ('return')
          
-         405          68 LOAD_NAME               11 (Optional)
+         489          68 LOAD_NAME               11 (Optional)
                       70 LOAD_NAME               12 (HttpResponse)
                       72 BINARY_SUBSCR
          
-         403          82 BUILD_TUPLE              6
-                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 403>)
+         487          82 BUILD_TUPLE              6
+                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 487>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              13 (replace_response)
                       90 LOAD_CONST               9 (None)
                       92 RETURN_VALUE
          consts
             'InjectedParamForm'
             code
@@ -3334,49 +3983,49 @@
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000740400
                   0000000000000000006a030000000000000000a6020000ab020000000000
                   000000731774090000000000000000000064017c006a0100000000000000
                   009b009d02a6010000ab010000000000000000820164005300
-               385           0 RESUME                   0
+               469           0 RESUME                   0
                
-               386           2 LOAD_GLOBAL              1 (NULL + issubclass)
+               470           2 LOAD_GLOBAL              1 (NULL + issubclass)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (target_type)
                             26 LOAD_GLOBAL              4 (forms)
                             38 LOAD_ATTR                3 (BaseForm)
                             48 PRECALL                  2
                             52 CALL                     2
                             62 POP_JUMP_FORWARD_IF_TRUE    23 (to 110)
                
-               387          64 LOAD_GLOBAL              9 (NULL + Exception)
+               471          64 LOAD_GLOBAL              9 (NULL + Exception)
                
-               388          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
+               472          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                1 (target_type)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             2
                
-               387          94 PRECALL                  1
+               471          94 PRECALL                  1
                             98 CALL                     1
                            108 RAISE_VARARGS            1
                
-               386     >>  110 LOAD_CONST               0 (None)
+               470     >>  110 LOAD_CONST               0 (None)
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
-               firstlineno 385
+               firstlineno 469
                lnotab 0x02013e010c0112ff10ff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -3393,99 +4042,99 @@
                   0000000000000000007d057c05a00a000000000000000000000000000000
                   00000000007417000000000000000000006a0c00000000000000007c036a
                   0d0000000000000000a6010000ab010000000000000000a6010000ab0100
                   0000000000000001007c00a0020000000000000000000000000000000000
                   0000007c05ac03a6010000ab0100000000000000007d046e147c00a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007d047c045300
-               391           0 RESUME                   0
+               475           0 RESUME                   0
                
-               392           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               476           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               393          32 LOAD_GLOBAL              3 (NULL + is_post)
+               477          32 LOAD_GLOBAL              3 (NULL + is_post)
                             44 LOAD_FAST                3 (request)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 POP_JUMP_FORWARD_IF_FALSE    34 (to 130)
                
-               394          62 LOAD_FAST                0 (self)
+               478          62 LOAD_FAST                0 (self)
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
                
-               395     >>  130 LOAD_FAST                3 (request)
+               479     >>  130 LOAD_FAST                3 (request)
                            132 LOAD_ATTR                5 (content_type)
                            142 LOAD_CONST               2 ('application/json')
                            144 COMPARE_OP               2 (==)
                            150 POP_JUMP_FORWARD_IF_FALSE   116 (to 384)
                
-               396         152 LOAD_GLOBAL             13 (NULL + typing)
+               480         152 LOAD_GLOBAL             13 (NULL + typing)
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
                
-               397         250 LOAD_FAST                5 (new_post_dict)
+               481         250 LOAD_FAST                5 (new_post_dict)
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
                
-               398         338 LOAD_FAST                0 (self)
+               482         338 LOAD_FAST                0 (self)
                            340 LOAD_METHOD              2 (target_type)
                            362 LOAD_FAST                5 (new_post_dict)
                            364 KW_NAMES                 3
                            366 PRECALL                  1
                            370 CALL                     1
                            380 STORE_FAST               4 (form)
                            382 JUMP_FORWARD            20 (to 424)
                
-               400     >>  384 LOAD_FAST                0 (self)
+               484     >>  384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD              2 (target_type)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 STORE_FAST               4 (form)
                
-               401     >>  424 LOAD_FAST                4 (form)
+               485     >>  424 LOAD_FAST                4 (form)
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
-               firstlineno 391
+               firstlineno 475
                lnotab 0x02011e011e0144011601620158012e022801
             'request'
             'value'
             'return'
             code
                argcount  : 3
                nlocals   : 7
@@ -3504,362 +4153,243 @@
                   0000000000a6010000ab0100000000000000007c066a0b00000000000000
                   0064049c037c047c056a0a00000000000000003c0000008c557419000000
                   000000000000007c037c047413000000000000000000007c02a00d000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00a6010000ab0100000000000000007c02a0040000000000000000000000
                   000000000000000000a6000000ab00000000000000000064059c04a60100
                   00ab010000000000000000530064005300
-               403           0 RESUME                   0
+               487           0 RESUME                   0
                
-               406           2 LOAD_GLOBAL              1 (NULL + is_patch)
+               490           2 LOAD_GLOBAL              1 (NULL + is_patch)
                             14 LOAD_FAST                1 (request)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 POP_JUMP_FORWARD_IF_FALSE   215 (to 462)
                             32 LOAD_FAST                1 (request)
                             34 LOAD_ATTR                1 (content_type)
                             44 LOAD_CONST               1 ('application/json')
                             46 COMPARE_OP               2 (==)
                             52 POP_JUMP_FORWARD_IF_FALSE   204 (to 462)
                
-               407          54 LOAD_FAST                1 (request)
+               491          54 LOAD_FAST                1 (request)
                             56 LOAD_ATTR                2 (headers)
                             66 LOAD_METHOD              3 (get)
                             88 LOAD_CONST               2 ('X-DFV-Validate-Field')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 STORE_FAST               3 (validate_field)
                
-               408         106 LOAD_FAST                2 (value)
+               492         106 LOAD_FAST                2 (value)
                            108 LOAD_METHOD              4 (is_valid)
                            130 PRECALL                  0
                            134 CALL                     0
                            144 POP_TOP
                
-               409         146 BUILD_MAP                0
+               493         146 BUILD_MAP                0
                            148 STORE_FAST               4 (fields)
                
-               410         150 LOAD_FAST                2 (value)
+               494         150 LOAD_FAST                2 (value)
                            152 GET_ITER
                        >>  154 FOR_ITER                84 (to 324)
                            156 STORE_FAST               5 (bound_field)
                
-               411         158 LOAD_FAST                5 (bound_field)
+               495         158 LOAD_FAST                5 (bound_field)
                            160 LOAD_ATTR                5 (field)
                            170 LOAD_ATTR                6 (widget)
                            180 STORE_FAST               6 (widget)
                
-               413         182 LOAD_GLOBAL             15 (NULL + len)
+               497         182 LOAD_GLOBAL             15 (NULL + len)
                            194 LOAD_FAST                5 (bound_field)
                            196 LOAD_ATTR                8 (errors)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 LOAD_CONST               3 (0)
                            222 COMPARE_OP               2 (==)
                
-               414         228 LOAD_GLOBAL             19 (NULL + str)
+               498         228 LOAD_GLOBAL             19 (NULL + str)
                            240 LOAD_FAST                2 (value)
                            242 LOAD_FAST                5 (bound_field)
                            244 LOAD_ATTR               10 (name)
                            254 BINARY_SUBSCR
                            264 LOAD_ATTR                8 (errors)
                            274 PRECALL                  1
                            278 CALL                     1
                
-               415         288 LOAD_FAST                6 (widget)
+               499         288 LOAD_FAST                6 (widget)
                            290 LOAD_ATTR               11 (attrs)
                
-               412         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
+               496         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
                            302 BUILD_CONST_KEY_MAP      3
                            304 LOAD_FAST                4 (fields)
                            306 LOAD_FAST                5 (bound_field)
                            308 LOAD_ATTR               10 (name)
                            318 STORE_SUBSCR
                            322 JUMP_BACKWARD           85 (to 154)
                
-               418     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
+               502     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
                
-               420         336 LOAD_FAST                3 (validate_field)
+               504         336 LOAD_FAST                3 (validate_field)
                
-               421         338 LOAD_FAST                4 (fields)
+               505         338 LOAD_FAST                4 (fields)
                
-               422         340 LOAD_GLOBAL             19 (NULL + str)
+               506         340 LOAD_GLOBAL             19 (NULL + str)
                            352 LOAD_FAST                2 (value)
                            354 LOAD_METHOD             13 (non_field_errors)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 PRECALL                  1
                            394 CALL                     1
                
-               423         404 LOAD_FAST                2 (value)
+               507         404 LOAD_FAST                2 (value)
                            406 LOAD_METHOD              4 (is_valid)
                            428 PRECALL                  0
                            432 CALL                     0
                
-               419         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
+               503         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
                            444 BUILD_CONST_KEY_MAP      4
                
-               418         446 PRECALL                  1
+               502         446 PRECALL                  1
                            450 CALL                     1
                            460 RETURN_VALUE
                
-               427     >>  462 LOAD_CONST               0 (None)
+               511     >>  462 LOAD_CONST               0 (None)
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
-               firstlineno 403
+               firstlineno 487
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
-         firstlineno 384
+         firstlineno 468
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
-         430           0 RESUME                   0
+         514           0 RESUME                   0
          
-         431           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
+         515           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
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
-         firstlineno 430
+         firstlineno 514
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
-         439           0 RESUME                   0
+         523           0 RESUME                   0
          
-         440           2 LOAD_GLOBAL              1 (NULL + QueryDict)
+         524           2 LOAD_GLOBAL              1 (NULL + QueryDict)
                       14 LOAD_CONST               1 (True)
                       16 KW_NAMES                 2
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               2 (temp)
          
-         441          34 LOAD_FAST                2 (temp)
+         525          34 LOAD_FAST                2 (temp)
                       36 LOAD_METHOD              1 (update)
                       58 LOAD_FAST                0 (querydict)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_TOP
          
-         442          76 LOAD_FAST                2 (temp)
+         526          76 LOAD_FAST                2 (temp)
                       78 LOAD_FAST                1 (key)
                       80 DELETE_SUBSCR
          
-         443          82 LOAD_FAST                2 (temp)
+         527          82 LOAD_FAST                2 (temp)
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
-         firstlineno 439
+         firstlineno 523
          lnotab 0x020120012a010601
-      'request'
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 2
-         flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         446           0 RESUME                   0
-         
-         447           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('HEAD')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
-         consts
-            None
-            'HEAD'
-         names      ('method',)
-         varnames   ('request',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       'is_head'
-         firstlineno 446
-         lnotab 0x0201
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 2
-         flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         450           0 RESUME                   0
-         
-         451           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('GET')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
-         consts
-            None
-            'GET'
-         names      ('method',)
-         varnames   ('request',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       'is_get'
-         firstlineno 450
-         lnotab 0x0201
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 2
-         flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         454           0 RESUME                   0
-         
-         455           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('POST')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
-         consts
-            None
-            'POST'
-         names      ('method',)
-         varnames   ('request',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       'is_post'
-         firstlineno 454
-         lnotab 0x0201
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 2
-         flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         458           0 RESUME                   0
-         
-         459           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('PUT')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
-         consts
-            None
-            'PUT'
-         names      ('method',)
-         varnames   ('request',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       'is_put'
-         firstlineno 458
-         lnotab 0x0201
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 2
-         flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         462           0 RESUME                   0
-         
-         463           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('PATCH')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
-         consts
-            None
-            'PATCH'
-         names      ('method',)
-         varnames   ('request',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       'is_patch'
-         firstlineno 462
-         lnotab 0x0201
+      'args'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         466           0 RESUME                   0
+         code 0x97007c006401190000000000000000005300
+         530           0 RESUME                   0
          
-         467           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('DELETE')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
+         531           2 LOAD_FAST                0 (args)
+                       4 LOAD_CONST               1 (0)
+                       6 BINARY_SUBSCR
+                      16 RETURN_VALUE
          consts
             None
-            'DELETE'
-         names      ('method',)
-         varnames   ('request',)
+            0
+         names      ()
+         varnames   ('args',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
-         name       'is_delete'
-         firstlineno 466
+         name       '_get_request_from_args'
+         firstlineno 530
          lnotab 0x0201
       (None,)
       ('outerHTML',)
       (True,)
       (None, True)
-   names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'element', 'swap_oob', 'bool', 'inject_args', '_inject_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'list', 'dict', '_extract_injected_params', '_get_request_from_args', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete')
+   names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'element', 'swap_oob', 'overload', 'list', 'get_view_fn_call_stack_from_request', 'bool', 'view', 'is_view_fn_request_target', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete', 'inject_args', '_inject_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'dict', '_extract_injected_params', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', '_get_request_from_args')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c012002080108010c010c0118
       010c0110021601160116082621160902ff02030201020102010201020102
-      f806010eff02060efa020934f7082b02ff040102ff020102ff020202fe08
-      17020102fd060214fe020314fd020434fc082004030c0118ff0e0102101e
-      1402fd040118ff020226fe020314fd020412fc08351c090c011aff0e0102
-      2f0c011aff0e01020c0c011aff0e01020c0e040e04340426231c2e0c0910
-      070c040c040c040c040c04
+      f806010eff02060efa020934f7082902ff040102ff020102ff020202fe08
+      150c011aff0e0102040c01020102ff020102ff02021afe06ff0e01020702
+      ff040102ff02021afe080940140c050c040c040c040c040c040c0b020102
+      fd060214fe020314fd020434fc082204030c0118ff0e010211020114ff02
+      0202fe020302fd02040cfc081b02fc040114ff020218fe020326fd020414
+      fc020512fb08400c011aff0e01022f0c011aff0e01020c0c011aff0e0102
+      0c0e040e04340426231c2e0c091007
```

### Comparing `dfv-0.6.0/dfv/__pycache__/test_element.cpython-311.pyc` & `dfv-0.7.0/dfv/__pycache__/test_element.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/__pycache__/test_form.cpython-311.pyc` & `dfv-0.7.0/dfv/__pycache__/test_form.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc` & `dfv-0.7.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/static/dfv.js` & `dfv-0.7.0/dfv/static/dfv.js`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc` & `dfv-0.7.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/test_element.py` & `dfv-0.7.0/dfv/test_element.py`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/test_form.py` & `dfv-0.7.0/dfv/test_form.py`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/dfv/test_params_to_args.py` & `dfv-0.7.0/dfv/test_params_to_args.py`

 * *Files identical despite different names*

### Comparing `dfv-0.6.0/pyproject.toml` & `dfv-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfv"
-version = "0.6.0"
+version = "0.7.0"
 description = "Django Function Views"
 authors = ["Roman Roelofsen <romanroe@gmail.com>"]
 include = ["dfv"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 django = "^4.1.7"
```

### Comparing `dfv-0.6.0/setup.py` & `dfv-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'django>=4.1.7,<5.0.0',
  'lxml>=4.9.2,<5.0.0',
  'typeguard',
  'wrapt>=1.15.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'dfv',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Django Function Views',
     'long_description': 'None',
     'author': 'Roman Roelofsen',
     'author_email': 'romanroe@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dfv-0.6.0/PKG-INFO` & `dfv-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfv
-Version: 0.6.0
+Version: 0.7.0
 Summary: Django Function Views
 Author: Roman Roelofsen
 Author-email: romanroe@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

