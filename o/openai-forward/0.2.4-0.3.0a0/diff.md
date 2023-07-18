# Comparing `tmp/openai_forward-0.2.4.tar.gz` & `tmp/openai_forward-0.3.0a0.tar.gz`

## Comparing `openai_forward-0.2.4.tar` & `openai_forward-0.3.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/__init__.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/__main__.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/app.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/base.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/config.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/openai.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.4/LICENSE
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 openai_forward-0.2.4/README.md
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 openai_forward-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 openai_forward-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/__main__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/app.py
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/base.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/config.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/openai.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/content/chat.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/content/whisper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12172 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/PKG-INFO
```

### Comparing `openai_forward-0.2.4/openai_forward/__main__.py` & `openai_forward-0.3.0a0/openai_forward/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,20 +56,20 @@
             workers=workers,
             app_dir="..",
             ssl_keyfile=ssl_keyfile,
             ssl_certfile=ssl_certfile,
         )
 
     @staticmethod
-    def convert(log_path: str = "./Log/chat.log", target_path: str = "./Log/chat.json"):
-        """Convert log file  to jsonl file"""
-        from openai_forward.tool import convert_chatlog_to_jsonl
+    def convert(log_folder: str = "./Log/chat", target_path: str = "./Log/chat.json"):
+        """Convert log folder to jsonl file"""
+        from openai_forward.tool import convert_folder_to_jsonl
 
-        print(f"Convert {log_path} to {target_path}")
-        convert_chatlog_to_jsonl(log_path, target_path)
+        print(f"Convert {log_folder}/*.log to {target_path}")
+        convert_folder_to_jsonl(log_folder, target_path)
 
 
 def main():
     fire.Fire(Cli)
 
 
 if __name__ == "__main__":
```

### Comparing `openai_forward-0.2.4/openai_forward/base.py` & `openai_forward-0.3.0a0/openai_forward/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from fastapi import HTTPException, Request, status
 from fastapi.responses import StreamingResponse
 from loguru import logger
 from starlette.background import BackgroundTask
 
 from .config import print_startup_info, setting_log
 from .content.chat import ChatSaver
+from .content.whisper import WhisperSaver
 from .tool import env2list
 
 
 class OpenaiBase:
     BASE_URL = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com").strip()
     ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "").strip()
     _LOG_CHAT = os.environ.get("LOG_CHAT", "False").strip().lower() == "true"
@@ -32,14 +33,15 @@
 
     print_startup_info(
         BASE_URL, ROUTE_PREFIX, _openai_api_key_list, _no_auth_mode, _LOG_CHAT
     )
     if _LOG_CHAT:
         setting_log(save_file=False)
         chatsaver = ChatSaver()
+        whispersaver = WhisperSaver()
 
     def validate_request_host(self, ip):
         if self.IP_WHITELIST and ip not in self.IP_WHITELIST:
             raise HTTPException(
                 status_code=status.HTTP_403_FORBIDDEN,
                 detail=f"Forbidden, ip={ip} not in whitelist!",
             )
@@ -52,46 +54,53 @@
     @classmethod
     async def aiter_bytes(cls, r: httpx.Response, route_path: str, uid: str):
         bytes_ = b""
         async for chunk in r.aiter_bytes():
             bytes_ += chunk
             yield chunk
         try:
-            target_info = cls.chatsaver.parse_bytes_to_content(bytes_, route_path)
-            cls.chatsaver.add_chat(
-                {target_info["role"]: target_info["content"], "uid": uid}
-            )
+            if route_path == "/v1/chat/completions":
+                target_info = cls.chatsaver.parse_bytes_to_content(bytes_, route_path)
+                cls.chatsaver.add_chat(
+                    {target_info["role"]: target_info["content"], "uid": uid}
+                )
+            elif route_path.startswith("/v1/audio/"):
+                cls.whispersaver.add_log(bytes_)
         except Exception as e:
             logger.debug(f"log chat (not) error:\n{e=}")
 
     @classmethod
     async def _reverse_proxy(cls, request: Request):
         client = httpx.AsyncClient(base_url=cls.BASE_URL, http1=True, http2=False)
         url_path = request.url.path
         url_path = url_path[len(cls.ROUTE_PREFIX) :]
         url = httpx.URL(path=url_path, query=request.url.query.encode("utf-8"))
         headers = dict(request.headers)
         auth = headers.pop("authorization", "")
