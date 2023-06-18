# Comparing `tmp/bbwebservice-0.0.7.tar.gz` & `tmp/bbwebservice-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\pypi_final\dist\.tmp-zhfna_7_\bbwebservice-0.0.7.tar", last modified: Wed Jan 25 11:51:06 2023, max compression
+gzip compressed data, was "bbwebservice-0.0.8.tar", last modified: Sun Jun 18 20:30:02 2023, max compression
```

## Comparing `bbwebservice-0.0.7.tar` & `bbwebservice-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 11:51:06.686541 bbwebservice-0.0.7/
--rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      698 2023-01-25 11:51:06.686541 bbwebservice-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      312 2022-11-22 08:20:40.000000 bbwebservice-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      522 2023-01-25 11:51:06.697669 bbwebservice-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-25 11:51:06.024972 bbwebservice-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-01-25 11:51:06.591732 bbwebservice-0.0.7/src/bbwebservice/
--rw-rw-rw-   0        0        0     2160 2023-01-01 15:47:46.000000 bbwebservice-0.0.7/src/bbwebservice/__init__.py
--rw-rw-rw-   0        0        0     1949 2022-11-22 10:00:46.000000 bbwebservice-0.0.7/src/bbwebservice/config_loader.py
--rw-rw-rw-   0        0        0     3490 2023-01-25 11:28:15.000000 bbwebservice-0.0.7/src/bbwebservice/core.py
--rw-rw-rw-   0        0        0     7361 2023-01-25 11:30:49.000000 bbwebservice-0.0.7/src/bbwebservice/http_parser.py
--rw-rw-rw-   0        0        0     5914 2023-01-01 15:22:38.000000 bbwebservice-0.0.7/src/bbwebservice/webserver.py
-drwxrwxrwx   0        0        0        0 2023-01-25 11:51:06.667845 bbwebservice-0.0.7/src/bbwebservice.egg-info/
--rw-rw-rw-   0        0        0      698 2023-01-25 11:51:05.000000 bbwebservice-0.0.7/src/bbwebservice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-01-25 11:51:05.000000 bbwebservice-0.0.7/src/bbwebservice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 11:51:05.000000 bbwebservice-0.0.7/src/bbwebservice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-01-25 11:51:05.000000 bbwebservice-0.0.7/src/bbwebservice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 20:30:02.801920 bbwebservice-0.0.8/
+-rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      698 2023-06-18 20:30:02.801920 bbwebservice-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2022-11-22 08:20:40.000000 bbwebservice-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      522 2023-06-18 20:30:02.811843 bbwebservice-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 20:30:02.168021 bbwebservice-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 20:30:02.670851 bbwebservice-0.0.8/src/bbwebservice/
+-rw-rw-rw-   0        0        0     2160 2023-01-01 15:47:46.000000 bbwebservice-0.0.8/src/bbwebservice/__init__.py
+-rw-rw-rw-   0        0        0     1949 2022-11-22 10:00:46.000000 bbwebservice-0.0.8/src/bbwebservice/config_loader.py
+-rw-rw-rw-   0        0        0     3435 2023-02-04 15:35:47.000000 bbwebservice-0.0.8/src/bbwebservice/core.py
+-rw-rw-rw-   0        0        0     7724 2023-06-18 20:27:41.000000 bbwebservice-0.0.8/src/bbwebservice/http_parser.py
+-rw-rw-rw-   0        0        0     5982 2023-06-18 20:24:41.000000 bbwebservice-0.0.8/src/bbwebservice/webserver.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:30:02.746344 bbwebservice-0.0.8/src/bbwebservice.egg-info/
+-rw-rw-rw-   0        0        0      698 2023-06-18 20:30:02.000000 bbwebservice-0.0.8/src/bbwebservice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-18 20:30:02.000000 bbwebservice-0.0.8/src/bbwebservice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:30:02.000000 bbwebservice-0.0.8/src/bbwebservice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 20:30:02.000000 bbwebservice-0.0.8/src/bbwebservice.egg-info/top_level.txt
```

### Comparing `bbwebservice-0.0.7/LICENSE` & `bbwebservice-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bbwebservice-0.0.7/PKG-INFO` & `bbwebservice-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 0.0.7
+Version: 0.0.8
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `bbwebservice-0.0.7/setup.cfg` & `bbwebservice-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6277 6562 7365 7276 6963 650d   = bbwebservice.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e37  .version = 0.0.7
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e38  .version = 0.0.8
 00000030: 0d0a 6175 7468 6f72 203d 204c 756b 6173  ..author = Lukas
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206c 756b 6173 6f67 7761 6c6b 6572 4067   lukasogwalker@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4120 6261 7265 2062  ption = A bare b
 00000080: 6f6e 6520 7765 6273 6572 7665 720d 0a6c  one webserver..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description
```