-        auth_headers_dict = {"Content-Type": "application/json", "Authorization": auth}
+        content_type = headers.pop("content-type", "application/json")
+        auth_headers_dict = {"Content-Type": content_type, "Authorization": auth}
         auth_prefix = "Bearer "
         if cls._no_auth_mode or auth and auth[len(auth_prefix) :] in cls._FWD_KEYS:
             auth = auth_prefix + next(cls._cycle_api_key)
             auth_headers_dict["Authorization"] = auth
 
-        log_chat_completions = False
+        if_log = False
         uid = None
         if cls._LOG_CHAT and request.method == "POST":
             try:
-                chat_info = await cls.chatsaver.parse_payload_to_content(
-                    request, route_path=url_path
-                )
-                if chat_info:
-                    cls.chatsaver.add_chat(chat_info)
-                    uid = chat_info.get("uid")
-                    log_chat_completions = True
+                if url_path.startswith("/v1/audio/"):
+                    if_log = True
+                else:
+                    chat_info = await cls.chatsaver.parse_payload_to_content(
+                        request, route_path=url_path
+                    )
+                    if chat_info:
+                        cls.chatsaver.add_chat(chat_info)
+                        uid = chat_info.get("uid")
+                        if_log = True
             except Exception as e:
                 logger.debug(
                     f"log chat error:\n{request.client.host=} {request.method=}: {e}"
                 )
 
         req = client.build_request(
             request.method,
@@ -113,18 +122,14 @@
             )
         except Exception as e:
             logger.exception(f"{type(e)}:")
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=e
             )
 
-        aiter_bytes = (
-            cls.aiter_bytes(r, url_path, uid)
-            if log_chat_completions
-            else r.aiter_bytes()
-        )
+        aiter_bytes = cls.aiter_bytes(r, url_path, uid) if if_log else r.aiter_bytes()
         return StreamingResponse(
             aiter_bytes,
             status_code=r.status_code,
             media_type=r.headers.get("content-type"),
             background=BackgroundTask(r.aclose),
         )