### Comparing `bbwebservice-0.0.7/src/bbwebservice/__init__.py` & `bbwebservice-0.0.8/src/bbwebservice/__init__.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-0.0.7/src/bbwebservice/config_loader.py` & `bbwebservice-0.0.8/src/bbwebservice/config_loader.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-0.0.7/src/bbwebservice/core.py` & `bbwebservice-0.0.8/src/bbwebservice/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         try:
             conn,addr = server.accept()
             worker_state = Event()
             worker_state.set()
             worker_thread = Thread(target=servlet , args = [conn,worker_state])
             SERVER_THREADS.append([worker_thread,worker_state,conn])
             worker_thread.start()
-            print("thread_count",len(SERVER_THREADS))
         except:
             if state.is_set():
                 print('[CONNECTION_ERROR] a connection failed.')
 
 def start():
 
     '''The start function starts the server. First it tries to initiate a socket Object and
```

### Comparing `bbwebservice-0.0.7/src/bbwebservice/http_parser.py` & `bbwebservice-0.0.8/src/bbwebservice/http_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,35 +38,44 @@
     res = bytes()
     parts = re.split('\n\n|\r\n\r\n',msg)  
     if len(parts) > 1:
         payload = ''.join(parts[1:])
         res = bytes(payload,'utf-8')
     return res
 
-def parse_post(args,msg,session_id)-> dict:
+def parse_post(args,msg,session_id,bin_formats)-> dict:
 
     '''Parses payload of a POST request and sends it back as a dictionary'''
-    
-    result = {'payload':''}
+
+    payload = ''
+    result = {'payload': payload}
     result['session_id'] = session_id
-    parts = re.split('\n\n|\r\n\r\n',msg)  
-    if len(parts) > 1:
-        payload = ''.join(parts[1:])
-        if 'content-type' in args:
-            content_type = args['content-type']
-            result['content-type'] = content_type
-            if  content_type == 'application/x-www-form-urlencoded':
-                key_value = payload.split('&')
-                result['payload'] = {}
-                for pair in key_value:
-                    p = pair.split('=')
-                    if len(p) == 2:
-                        result['payload'][urllib.parse.unquote(p[0])] = urllib.parse.unquote(p[1])
+    try:
+        if len(msg) > 1:
+            payload = None
+            try:
+                payload = str(msg,'utf-8')
+            except:
+                pass
+            if 'content-type' in args and args['content-type'] not in bin_formats and payload:
+                content_type = args['content-type']
+                result['content-type'] = content_type
+                if  content_type == 'application/x-www-form-urlencoded':
+                    key_value = payload.split('&')
+                    result['payload'] = {}
+                    for pair in key_value:
+                        p = pair.split('=')
+                        if len(p) == 2:
+                            result['payload'][urllib.parse.unquote(p[0])] = urllib.parse.unquote(p[1])
+                else:
+                    result['payload'] = payload
             else:
-                result['payload'] = payload         
+                result['payload'] = msg
+    except Exception as e:
+        print("ERROR",e,msg,args)
     return result
 
 def get_query_string(path) ->dict:
     parts = re.split('\?(?!.+\/)',path)
     outer_args = {}
     inner_args = {}
     if len(parts) > 1:
@@ -110,18 +119,19 @@
     HEADER += 'connection: close\n'
     HEADER += f"content-length: {length}\n"
     HEADER += 'content-language: en\n'
     HEADER += f"content-type: text/plain\n"
     HEADER += '\n'+CONTENT  
     return HEADER          
 
-BIN_FORMATS = ['video/mp4',"image/png"]
+BIN_FORMATS = ['video/mp4',"image/png",'audio/webm']
            
 def parse_message(conn:socket.socket) -> bytes:
-    message = str(conn.recv(2048),'utf-8')
+    raw_message,_,post = conn.recv(2048).partition(b'\r\n\r\n')
+    message = str(raw_message,'utf-8')
     ERROR_0 = f'{HTTPProtocol.HTTP_1_1} {HTTPStatus.getString(HTTPStatus.ERROR)}\n\r'
     ERROR = f'{HTTPProtocol.HTTP_1_1} {HTTPStatus.getString(HTTPStatus.NO_CONTENT)}\n\r'
     session_id = str(uuid.uuid1().int)
     if len(message) == 0:
         conn.close()
         return ERROR_0.encode('utf-8')
     lines = re.split('\n|\r\n',message)
@@ -179,18 +189,18 @@
         HEADER += SESSION_COOKIE
         
     if TYPE == HTTPMessageType.POST:
         if PATH not in core.POST_HANDLER:
             log_request(message)
             return get_notfound_msg(ERROR_0).encode('utf-8')
         mimetype = core.POST_HANDLER[PATH][1]
-        missing_bytes = get_content_length(tokens_1)-len(get_payload(message))
+        missing_bytes = get_content_length(tokens_1)-len(post)
         if missing_bytes > 0:
-            message += str(conn.recv(missing_bytes),'utf-8')
-        args = parse_post(tokens_1,message,session_id)
+            post += conn.recv(missing_bytes)
+        args = parse_post(tokens_1,post,session_id,BIN_FORMATS)
         if mimetype == 'text/css':
              CONTENT = '\n'+re.sub('(?<=;|{|})\s+','', core.POST_HANDLER[PATH][0]({**args,**QUERY_STRING_ARGS}))
         else:
             CONTENT = core.POST_HANDLER[PATH][0]({**args,**QUERY_STRING_ARGS})
         HEADER += f'{HTTPProtocol.HTTP_1_1} {HTTPStatus.getString(HTTPStatus.OK)}\n'
         HEADER += f'accept-ranges: bytes\n'
         length = 0
```

### Comparing `bbwebservice-0.0.7/src/bbwebservice/webserver.py` & `bbwebservice-0.0.8/src/bbwebservice/webserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CSS = 'text/css'
     ICO = "image/x-icon"
     PNG = "image/png"
     SVG = "image/svg+xml"
     TEXT = "text/plain"
     MP4 = "video/mp4"
     JSON = "application/json"
+    WEBM_AUDIO = "audio/webm"
 
 class STORE_VARS:
     '''Keys used to access attributes of the dict provided to the respective handler methods'''
     SESSION_ID = 'session_id'
     QUERY_STRING = 'query_string'
 
 class LOGGING_OPTIONS:
@@ -110,26 +111,26 @@
     If a variable name starts with an underscore "_" the python code wrapped in curley braces will be substituded by it's content.
     The values passed with the args dictionary can be accessed with the globals() function in the targeted file'''
 
     content = ''
     try:
         with open(MAIN_PATH+path,'r',encoding='utf-8') as page:
             content = '\n'.join(page.readlines())
-            
-        to_eval= re.finditer("{{(.|\n)*?}}",content)
+            res_content = content[:]
+        to_eval = re.finditer("{{(.|\n)*?}}",content)
         for var in to_eval:
             OUTPUT = {}
             var = content[var.span()[0]:var.span()[1]]
             exec(compile(var.strip('{{}}'),'temp','exec'),args,OUTPUT)
             insert = '\n'.join([str(OUTPUT[x]) for x in OUTPUT.keys() if x[0] == '_'])
-            content = content.replace(var,insert)
+            res_content = res_content.replace(var,insert)
     except Exception as e:
         print('[RENDERER] Error with rendering Page.')
         print(e)
-    return content
+    return res_content
 
 def substitude_vars(content:str, vars:dict) -> str:
     
     '''This function accepts a string and substitudes all "%% + key + %%" with the according value from the dictionary'''
     
     try:
         _content = content
```

### Comparing `bbwebservice-0.0.7/src/bbwebservice.egg-info/PKG-INFO` & `bbwebservice-0.0.8/src/bbwebservice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 0.0.7
+Version: 0.0.8
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