```

### Comparing `openai_forward-0.2.4/openai_forward/config.py` & `openai_forward-0.3.0a0/openai_forward/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,20 +65,27 @@
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
 
     config_handlers = [
         {"sink": sys.stdout, "level": "DEBUG"},
         {
-            "sink": f"./Log/chat.log",
+            "sink": f"./Log/chat/chat.log",
             "enqueue": multi_process,
-            "rotation": "20 MB",
+            "rotation": "50 MB",
             "filter": lambda record: "chat" in record["extra"],
             "format": "{message}",
         },
+        {
+            "sink": f"./Log/whisper/whisper.log",
+            "enqueue": multi_process,
+            "rotation": "30 MB",
+            "filter": lambda record: "whisper" in record["extra"],
+            "format": "{message}",
+        },
     ]
     if save_file:
         config_handlers += [
             {
                 "sink": f"./Log/{log_name}.log",
                 "enqueue": multi_process,
                 "rotation": "100 MB",
```

### Comparing `openai_forward-0.2.4/openai_forward/openai.py` & `openai_forward-0.3.0a0/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.4/openai_forward/content/chat.py` & `openai_forward-0.3.0a0/openai_forward/content/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+import time
 import uuid
 
 import orjson
 from fastapi import Request
 from httpx._decoders import LineDecoder
 from loguru import logger
 from orjson import JSONDecodeError
 
 decoder = LineDecoder()
 
 
 def _parse_iter_line_content(line: str):
-    line = line[6:]
     try:
         line_dict = orjson.loads(line)
         return line_dict["choices"][0]["delta"]["content"]
     except JSONDecodeError:
         return ""
     except KeyError:
         return ""
 
 
 def parse_chat_completions(bytes_: bytes):
     txt_lines = decoder.decode(bytes_.decode("utf-8"))
     line0 = txt_lines[0]
     target_info = dict()
-    if line0.startswith("data:"):
+    _start_token = "data: "
+    if line0.startswith(_start_token):
         is_stream = True
-        line0 = orjson.loads(line0[6:])
+        line0 = orjson.loads(line0[len(_start_token) :])
         msg = line0["choices"][0]["delta"]
     else:
         is_stream = False
         line0 = orjson.loads("".join(txt_lines))
         msg = line0["choices"][0]["message"]
 
     target_info["created"] = line0["created"]
@@ -40,16 +41,18 @@
     target_info["content"] = msg.get("content", "")
     if not is_stream:
         return target_info
     # loop for stream
     for line in txt_lines[1:]:
         if line in ("", "\n", "\n\n"):
             continue
-        elif line.startswith("data: "):
-            target_info["content"] += _parse_iter_line_content(line)
+        elif line.startswith(_start_token):
+            target_info["content"] += _parse_iter_line_content(
+                line[len(_start_token) :]
+            )
         else:
             logger.warning(f"line not startswith data: {line}")
     return target_info
 
 
 class ChatSaver:
     def __init__(self):
@@ -63,14 +66,15 @@
             msgs = payload["messages"]
             model = payload["model"]
             content = {
                 "messages": [{msg["role"]: msg["content"]} for msg in msgs],
                 "model": model,
                 "forwarded-for": request.headers.get("x-forwarded-for") or "",
                 "uid": uid,
+                "datetime": time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
             }
         else:
             content = {}
         return content
 
     @staticmethod
     def parse_bytes_to_content(bytes_: bytes, route_path: str):
```

### Comparing `openai_forward-0.2.4/openai_forward/routers/openai_v1.py` & `openai_forward-0.3.0a0/openai_forward/routers/openai_v1.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.4/openai_forward/routers/schemas.py` & `openai_forward-0.3.0a0/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.4/.gitignore` & `openai_forward-0.3.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.4/LICENSE` & `openai_forward-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.4/README.md` & `openai_forward-0.3.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**中文** | [**English**](./README_EN.md)
+**中文** | ~~[**English**](./README_EN.md)~~
 
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
 <p align="center">
@@ -51,66 +51,76 @@
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问OpenAI API的(云)服务器上，
 通过该服务转发OpenAI的请求。即搭建反向代理服务; 允许输入多个OpenAI API-KEY 组成轮询池; 可自定义二次分发api key.
 
 ---
 
 由本项目搭建的长期代理地址：
 > https://api.openai-forward.com  
+> https://cloudflare.worker.openai-forward.com  
+> https://cloudflare.page.openai-forward.com  
+> https://vercel.openai-forward.com  
+> https://render.openai-forward.com  
+> https://railway.openai-forward.com
 
 ## 功能
 
 **基础功能**
 
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
 - [x] cloudflare 部署
-- [x] ~~Vercel一键部署(不建议)~~
+- [x] Vercel一键部署
 - [x] Railway 一键部署
 - [x] Render 一键部署
 
 **高级功能**
 
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 转发api key (见[高级配置](#高级配置))
 - [x] 流式响应对话日志
 
 ## 部署指南
 
-[部署文档](deploy.md)
+👉 [部署文档](deploy.md)
 
 提供以下几种部署方式  
 **有海外vps方案**
 
-1. [pip 安装部署](deploy.md#pip部署) (推荐)
-2. [Docker部署](deploy.md#docker部署) (推荐)
+1. [pip 安装部署](deploy.md#pip部署)
+2. [Docker部署](deploy.md#docker部署)
    > https://api.openai-forward.com
 
 **无vps免费部署方案**
 
-1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
-   > ~~https://vercel.openai-forward.com~~
-2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
-   > https://cloudflare.page.openai-forward.com
-3. [Railway部署](deploy.md#Railway-一键部署)
+1. [Railway部署](deploy.md#Railway-一键部署)
    > https://railway.openai-forward.com
-4. [Render一键部署](deploy.md#render-一键部署) (推荐)
+2. [Render一键部署](deploy.md#render-一键部署)
    > https://render.openai-forward.com
 
+---
+下面的部署仅提供单一转发功能
+
+3. [一键Vercel部署](deploy.md#vercel-一键部署)
+   > https://vercel.openai-forward.com
+4. [cloudflare部署](deploy.md#cloudflare-部署)
+   > https://cloudflare.page.openai-forward.com
+
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
 
-<details markdown="1">
-<summary>Click for more details</summary>  
+
+<details >
+   <summary> details</summary>  
 
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
     -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="kunyuan" \
@@ -127,15 +137,15 @@
 
 ```diff
   import openai
 + openai.api_base = "https://api.openai-forward.com/v1"
   openai.api_key = "sk-******"
 ```
 
-<details markdown="1">
+<details open>
   <summary>More Examples</summary>
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
@@ -175,62 +185,61 @@
 ## 配置选项
 
 配置的设置方式支持两种  
 一种为在命令行中执行`openai-forward run`的运行参数(如`--port=8000`)中指定;  
 另一种为读取环境变量的方式指定。
 
 ### 命令行参数
+
 可通过 `openai-forward run --help` 查看
 
-<details markdown="1">
+<details open>
   <summary>Click for more details</summary>
 
 **`openai-forward run`参数配置项**
 
 | 配置项 | 说明                |          默认值           |
 |-----------------|-------------------|:----------------------:|
 | --port | 服务端口号             |          8000          |
 | --workers | 工作进程数             |           1            |
 | --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
 | --api_key | 同 OPENAI_API_KEY  |         `None`         |
 | --forward_key | 同 FORWARD_KEY     |         `None`         |
 | --route_prefix | 同 ROUTE_PREFIX    |          `None`          |
 | --log_chat | 同 LOG_CHAT        |        `False`         |
 
-
 </details>
 
 ### 环境变量配置项
+
 支持从运行目录下的`.env`文件中读取
 
 | 环境变量            | 说明                                                                                                                                |           默认值            |
 |-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
 | OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
 | ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
 | LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
-
 ## 高级配置
 
 **设置openai api_key为自定义的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
 <details markdown="1">
   <summary>Click for more details</summary>
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
 ```
 
 这里我们配置了FORWARD_KEY为`fk-******`, 那么后面客户端在调用时只需设置OPENAI_API_KEY为我们自定义的`fk-******` 即可。  
-这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配代理服务使用（如下面的例子）
-而无需担心OPENAI_API_KEY被泄露。  
-并且可以对外分发`fk-******`
+这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用自定义的api-key`fk-******`,
+无需担心真正的OPENAI_API_KEY被泄露。并且可以对外分发`fk-******`。
 
 **用例:**
 
 ```bash
 curl https://api.openai-forward.com/v1/chat/completions \
   -H "Content-Type: application/json" \
   -H "Authorization: Bearer fk-******" \
@@ -261,15 +270,15 @@
 ``` 
 
 </details>
 
 ## 对话日志
 
 默认不记录对话日志，若要开启需设置环境变量`LOG_CHAT=true`
-<details markdown="1">
+<details open>
   <summary>Click for more details</summary>
 
 保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
 {'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-**ä¸­æ** | [**English**](./README_EN.md)
+**ä¸­æ** | ~~[**English**](./README_EN.md)~~
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
@@ -13,37 +13,40 @@
      deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
                  github.com/beidongjiedeguang/openai-forward)
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®OpenAI
 APIç(äº)æå¡å¨ä¸ï¼
 éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡;
 åè®¸è¾å¥å¤ä¸ªOpenAI API-KEY ç»æè½®è¯¢æ± ; å¯èªå®ä¹äºæ¬¡ååapi
 key. --- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-
-forward.com ## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ -
-[x] æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½²
-- [x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
-(ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
-**é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key ç»æè½®è¯¢æ±  - [x]
-èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®](#é«çº§éç½®)) - [x]
-æµå¼ååºå¯¹è¯æ¥å¿ ## é¨ç½²æå [é¨ç½²ææ¡£](deploy.md)
-æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²]
-(deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²](deploy.md#dockeré¨ç½²)
-(æ¨è) > https://api.openai-forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1.
-[ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://
-vercel.openai-forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²)
-(æ¨è) > https://cloudflare.page.openai-forward.com 3. [Railwayé¨ç½²]
-(deploy.md#Railway-ä¸é®é¨ç½²) > https://railway.openai-forward.com 4.
-[Renderä¸é®é¨ç½²](deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://
-render.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
+forward.com > https://cloudflare.worker.openai-forward.com > https://
+cloudflare.page.openai-forward.com > https://vercel.openai-forward.com > https:
+//render.openai-forward.com > https://railway.openai-forward.com ## åè½
+**åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº
+- [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½²
+- [x] cloudflare é¨ç½² - [x] Vercelä¸é®é¨ç½² - [x] Railway ä¸é®é¨ç½² -
+[x] Render ä¸é®é¨ç½² **é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
+ç»æè½®è¯¢æ±  - [x] èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®]
+(#é«çº§éç½®)) - [x] æµå¼ååºå¯¹è¯æ¥å¿ ## é¨ç½²æå ð
+[é¨ç½²ææ¡£](deploy.md) æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡**
+1. [pip å®è£é¨ç½²](deploy.md#pipé¨ç½²) 2. [Dockeré¨ç½²]
+(deploy.md#dockeré¨ç½²) > https://api.openai-forward.com
+**æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [Railwayé¨ç½²](deploy.md#Railway-ä¸é®é¨ç½²)
+> https://railway.openai-forward.com 2. [Renderä¸é®é¨ç½²](deploy.md#render-
+ä¸é®é¨ç½²) > https://render.openai-forward.com --
+- ä¸é¢çé¨ç½²ä»æä¾åä¸è½¬ååè½ 3. [ä¸é®Vercelé¨ç½²]
+(deploy.md#vercel-ä¸é®é¨ç½²) > https://vercel.openai-forward.com 4.
+[cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) > https://
+cloudflare.page.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
 chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
 github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
 æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
-`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
-```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
-e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
-chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å   details ```bash docker
+run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://
+api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
+è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
 **Python** ```diff import openai + openai.api_base = "https://api.openai-
 forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
 ```diff import { Configuration } from "openai"; const configuration = new
 Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey: "sk-
 ******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-forward.com/
 v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
@@ -77,25 +80,25 @@
 è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` | ##
 é«çº§éç½® **è®¾ç½®openai api_keyä¸ºèªå®ä¹çforward key** éè¦éç½®
 OPENAI_API_KEY å FORWARD_KEY, ä¾å¦  Click for more details ```bash
 OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
 tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
-è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
-******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
-èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã å¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-******`
-**ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
-H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
-d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
-"Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base = "https:/
-/api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
-"fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
-e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
-e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
+è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨èªå®ä¹çapi-
+key`fk-******`,
+æ éæå¿çæ­£çOPENAI_API_KEYè¢«æ³é²ãå¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-
+******`ã **ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/
+completions \ -H "Content-Type: application/json" \ -H "Authorization: Bearer
+fk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user",
+"content": "Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base
+= "https://api.openai-forward.com/v1" - openai.api_key = "sk-******" +
+openai.api_key = "fk-******" ``` **Web application** ```bash docker run -d \ -
+p 3000:3000 \ -e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-
+forward.com" \ -e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
 é»è®¤ä¸è®°å½å¯¹è¯æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
 Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
 chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
 e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
 '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
```

### Comparing `openai_forward-0.2.4/pyproject.toml` & `openai_forward-0.3.0a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
     "loguru",
-    "sparrow-python>=0.1.3",
+    "sparrow-python>=0.1.5",
     "fastapi",
     "uvicorn",
     "orjson",
     "python-dotenv",
     "httpx",
     "pytz",
 ]
@@ -34,16 +34,17 @@
 [project.urls]
 Homepage = "https://github.com/beidongjiedeguang/openai-forward"
 Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forward"
 Issues = "https://github.com/beidongjiedeguang/openai-forward/issues"
 Source = "https://github.com/beidongjiedeguang/openai-forward"
 
 [project.optional-dependencies]
-tool = [
-    "orjsonl"
+test = [
+    "openai",
+    "pytest",
 ]
 
 [project.scripts]
 openai_forward = "openai_forward.__main__:main"
 openai-forward = "openai_forward.__main__:main"
 aifwd = "openai_forward.__main__:main"
```

### Comparing `openai_forward-0.2.4/PKG-INFO` & `openai_forward-0.3.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.2.4
+Version: 0.3.0a0
 Summary: 🚀 OpenAI API Reverse Proxy · ChatGPT API Proxy
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
@@ -16,21 +16,22 @@
 Requires-Python: >=3.6
 Requires-Dist: fastapi
 Requires-Dist: httpx
 Requires-Dist: loguru
 Requires-Dist: orjson
 Requires-Dist: python-dotenv
 Requires-Dist: pytz
-Requires-Dist: sparrow-python>=0.1.3
+Requires-Dist: sparrow-python>=0.1.5
 Requires-Dist: uvicorn
-Provides-Extra: tool
-Requires-Dist: orjsonl; extra == 'tool'
+Provides-Extra: test
+Requires-Dist: openai; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-**中文** | [**English**](./README_EN.md)
+**中文** | ~~[**English**](./README_EN.md)~~
 
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
 <p align="center">
@@ -79,66 +80,76 @@
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问OpenAI API的(云)服务器上，
 通过该服务转发OpenAI的请求。即搭建反向代理服务; 允许输入多个OpenAI API-KEY 组成轮询池; 可自定义二次分发api key.
 
 ---
 
 由本项目搭建的长期代理地址：
 > https://api.openai-forward.com  
+> https://cloudflare.worker.openai-forward.com  
+> https://cloudflare.page.openai-forward.com  
+> https://vercel.openai-forward.com  
+> https://render.openai-forward.com  
+> https://railway.openai-forward.com
 
 ## 功能
 
 **基础功能**
 
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
 - [x] cloudflare 部署
-- [x] ~~Vercel一键部署(不建议)~~
+- [x] Vercel一键部署
 - [x] Railway 一键部署
 - [x] Render 一键部署
 
 **高级功能**
 
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 转发api key (见[高级配置](#高级配置))
 - [x] 流式响应对话日志
 
 ## 部署指南
 
-[部署文档](deploy.md)
+👉 [部署文档](deploy.md)
 
 提供以下几种部署方式  
 **有海外vps方案**
 
-1. [pip 安装部署](deploy.md#pip部署) (推荐)
-2. [Docker部署](deploy.md#docker部署) (推荐)
+1. [pip 安装部署](deploy.md#pip部署)
+2. [Docker部署](deploy.md#docker部署)
    > https://api.openai-forward.com
 
 **无vps免费部署方案**
 
-1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
-   > ~~https://vercel.openai-forward.com~~
-2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
-   > https://cloudflare.page.openai-forward.com
-3. [Railway部署](deploy.md#Railway-一键部署)
+1. [Railway部署](deploy.md#Railway-一键部署)
    > https://railway.openai-forward.com
-4. [Render一键部署](deploy.md#render-一键部署) (推荐)
+2. [Render一键部署](deploy.md#render-一键部署)
    > https://render.openai-forward.com
 
+---
+下面的部署仅提供单一转发功能
+
+3. [一键Vercel部署](deploy.md#vercel-一键部署)
+   > https://vercel.openai-forward.com
+4. [cloudflare部署](deploy.md#cloudflare-部署)
+   > https://cloudflare.page.openai-forward.com
+
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
 
-<details markdown="1">
-<summary>Click for more details</summary>  
+
+<details >
+   <summary> details</summary>  
 
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
     -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="kunyuan" \
@@ -155,15 +166,15 @@
 
 ```diff
   import openai
 + openai.api_base = "https://api.openai-forward.com/v1"
   openai.api_key = "sk-******"
 ```
 
-<details markdown="1">
+<details open>
   <summary>More Examples</summary>
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
@@ -203,62 +214,61 @@
 ## 配置选项
 
 配置的设置方式支持两种  
 一种为在命令行中执行`openai-forward run`的运行参数(如`--port=8000`)中指定;  
 另一种为读取环境变量的方式指定。
 
 ### 命令行参数
+
 可通过 `openai-forward run --help` 查看
 
-<details markdown="1">
+<details open>
   <summary>Click for more details</summary>
 
 **`openai-forward run`参数配置项**
 
 | 配置项 | 说明                |          默认值           |
 |-----------------|-------------------|:----------------------:|
 | --port | 服务端口号             |          8000          |
 | --workers | 工作进程数             |           1            |
 | --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
 | --api_key | 同 OPENAI_API_KEY  |         `None`         |
 | --forward_key | 同 FORWARD_KEY     |         `None`         |
 | --route_prefix | 同 ROUTE_PREFIX    |          `None`          |
 | --log_chat | 同 LOG_CHAT        |        `False`         |
 
-
 </details>
 
 ### 环境变量配置项
+
 支持从运行目录下的`.env`文件中读取
 
 | 环境变量            | 说明                                                                                                                                |           默认值            |
 |-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
 | OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
 | ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
 | LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
-
 ## 高级配置
 
 **设置openai api_key为自定义的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
 <details markdown="1">
   <summary>Click for more details</summary>
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
 ```
 
 这里我们配置了FORWARD_KEY为`fk-******`, 那么后面客户端在调用时只需设置OPENAI_API_KEY为我们自定义的`fk-******` 即可。  
-这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配代理服务使用（如下面的例子）
-而无需担心OPENAI_API_KEY被泄露。  
-并且可以对外分发`fk-******`
+这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用自定义的api-key`fk-******`,
+无需担心真正的OPENAI_API_KEY被泄露。并且可以对外分发`fk-******`。
 
 **用例:**
 
 ```bash
 curl https://api.openai-forward.com/v1/chat/completions \
   -H "Content-Type: application/json" \
   -H "Authorization: Bearer fk-******" \
@@ -289,15 +299,15 @@
 ``` 
 
 </details>
 
 ## 对话日志
 
 默认不记录对话日志，若要开启需设置环境变量`LOG_CHAT=true`
-<details markdown="1">
+<details open>
   <summary>Click for more details</summary>
 
 保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
 {'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.2.4 Summary: ð OpenAI
-API Reverse Proxy Â· ChatGPT API Proxy Project-URL: Homepage, https://
+Metadata-Version: 2.1 Name: openai_forward Version: 0.3.0a0 Summary: ð
+OpenAI API Reverse Proxy Â· ChatGPT API Proxy Project-URL: Homepage, https://
 github.com/beidongjiedeguang/openai-forward Project-URL: Documentation, https:/
 /github.com/beidongjiedeguang/openai-forward#openai-forward Project-URL:
 Issues, https://github.com/beidongjiedeguang/openai-forward/issues Project-URL:
 Source, https://github.com/beidongjiedeguang/openai-forward Author-email:
 kunyuan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
 Forwarding,chatgpt,fastapi,openai,openai-api,openai-proxy,python,streaming-api
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Requires-Dist: fastapi Requires-Dist: httpx Requires-
 Dist: loguru Requires-Dist: orjson Requires-Dist: python-dotenv Requires-Dist:
-pytz Requires-Dist: sparrow-python>=0.1.3 Requires-Dist: uvicorn Provides-
-Extra: tool Requires-Dist: orjsonl; extra == 'tool' Description-Content-Type:
-text/markdown **ä¸­æ** | [**English**](./README_EN.md)
+pytz Requires-Dist: sparrow-python>=0.1.5 Requires-Dist: uvicorn Provides-
+Extra: test Requires-Dist: openai; extra == 'test' Requires-Dist: pytest; extra
+== 'test' Description-Content-Type: text/markdown **ä¸­æ** | ~~[**English**]
+(./README_EN.md)~~
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
@@ -28,37 +29,40 @@
      deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
                  github.com/beidongjiedeguang/openai-forward)
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®OpenAI
 APIç(äº)æå¡å¨ä¸ï¼
 éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡;
 åè®¸è¾å¥å¤ä¸ªOpenAI API-KEY ç»æè½®è¯¢æ± ; å¯èªå®ä¹äºæ¬¡ååapi
 key. --- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-
-forward.com ## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ -
-[x] æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½²
-- [x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
-(ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
-**é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key ç»æè½®è¯¢æ±  - [x]
-èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®](#é«çº§éç½®)) - [x]
-æµå¼ååºå¯¹è¯æ¥å¿ ## é¨ç½²æå [é¨ç½²ææ¡£](deploy.md)
-æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²]
-(deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²](deploy.md#dockeré¨ç½²)
-(æ¨è) > https://api.openai-forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1.
-[ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://
-vercel.openai-forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²)
-(æ¨è) > https://cloudflare.page.openai-forward.com 3. [Railwayé¨ç½²]
-(deploy.md#Railway-ä¸é®é¨ç½²) > https://railway.openai-forward.com 4.
-[Renderä¸é®é¨ç½²](deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://
-render.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
+forward.com > https://cloudflare.worker.openai-forward.com > https://
+cloudflare.page.openai-forward.com > https://vercel.openai-forward.com > https:
+//render.openai-forward.com > https://railway.openai-forward.com ## åè½
+**åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº
+- [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½²
+- [x] cloudflare é¨ç½² - [x] Vercelä¸é®é¨ç½² - [x] Railway ä¸é®é¨ç½² -
+[x] Render ä¸é®é¨ç½² **é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
+ç»æè½®è¯¢æ±  - [x] èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®]
+(#é«çº§éç½®)) - [x] æµå¼ååºå¯¹è¯æ¥å¿ ## é¨ç½²æå ð
+[é¨ç½²ææ¡£](deploy.md) æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡**
+1. [pip å®è£é¨ç½²](deploy.md#pipé¨ç½²) 2. [Dockeré¨ç½²]
+(deploy.md#dockeré¨ç½²) > https://api.openai-forward.com
+**æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [Railwayé¨ç½²](deploy.md#Railway-ä¸é®é¨ç½²)
+> https://railway.openai-forward.com 2. [Renderä¸é®é¨ç½²](deploy.md#render-
+ä¸é®é¨ç½²) > https://render.openai-forward.com --
+- ä¸é¢çé¨ç½²ä»æä¾åä¸è½¬ååè½ 3. [ä¸é®Vercelé¨ç½²]
+(deploy.md#vercel-ä¸é®é¨ç½²) > https://vercel.openai-forward.com 4.
+[cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) > https://
+cloudflare.page.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
 chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
 github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
 æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
-`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
-```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
-e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
-chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å   details ```bash docker
+run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://
+api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
+è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
 **Python** ```diff import openai + openai.api_base = "https://api.openai-
 forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
 ```diff import { Configuration } from "openai"; const configuration = new
 Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey: "sk-
 ******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-forward.com/
 v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
@@ -92,25 +96,25 @@
 è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` | ##
 é«çº§éç½® **è®¾ç½®openai api_keyä¸ºèªå®ä¹çforward key** éè¦éç½®
 OPENAI_API_KEY å FORWARD_KEY, ä¾å¦  Click for more details ```bash
 OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
 tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
-è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
-******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
-èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã å¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-******`
-**ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
-H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
-d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
-"Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base = "https:/
-/api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
-"fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
-e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
-e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
+è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨èªå®ä¹çapi-
+key`fk-******`,
+æ éæå¿çæ­£çOPENAI_API_KEYè¢«æ³é²ãå¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-
+******`ã **ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/
+completions \ -H "Content-Type: application/json" \ -H "Authorization: Bearer
+fk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user",
+"content": "Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base
+= "https://api.openai-forward.com/v1" - openai.api_key = "sk-******" +
+openai.api_key = "fk-******" ``` **Web application** ```bash docker run -d \ -
+p 3000:3000 \ -e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-
+forward.com" \ -e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
 é»è®¤ä¸è®°å½å¯¹è¯æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
 Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
 chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
 e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
 '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
```

